# Comparing `tmp/pydantic_sqlite-0.2.1.tar.gz` & `tmp/pydantic_sqlite-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_sqlite-0.2.1.tar", max compression
+gzip compressed data, was "pydantic_sqlite-0.2.2.tar", max compression
```

## Comparing `pydantic_sqlite-0.2.1.tar` & `pydantic_sqlite-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1064 2022-01-10 15:31:20.858876 pydantic_sqlite-0.2.1/LICENSE
--rw-r--r--   0        0        0     5980 2022-01-10 15:31:20.858876 pydantic_sqlite-0.2.1/README.md
--rw-r--r--   0        0        0      109 2022-01-10 15:31:20.862876 pydantic_sqlite-0.2.1/pydantic_sqlite/__init__.py
--rw-r--r--   0        0        0    11369 2022-01-10 15:31:20.862876 pydantic_sqlite-0.2.1/pydantic_sqlite/_core.py
--rw-r--r--   0        0        0     1022 2022-01-10 15:31:20.862876 pydantic_sqlite-0.2.1/pydantic_sqlite/_handler.py
--rw-r--r--   0        0        0      351 2022-01-10 15:31:20.862876 pydantic_sqlite-0.2.1/pydantic_sqlite/_misc.py
--rw-r--r--   0        0        0      748 2022-01-10 15:31:20.862876 pydantic_sqlite-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7005 2022-01-10 15:31:33.099488 pydantic_sqlite-0.2.1/setup.py
--rw-r--r--   0        0        0     6801 2022-01-10 15:31:33.100047 pydantic_sqlite-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-05 21:31:02.227397 pydantic_sqlite-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5980 2024-04-05 21:31:02.227397 pydantic_sqlite-0.2.2/README.md
+-rw-r--r--   0        0        0      109 2024-04-05 21:31:02.227397 pydantic_sqlite-0.2.2/pydantic_sqlite/__init__.py
+-rw-r--r--   0        0        0    11704 2024-04-05 21:31:02.227397 pydantic_sqlite-0.2.2/pydantic_sqlite/_core.py
+-rw-r--r--   0        0        0     1022 2024-04-05 21:31:02.227397 pydantic_sqlite-0.2.2/pydantic_sqlite/_handler.py
+-rw-r--r--   0        0        0      351 2024-04-05 21:31:02.227397 pydantic_sqlite-0.2.2/pydantic_sqlite/_misc.py
+-rw-r--r--   0        0        0      691 2024-04-05 21:31:02.227397 pydantic_sqlite-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6810 1970-01-01 00:00:00.000000 pydantic_sqlite-0.2.2/PKG-INFO
```

### Comparing `pydantic_sqlite-0.2.1/LICENSE` & `pydantic_sqlite-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_sqlite-0.2.1/README.md` & `pydantic_sqlite-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_sqlite-0.2.1/pydantic_sqlite/_core.py` & `pydantic_sqlite-0.2.2/pydantic_sqlite/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import inspect
 import json
 import os
 import sqlite3
 import tempfile
 import typing
 from shutil import copyfile
-from typing import Any, Generator, List, Union
+from typing import Any, Generator, List, Literal, Union, get_origin
 
 from pydantic import BaseModel, root_validator
 from pydantic.fields import ModelField
 from sqlite_utils import Database as _Database
-from typing_inspect import is_literal_type, is_union_type
 
 from ._misc import iterable_in_type_repr
 
 SPECIALTYPE = [
-    typing.Any, 
+    typing.Any,
     typing.Literal,
     typing.Union]
 
+
 class TableBaseModel(BaseModel):
     table: str
     moduleclass: typing.Any
     modulename: str
     pks: List[str]
 
     @root_validator(pre=True)
@@ -76,55 +76,69 @@
                 raise ValueError(f"not all values in the List are from the same type: '{field_value}'")
             return [obj_class.SQConfig.convert(value) for value in field_value]
         else:
             if not special_possible(obj_class := field_value.__class__):
                 return False
             return obj_class.SQConfig.convert(field_value)
 
-    def add(self, tablename: str, value: BaseModel, foreign_tables={}, update_nested_models=True, pk: str = "uuid") -> None:
+    def add(
+            self,
+            tablename: str,
+            value: BaseModel,
+            foreign_tables={},
+            update_nested_models=True,
+            pk: str = "uuid") -> None:
         """adds a new value to the table tablename"""
 
         # unkown Tablename -> means new Table -> update the table_basemodel_ref list
         if tablename not in self._basemodels:
             self._basemodels_add_model(table=tablename, moduleclass=value.__class__, pks=[pk])
 
         # check whether the value matches the basemodels in the table
         if not self._basemodels[tablename].moduleclass == type(value):
-            raise ValueError(
-                f"Can not add type '{type(value)}' to the table '{tablename}', which contains values of type '{self._basemodels[tablename].moduleclass}'")
+            msg = f"Can not add type '{type(value)}' to the table '{tablename}',"
+            msg += f" which contains values of type '{self._basemodels[tablename].moduleclass}'"
+            raise ValueError(msg)
 
         # create dict for writing to the Table
         data_for_save = value.dict() if not hasattr(value, "sqlite_repr") else value.sqlite_repr
         foreign_keys = []
         for field_name, field in value.__fields__.items():
             field_value = getattr(value, field_name)
 
             if res := self._special_conversion(field_value):  # Special Insert with SQConfig.convert
                 data_for_save[field_name] = res
 
-            elif field.type_ in SPECIALTYPE or typing.get_origin(field.type_):  
+            elif field.type_ in SPECIALTYPE or typing.get_origin(field.type_):
                 # typing._SpecialForm: Any, NoReturn, ClassVar, Union, Optional
                 # typing.get_origin(field.type_) -> e.g. Literal
                 data_for_save[field_name] = self._typing_conversion(field, field_value)
 
             elif issubclass(field.type_, BaseModel):  # nested BaseModels in this value
                 # the value has got a field which is of type BaseModel, so this filed must be in a foreign table
-                # if the field is already in the Table it continues, but if is it not in the table it will add this to the table
-                # !recursive call to self.add
+                # if the field is already in the Table it continues, but if is it not in the table it will add this
+                # to the table recursive call to self.add
 
                 if field_name not in foreign_tables.keys():
                     keys = list(foreign_tables.keys())
-                    raise KeyError(f"detect field of Type BaseModel, but can not find '{field_name}' in foreign_tables (Keys: {keys})") from None
+                    msg = f"detect field of Type BaseModel, but can not find '{field_name}'"
+                    msg += f"in foreign_tables (Keys: {keys})"
+                    raise KeyError(msg) from None
                 else:
                     foreign_table_name = foreign_tables[field_name]
 
                 if foreign_table_name not in self._db.table_names():
-                    raise KeyError(f"Can not add a value, which has a foreign Key '{foreign_tables}' to a Table '{foreign_table_name}' which does not exists")
-
-                nested_obj_ids = self._upsert_value_in_foreign_table(field_value, foreign_table_name, update_nested_models)
+                    msg = f"Can not add a value, which has a foreign Key '{foreign_tables}'"
+                    msg += f" to a Table '{foreign_table_name}' which does not exists"
+                    raise KeyError(msg)
+
+                nested_obj_ids = self._upsert_value_in_foreign_table(
+                    field_value,
+                    foreign_table_name,
+                    update_nested_models)
                 data_for_save[field_name] = nested_obj_ids
                 foreign_keys.append((field_name, foreign_table_name, pk))  # ignore=True
 
         self._db[tablename].upsert(data_for_save, pk=pk, foreign_keys=foreign_keys)
 
     def uuid_in_table(self, tablename: str, uuid: str) -> bool:
         """checks if the given uuid is used as a primary key in the table"""
@@ -134,19 +148,22 @@
         return False if not hits else True
 
     def value_in_table(self, tablename: str, value: BaseModel) -> bool:
         """checks if the given value is in the table"""
         return self.uuid_in_table(tablename, value.uuid)
 
     def value_from_table(self, tablename: str, uuid: str) -> typing.Any:
-        """searchs the Objekt with the given uuid in the table and returns it. Returns a subclass of type pydantic.BaseModel"""
+        """
+        searchs the Objekt with the given uuid in the table and returns it.
+        Returns a subclass of type pydantic.BaseModel
+        """
         hits = [row for row in self._db[tablename].rows_where("uuid = ?", [uuid])]
         if len(hits) > 1:
             raise Exception("uuid is two times in table")  # TODO choice correct exceptiontype
- 
+
         model = self._basemodels[tablename]
         foreign_refs = {key.column: key.other_table for key in self._db[tablename].foreign_keys}
         return None if not hits else self._build_basemodel_from_dict(model, hits[0], foreign_refs=foreign_refs)
 
     def values_in_table(self, tablename) -> int:
         """returns the number of values in the Table"""
         return self._db[tablename].count
@@ -192,37 +209,42 @@
 
     def _basemodels_add_model(self, **kwargs):
         model = TableBaseModel(**kwargs)
         self._basemodels.update({kwargs['table']: model})
         self._db["__basemodels__"].upsert(model.data(), pk="modulename")
 
     def _build_basemodel_from_dict(self, basemodel: TableBaseModel, row: dict, foreign_refs: dict):
-        # returns a subclass object of type BaseModel which is build out of class basemodel.moduleclass and the data out of the dict
+        # returns a subclass object of type BaseModel which is build out of
+        # class basemodel.moduleclass and the data out of the dict
 
-        members = inspect.getmembers(basemodel.moduleclass, lambda a: not(inspect.isroutine(a)))
+        members = inspect.getmembers(basemodel.moduleclass, lambda a: not inspect.isroutine(a))
         field_models = next(line[1] for line in members if '__fields__' in line)
 
         d = {}
         for field_name, field_value in row.items():
             type_repr = field_models[field_name].__str__().split(' ')[1]  # 'type=Any'
 
             if field_name in foreign_refs.keys():  # the column contains another subclass of BaseModel
                 if not iterable_in_type_repr(type_repr):
                     data = self.value_from_table(foreign_refs[field_name], field_value)
                 else:
                     data = [self.value_from_table(foreign_refs[field_name], val) for val in json.loads(field_value)]
-            else:  
+            else:
                 data = field_value if not iterable_in_type_repr(type_repr) else json.loads(field_value)
             d.update({field_name: data})
 
         return basemodel.moduleclass(**d)
 
-    def _upsert_value_in_foreign_table(self, field_value, foreign_table_name, update_nested_models) -> Union[str, List[str]]:
+    def _upsert_value_in_foreign_table(
+            self,
+            field_value,
+            foreign_table_name,
+            update_nested_models) -> Union[str, List[str]]:
         # The nested BaseModel will be inserted or upserted to the foreign table if it is not contained there,
-        # or the update_nested_models parameter is True. If the value is Iterable (e.g. List) all values in the 
+        # or the update_nested_models parameter is True. If the value is Iterable (e.g. List) all values in the
         # List will be be inserted or upserted. The function returns the ids of the values
 
         # The foreign keys of this table are needed to add the nested basemodel object.
         foreign_refs = {key.column: key.other_table for key in self._db.table(foreign_table_name).foreign_keys}
 
         def add_nested_model(value):
             if not self.value_in_table(foreign_table_name, value) or update_nested_models:
@@ -233,13 +255,13 @@
             return add_nested_model(field_value)
         else:
             return [add_nested_model(element) for element in field_value]
 
     def _typing_conversion(self, field: ModelField, field_value: typing) -> typing.Any:
         if field.type_ == typing.Any:
             return field_value
-        elif is_union_type(field.type_):
+        elif get_origin(field.type_) is Union:
             return str(field_value)
-        elif is_literal_type(field.type_):
+        elif get_origin(field.type_) is Literal:
             return str(field_value)
         else:
             raise NotImplementedError(f"type {field.type_} is not supported yet")
```

### Comparing `pydantic_sqlite-0.2.1/pydantic_sqlite/_handler.py` & `pydantic_sqlite-0.2.2/pydantic_sqlite/_handler.py`

 * *Files identical despite different names*

### Comparing `pydantic_sqlite-0.2.1/setup.py` & `pydantic_sqlite-0.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,190 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['pydantic_sqlite']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pydantic>=1.8.2,<2.0.0',
- 'sqlite-utils>=3.19,<4.0',
- 'typing-inspect>=0.7.1,<0.8.0']
-
-setup_kwargs = {
-    'name': 'pydantic-sqlite',
-    'version': '0.2.1',
-    'description': 'Simple package for storing pydantic BaseModels in an in-memory SQLite database.',
-    'long_description': '# pydantic_sqlite\nSimple package for storing pydantic BaseModels in an in-memory SQLite database.\n\n## Installation\n\n    pip install pydantic-sqlite\n\n## Basic Example\nCreate two objects of the type TestCase and add them to the database in the table \'Test\'. Later, all values in the table are printed while iteration over the Table \'Test\'.\n\n``` python\nfrom pydantic_sqlite import DataBase\nfrom pydantic import BaseModel\nfrom uuid import uuid4\n\nclass TestCase(BaseModel):\n    uuid: str\n    name: str \n    age: int\n        \ntest1 = TestCase(uuid=str(uuid4()), name="Bob", age=12)\ntest2 = TestCase(uuid=str(uuid4()), name="Alice", age=28)\n\ndb = DataBase()\ndb.add("Test", test1)\ndb.add("Test", test2)\n\nfor x in db("Test"):\n    assert issubclass(x.__class__, BaseModel)\n    assert isinstance(x, TestCase)\n    print(x)\n\n#>>> uuid=\'10d002bc-9941-4943-a46b-82b8214bf618\' name=\'Bob\' age=12\n#>>> uuid=\'595fd605-4684-4f78-96a5-8420bdb3fc0f\' name=\'Alice\' age=28\n\n```\n\n## Nested Example\nCreate one object of the type address and two objects of the type person. Each person has an attribute of the type address. \nWhen adding the person to the database, the database needs the foreign_table \'Adresses\' to create the foreign key. This means that when iterating over the table \'Persons\', a complete object "Person" can be created again, which has an attribute of the type \'Address\'.\n\n\n```python\nfrom pydantic_sqlite import DataBase\nfrom pydantic import BaseModel\nfrom uuid import uuid4\n\nclass Address(BaseModel):\n    uuid: str\n    town: str\n    street: str\n    number: int\n        \nclass Person(BaseModel):\n    uuid: str\n    name: str \n    address: Address\n\naddress = Address(uuid=str(uuid4()), town="Berlin", street="Bahnhofstraße", number=67)\nperson1 = Person(uuid=str(uuid4()), name="Bob", address=address)\nperson2 = Person(uuid=str(uuid4()), name="Alice", address=address)\n\ndb = DataBase()\ndb.add("Adresses", address)\ndb.add("Persons", person1, foreign_tables={\'address\': \'Adresses\'})\ndb.add("Persons", person2, foreign_tables={\'address\': \'Adresses\'})\n\nfor x in db("Adresses"):\n    assert issubclass(x.__class__, BaseModel)\n    assert isinstance(x, Address)\n    print(x)\n\nfor y in db("Persons"):\n    assert issubclass(y.__class__, BaseModel)\n    assert isinstance(y, Person)\n    print(y)\n\n#>>> uuid=\'7cd5410e-cfaa-481e-a201-ad04cd959719\' town=\'Berlin\' street=\'Bahnhofstraße\' number=67\n#>>> uuid=\'cc1cedaf-dac5-4fc2-a11a-41c6631271a5\' name=\'Bob\' address=Address(uuid=\'7cd5410e-cfaa-481e-a201-ad04cd959719\', town=\'Berlin\', street=\'Bahnhofstraße\', number=67)\n#>>> uuid=\'b144ed22-d8a4-46da-8a18-e34c260d7c45\' name=\'Alice\' address=Address(uuid=\'7cd5410e-cfaa-481e-a201-ad04cd959719\', town=\'Berlin\', street=\'Bahnhofstraße\', number=67)\n\n```\n\n# Nested Example without foreign Table\nIf you do not want to have an additional table, you can save an object of the BaseModel type differently.\n\nIn this example, the address object is not saved as an additional table. It is stored as a string in a column of the table \'Persons\'. To realise this, the class `SQConfig` is added to the Address class. This class must contain the method `convert`, which determines how the object is to be stored in SQLite. During the subsequent loading, an object of the type Address is created again from the string with the function pydantic.validator.\n\n```python\nfrom pydantic_sqlite import DataBase\nfrom pydantic import BaseModel, validator\nfrom uuid import uuid4\n\nclass Address(BaseModel):\n    town: str\n    street: str\n        \n    class SQConfig:\n        special_insert: bool = True\n\n        def convert(obj):\n            return f"{obj.town},{obj.street}"\n\nclass Person(BaseModel):\n    uuid: str\n    name: str \n    address: Address\n        \n    @validator(\'address\', pre=True)\n    def validate(cls, v):\n        if isinstance(v, Address):\n            return v\n        town, street = v.split(\',\')\n        return Address(town=town, street=street)\n\naddress = Address(town="Berlin", street="Bahnhofstraße 67")\nperson1 = Person(uuid=str(uuid4()), name="Bob", address=address)\nperson2 = Person(uuid=str(uuid4()), name="Alice", address=address)\n\ndb = DataBase()\ndb.add("Persons", person1)\ndb.add("Persons", person2)\n\nfor y in db("Persons"):\n    assert issubclass(y.__class__, BaseModel)\n    assert isinstance(y, Person)\n    print(y)\n\n#>>> uuid=\'802f50d6-b6a2-47f4-bb96-4375790daed9\' name=\'Bob\' address=Address(town=\'Berlin\', street=\'Bahnhofstraße 67\')\n#>>> uuid=\'79488c0d-44c8-4a6a-afa3-1ed0b88af4a2\' name=\'Alice\' address=Address(town=\'Berlin\', street=\'Bahnhofstraße 67\')\n```\n\n# DB_Handler\nThe DB_handler provides a wrapper for the DataBase. The database returned by the context manager can be used in the same way as in the previous examples. \n\nHowever, the handler has the advantage that if an exception occurs, e.g. a \'ZeroDevisionError\', a database with the last values is saved as \'<<dbname_crash>>.db\'. If this file already exists, the file name is incremented.\n\nThis example creates two files hello.db and hello_crash.db If you run this script twice, three files are created: hello.db, hello_crash.db and hello_crash_(1).db\n```python\nfrom pydantic_sqlite import DataBase, DB_Handler\nfrom pydantic import BaseModel, validator\nfrom uuid import uuid4\n\nclass TestCase(BaseModel):\n    uuid: str\n    name: str \n    age: int\n\nwith DB_Handler("hello") as db:\n    test1 = TestCase(uuid=str(uuid4()), name="Bob", age=12)\n    db.add("Test", test1)\n    for x in db("Test"):\n        assert issubclass(x.__class__, BaseModel)\n        assert isinstance(x, TestCase)\n        print(x)\n    db.save("hello_world.db")\n    \n    1/0\n\n#>>> uuid=\'04d6dfad-0ce5-4222-8686-22348e1f0c0b\' name=\'Bob\' age=12\n#>>> ---------------------------------------------------------------------------\n#>>> ZeroDivisionError    Traceback (most recent call last)\n#>>> ~\\AppData\\Local\\Temp/ipykernel_20124/1430346317.py in <module>\n#>>>      17     db.save("hello_world.db")\n#>>>      18 \n#>>> ---> 19     1/0\n#>>> \n#>>> ZeroDivisionError: division by zero\n```',
-    'author': 'Your Name',
-    'author_email': 'you@example.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/Phil997/pydantic-sqlite',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: pydantic_sqlite
+Version: 0.2.2
+Summary: Simple package for storing pydantic BaseModels in an in-memory SQLite database.
+Home-page: https://github.com/Phil997/pydantic-sqlite
+License: MIT
+Keywords: pydantic,sqlite-utils,sqlite3
+Author: Your Name
+Author-email: you@example.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: sqlite-utils (>=3.19,<4.0)
+Project-URL: Repository, https://github.com/Phil997/pydantic-sqlite
+Description-Content-Type: text/markdown
+
+# pydantic_sqlite
+Simple package for storing pydantic BaseModels in an in-memory SQLite database.
+
+## Installation
+
+    pip install pydantic-sqlite
+
+## Basic Example
+Create two objects of the type TestCase and add them to the database in the table 'Test'. Later, all values in the table are printed while iteration over the Table 'Test'.
+
+``` python
+from pydantic_sqlite import DataBase
+from pydantic import BaseModel
+from uuid import uuid4
+
+class TestCase(BaseModel):
+    uuid: str
+    name: str 
+    age: int
+        
+test1 = TestCase(uuid=str(uuid4()), name="Bob", age=12)
+test2 = TestCase(uuid=str(uuid4()), name="Alice", age=28)
+
+db = DataBase()
+db.add("Test", test1)
+db.add("Test", test2)
+
+for x in db("Test"):
+    assert issubclass(x.__class__, BaseModel)
+    assert isinstance(x, TestCase)
+    print(x)
+
+#>>> uuid='10d002bc-9941-4943-a46b-82b8214bf618' name='Bob' age=12
+#>>> uuid='595fd605-4684-4f78-96a5-8420bdb3fc0f' name='Alice' age=28
+
+```
+
+## Nested Example
+Create one object of the type address and two objects of the type person. Each person has an attribute of the type address. 
+When adding the person to the database, the database needs the foreign_table 'Adresses' to create the foreign key. This means that when iterating over the table 'Persons', a complete object "Person" can be created again, which has an attribute of the type 'Address'.
+
+
+```python
+from pydantic_sqlite import DataBase
+from pydantic import BaseModel
+from uuid import uuid4
+
+class Address(BaseModel):
+    uuid: str
+    town: str
+    street: str
+    number: int
+        
+class Person(BaseModel):
+    uuid: str
+    name: str 
+    address: Address
+
+address = Address(uuid=str(uuid4()), town="Berlin", street="Bahnhofstraße", number=67)
+person1 = Person(uuid=str(uuid4()), name="Bob", address=address)
+person2 = Person(uuid=str(uuid4()), name="Alice", address=address)
+
+db = DataBase()
+db.add("Adresses", address)
+db.add("Persons", person1, foreign_tables={'address': 'Adresses'})
+db.add("Persons", person2, foreign_tables={'address': 'Adresses'})
+
+for x in db("Adresses"):
+    assert issubclass(x.__class__, BaseModel)
+    assert isinstance(x, Address)
+    print(x)
+
+for y in db("Persons"):
+    assert issubclass(y.__class__, BaseModel)
+    assert isinstance(y, Person)
+    print(y)
+
+#>>> uuid='7cd5410e-cfaa-481e-a201-ad04cd959719' town='Berlin' street='Bahnhofstraße' number=67
+#>>> uuid='cc1cedaf-dac5-4fc2-a11a-41c6631271a5' name='Bob' address=Address(uuid='7cd5410e-cfaa-481e-a201-ad04cd959719', town='Berlin', street='Bahnhofstraße', number=67)
+#>>> uuid='b144ed22-d8a4-46da-8a18-e34c260d7c45' name='Alice' address=Address(uuid='7cd5410e-cfaa-481e-a201-ad04cd959719', town='Berlin', street='Bahnhofstraße', number=67)
+
+```
+
+# Nested Example without foreign Table
+If you do not want to have an additional table, you can save an object of the BaseModel type differently.
+
+In this example, the address object is not saved as an additional table. It is stored as a string in a column of the table 'Persons'. To realise this, the class `SQConfig` is added to the Address class. This class must contain the method `convert`, which determines how the object is to be stored in SQLite. During the subsequent loading, an object of the type Address is created again from the string with the function pydantic.validator.
+
+```python
+from pydantic_sqlite import DataBase
+from pydantic import BaseModel, validator
+from uuid import uuid4
+
+class Address(BaseModel):
+    town: str
+    street: str
+        
+    class SQConfig:
+        special_insert: bool = True
+
+        def convert(obj):
+            return f"{obj.town},{obj.street}"
+
+class Person(BaseModel):
+    uuid: str
+    name: str 
+    address: Address
+        
+    @validator('address', pre=True)
+    def validate(cls, v):
+        if isinstance(v, Address):
+            return v
+        town, street = v.split(',')
+        return Address(town=town, street=street)
+
+address = Address(town="Berlin", street="Bahnhofstraße 67")
+person1 = Person(uuid=str(uuid4()), name="Bob", address=address)
+person2 = Person(uuid=str(uuid4()), name="Alice", address=address)
+
+db = DataBase()
+db.add("Persons", person1)
+db.add("Persons", person2)
+
+for y in db("Persons"):
+    assert issubclass(y.__class__, BaseModel)
+    assert isinstance(y, Person)
+    print(y)
+
+#>>> uuid='802f50d6-b6a2-47f4-bb96-4375790daed9' name='Bob' address=Address(town='Berlin', street='Bahnhofstraße 67')
+#>>> uuid='79488c0d-44c8-4a6a-afa3-1ed0b88af4a2' name='Alice' address=Address(town='Berlin', street='Bahnhofstraße 67')
+```
+
+# DB_Handler
+The DB_handler provides a wrapper for the DataBase. The database returned by the context manager can be used in the same way as in the previous examples. 
+
+However, the handler has the advantage that if an exception occurs, e.g. a 'ZeroDevisionError', a database with the last values is saved as '<<dbname_crash>>.db'. If this file already exists, the file name is incremented.
+
+This example creates two files hello.db and hello_crash.db If you run this script twice, three files are created: hello.db, hello_crash.db and hello_crash_(1).db
+```python
+from pydantic_sqlite import DataBase, DB_Handler
+from pydantic import BaseModel, validator
+from uuid import uuid4
+
+class TestCase(BaseModel):
+    uuid: str
+    name: str 
+    age: int
+
+with DB_Handler("hello") as db:
+    test1 = TestCase(uuid=str(uuid4()), name="Bob", age=12)
+    db.add("Test", test1)
+    for x in db("Test"):
+        assert issubclass(x.__class__, BaseModel)
+        assert isinstance(x, TestCase)
+        print(x)
+    db.save("hello_world.db")
+    
+    1/0
+
+#>>> uuid='04d6dfad-0ce5-4222-8686-22348e1f0c0b' name='Bob' age=12
+#>>> ---------------------------------------------------------------------------
+#>>> ZeroDivisionError    Traceback (most recent call last)
+#>>> ~\AppData\Local\Temp/ipykernel_20124/1430346317.py in <module>
+#>>>      17     db.save("hello_world.db")
+#>>>      18 
+#>>> ---> 19     1/0
+#>>> 
+#>>> ZeroDivisionError: division by zero
+```
```

