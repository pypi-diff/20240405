# Comparing `tmp/openagi-0.1.0b2.tar.gz` & `tmp/openagi-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagi-0.1.0b2.tar", max compression
+gzip compressed data, was "openagi-0.1.0b3.tar", max compression
```

## Comparing `openagi-0.1.0b2.tar` & `openagi-0.1.0b3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     5813 2024-04-03 18:00:39.287788 openagi-0.1.0b2/README.md
--rw-r--r--   0        0        0     1053 2024-04-03 18:18:12.076852 openagi-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1499 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/Readme.md
--rw-r--r--   0        0        0      668 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/openagi/__init__.py
--rw-r--r--   0        0        0    14265 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/openagi/agent.py
--rw-r--r--   0        0        0     3745 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/openagi/init_agent.py
--rw-r--r--   0        0        0      196 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/openagi/llms/__init__.py
--rw-r--r--   0        0        0     2720 2024-04-03 18:00:39.342787 openagi-0.1.0b2/src/openagi/llms/azure.py
--rw-r--r--   0        0        0     1351 2024-04-03 18:00:39.342787 openagi-0.1.0b2/src/openagi/llms/base.py
--rw-r--r--   0        0        0      713 2024-04-03 18:00:39.342787 openagi-0.1.0b2/src/openagi/llms/openagi_main.py
--rw-r--r--   0        0        0     1619 2024-04-03 18:00:39.342787 openagi-0.1.0b2/src/openagi/llms/openai.py
--rw-r--r--   0        0        0     3782 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/queue/message_broker.py
--rw-r--r--   0        0        0     2750 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/queue/pq.py
--rw-r--r--   0        0        0     6433 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/queue/timer_pool.py
--rw-r--r--   0        0        0       28 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/tools/__init__.py
--rw-r--r--   0        0        0     1979 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/tools/base.py
--rw-r--r--   0        0        0      762 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/custom_tools/ProxyTool.py
--rw-r--r--   0        0        0      212 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/custom_tools/custom_tool_db.py
--rw-r--r--   0        0        0     1292 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/integrations/__init__.py
--rw-r--r--   0        0        0      581 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/integrations/dalle_image_generator.py
--rw-r--r--   0        0        0     2753 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/integrations/document_compare.py
--rw-r--r--   0        0        0     1047 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/integrations/duckducksearch.py
--rw-r--r--   0        0        0     1527 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/exa_search_tool.py
--rw-r--r--   0        0        0     1745 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/github.py
--rw-r--r--   0        0        0     1595 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/gmail.py
--rw-r--r--   0        0        0      270 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/google.py
--rw-r--r--   0        0        0     1433 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/google_finance_search.py
--rw-r--r--   0        0        0     1357 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/google_serper_specific.py
--rw-r--r--   0        0        0     1160 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/googlejobsearch.py
--rw-r--r--   0        0        0      841 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/googleserpersearch.py
--rw-r--r--   0        0        0     1350 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/nasa.py
--rw-r--r--   0        0        0      844 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/open_weathermap.py
--rw-r--r--   0        0        0     1743 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/polygon.py
--rw-r--r--   0        0        0     1444 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/serper_intermediate.py
--rw-r--r--   0        0        0     1357 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/sql.py
--rw-r--r--   0        0        0     1141 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/wikipedia_tool.py
--rw-r--r--   0        0        0     1256 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/xorbits.py
--rw-r--r--   0        0        0     1315 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/yahoofinancenews.py
--rw-r--r--   0        0        0      945 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/youtubesearch.py
--rw-r--r--   0        0        0     3198 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/tools/tools_db.py
--rw-r--r--   0        0        0     2474 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/tools/utils.py
--rw-r--r--   0        0        0      593 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/utils/extraction.py
--rw-r--r--   0        0        0    13792 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/utils/llmTasks.py
--rw-r--r--   0        0        0      730 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/utils/yamlParse.py
--rw-r--r--   0        0        0     7199 1970-01-01 00:00:00.000000 openagi-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     4094 2024-04-05 05:20:15.733992 openagi-0.1.0b3/README.md
+-rw-r--r--   0        0        0     1053 2024-04-05 05:21:37.778721 openagi-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1499 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/Readme.md
+-rw-r--r--   0        0        0      667 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/__init__.py
+-rw-r--r--   0        0        0    14360 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/agent.py
+-rw-r--r--   0        0        0     3398 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/init_agent.py
+-rw-r--r--   0        0        0      196 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/__init__.py
+-rw-r--r--   0        0        0     2720 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/azure.py
+-rw-r--r--   0        0        0     1351 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/base.py
+-rw-r--r--   0        0        0      713 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/openagi_main.py
+-rw-r--r--   0        0        0     1619 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/llms/openai.py
+-rw-r--r--   0        0        0     3782 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/queue/message_broker.py
+-rw-r--r--   0        0        0     2750 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/queue/pq.py
+-rw-r--r--   0        0        0     6433 2024-04-05 05:20:15.764992 openagi-0.1.0b3/src/openagi/queue/timer_pool.py
+-rw-r--r--   0        0        0       28 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/__init__.py
+-rw-r--r--   0        0        0     1979 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/base.py
+-rw-r--r--   0        0        0      762 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/custom_tools/ProxyTool.py
+-rw-r--r--   0        0        0      212 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/custom_tools/custom_tool_db.py
+-rw-r--r--   0        0        0     1292 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/__init__.py
+-rw-r--r--   0        0        0      581 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/dalle_image_generator.py
+-rw-r--r--   0        0        0     2753 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/document_compare.py
+-rw-r--r--   0        0        0     1047 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/duckducksearch.py
+-rw-r--r--   0        0        0     1527 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/exa_search_tool.py
+-rw-r--r--   0        0        0     1745 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/github.py
+-rw-r--r--   0        0        0     1595 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/gmail.py
+-rw-r--r--   0        0        0      270 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/google.py
+-rw-r--r--   0        0        0     1433 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/google_finance_search.py
+-rw-r--r--   0        0        0     1357 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/google_serper_specific.py
+-rw-r--r--   0        0        0     1160 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/googlejobsearch.py
+-rw-r--r--   0        0        0      841 2024-04-05 05:20:15.765992 openagi-0.1.0b3/src/openagi/tools/integrations/googleserpersearch.py
+-rw-r--r--   0        0        0     1350 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/nasa.py
+-rw-r--r--   0        0        0      844 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/open_weathermap.py
+-rw-r--r--   0        0        0     1743 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/polygon.py
+-rw-r--r--   0        0        0     1444 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/serper_intermediate.py
+-rw-r--r--   0        0        0     1357 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/sql.py
+-rw-r--r--   0        0        0     1141 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/wikipedia_tool.py
+-rw-r--r--   0        0        0     1256 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/xorbits.py
+-rw-r--r--   0        0        0     1315 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/yahoofinancenews.py
+-rw-r--r--   0        0        0      945 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/integrations/youtubesearch.py
+-rw-r--r--   0        0        0     3198 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/tools_db.py
+-rw-r--r--   0        0        0     3255 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/tools/utils.py
+-rw-r--r--   0        0        0      593 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/utils/extraction.py
+-rw-r--r--   0        0        0    13792 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/utils/llmTasks.py
+-rw-r--r--   0        0        0      730 2024-04-05 05:20:15.766991 openagi-0.1.0b3/src/openagi/utils/yamlParse.py
+-rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 openagi-0.1.0b3/PKG-INFO
```

### Comparing `openagi-0.1.0b2/pyproject.toml` & `openagi-0.1.0b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openagi"
-version = "0.1.0-b2"
+version = "0.1.0-b3"
 description = ""
 authors = ["AI Planet <tech@aiplanet.com>"]
 readme = "README.md"
 include = ["src/*"]
 
 [tool.poetry.dependencies]
 python = "~3.11"
```

### Comparing `openagi-0.1.0b2/src/Readme.md` & `openagi-0.1.0b3/src/Readme.md`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/__init__.py` & `openagi-0.1.0b3/src/openagi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from datetime import datetime
 from pathlib import Path
 
 BASE_PATH = "logs"
 pth = Path(BASE_PATH)
 pth.mkdir(parents=True, exist_ok=True)
-filename = (f'{pth.absolute()}/application_{datetime.now().strftime("%Y-%m-%d_%H-%M-%S")}.log',)
+filename = (f'{pth.absolute()}/application_{datetime.now().strftime("%Y-%m-%d_%H-%M-%S")}.log')
 
 # Setup basic logging configuration
 logging.basicConfig(
     level=logging.DEBUG,
     format="%(asctime)s %(levelname)s::%(thread)d::%(pathname)s:%(lineno)d:%(funcName)s:%(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     filename=f'{pth.absolute()}/application_{datetime.now().strftime("%Y-%m-%d_%H-%M-%S")}.log',
```

### Comparing `openagi-0.1.0b2/src/openagi/agent.py` & `openagi-0.1.0b3/src/openagi/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,529 +1,374 @@
 import logging
 import threading
 import time
 from concurrent.futures import ThreadPoolExecutor
-
 import spacy
 from spacytextblob.spacytextblob import SpacyTextBlob
-
 from openagi.llms.base import LLMBaseModel
 from openagi.queue.message_broker import NameIndexMapper
 from openagi.queue.pq import Message, MessageType, MultiThreadPriorityQueue
 from openagi.tools.integrations.duckducksearch import getDuckduckgoSearchResults
 from openagi.tools.tools_db import (
     TOOLS_DICT_MAPPING,
 )
-from openagi.tools.utils import search_string_in_list
+from openagi.tools.utils import search_string_in_list, isLastHGI
 from openagi.utils.llmTasks import handleLLMTask, tools_handler
 
 g_mapper = None
 g_timerlist = None
 main_condition = threading.Condition()
 
-
 def createDynamicAgent(agent, *functions):
     for startAgent, mapper in functions:
         startAgent(agent, mapper)
 
-
 def setGMapper(mapper):
     global g_mapper
     g_mapper = mapper
     logging.debug(f"mapper object = {g_mapper.__dict__}")
 
-
 def getGMapper():
     logging.debug(f"mapper object from get = {g_mapper.__dict__}")
     return g_mapper
 
-
 def setGTimerList(timerPool):
     global g_timerlist
     g_timerlist = timerPool
 
-
 def getGTimerList(timerPool):
     return g_timerlist
 
-
 def waitonConditionAgent(mapper, agentName, duration):
     lindex = mapper.get_index_by_name(agentName)
     logging.debug(f"index of {agentName} is {lindex}")
     cond = mapper.COND_LIST[lindex]
     cond.acquire()
     cond.wait(timeout=duration)
     cond.release()
 
-
 def wakeUpAgent(mapper, agentName):
     lindex = mapper.get_index_by_name(agentName)
     cond = mapper.COND_LIST[lindex]
     cond.acquire()
     cond.notify()
     cond.release()
 
-
 def waitonConditionMain(condition, duration):
     condition.acquire()
     condition.wait(timeout=duration)
     condition.release()
 
-
 def wakeupMainForKill(condition):
     condition.acquire()
-
     condition.notify()
-
     condition.release()
 
-
 def exitOpenAGI():
     wakeupMainForKill(main_condition)
 
-
-def createAndsendMessage(srcAgent, dstAgent, body, mapper):
-    priority = 0
-
-    perception_type = 0
-
-    message_type = MessageType.AGENT_MSG
-
-    body = body
-
-    message = Message(priority, perception_type, message_type, srcAgent, dstAgent, body)
-
-    pq = mapper.get_PQ_by_name(dstAgent)
-
-    time.sleep(10)
-
-    pq.insert(message)
-
-    wakeUpAgent(mapper, dstAgent)
-
+def createAndsendMessage(srcAgent, dstAgent, body, mapper, consumerList):
+    for dstAgent in consumerList:
+        priority = 0
+        perception_type = 0
+        message_type = MessageType.AGENT_MSG
+        body = body
+        message = Message(priority, perception_type, message_type, srcAgent, dstAgent, body)
+        pq = mapper.get_PQ_by_name(dstAgent)
+        pq.insert(message)
+        wakeUpAgent(mapper, dstAgent)
 
 def createAndsendMessageProfTrigger(srcAgent, dstAgent, body, mapper):
     priority = 0
-
     perception_type = 0
-
     message_type = MessageType.PROF_AGENT_TRIGGER
-
     body = body
-
     message = Message(priority, perception_type, message_type, srcAgent, dstAgent, body)
-
     pq = mapper.get_PQ_by_name(dstAgent)
-
     time.sleep(5)
-
     pq.insert(message)
-
     wakeUpAgent(mapper, dstAgent)
 
 
 def evalLLMResponse(resp):
     print(f"evalLLMResponse::{resp}")
-
     nlp = spacy.load(
         "en_core_web_sm"
     )  # Run this command if you face error: `python -m spacy download en_core_web_sm`
-
     nlp.add_pipe("spacytextblob")
-
     doc = nlp(resp)
-
     polarity = doc._.blob.polarity
-
     print(f"sentiment {polarity}")
-
     if polarity > 0:
         return True
-
     return False
 
 
 def createAndSendFeedbackMessage(srcAgent, dstAgent, body, mapper, feedbackSummary):
     priority = 0
-
     perception_type = 0
-
     message_type = MessageType.FEEDBACK_MSG
-
     final_reponse = "revise" + body + "based on feedback " + body
-
     logging.debug(
         f"the body of feedback messgae...............................{final_reponse}",
     )
-
     message = Message(priority, perception_type, message_type, srcAgent, dstAgent, final_reponse)
-
     if not dstAgent == "profAgent":
         pq = mapper.get_PQ_by_name(dstAgent)
-
         time.sleep(10)
-
         pq.insert(message)
-
         wakeUpAgent(mapper, dstAgent)
         return
-
     else:
         logging.debug(f"response is going to profAgent f{message}")
         return
 
 
 def example_callbackTimer(dstAgent, timerName, timerValue):
     logging.debug(f"Callback executed at {dstAgent}:{timerName}:{timerValue}")
-
     priority = 0
-
     perception_type = 0
-
     message_type = MessageType.TIMER_MSG
-
     body = "This is time out message"
-
     message = Message(priority, perception_type, message_type, "TIMER_AGENT", dstAgent, body)
-
     mapper = getGMapper()
-
     pq = mapper.get_PQ_by_name(dstAgent)
-
     pq.insert(message)
-
     logging.debug(f"timer message is inserted for {dstAgent}  {mapper.__dict__}")
-
     wakeUpAgent(mapper, dstAgent)
 
+def sendMessagetoHGI(consumer, resp):
+    logging.debug(f"final message to {consumer}= {resp}")
+    print(f"final OUTPUT for {consumer} ::{resp}")
+    return isLastHGI()
 
 class Agent:
     def __init__(
         self,
         agentName,
         role,
         goal,
         backstory,
         capability,
         task,
-        output_consumer_agent,
+        output_consumer_agent=[],
         llm_api=None,
         tools_list=[],
         feedback=False,
         agent_type="STATIC",
         multiplicity=0,
         aggregator=0,
         onAggregationAction=None,
         creator=None,
         HGI_Intf=None,
         llm_resp_timer_value=20000,
         llm=None,
     ):
         self.agentName = agentName
         self.aggregator = aggregator
-
         self.onAggregationAction = onAggregationAction
         self.creator = creator
-
         self.createAgentFlag = 0
-
         self.pq = MultiThreadPriorityQueue()
-
         self.condition = threading.Condition()
-
         self.is_data_found = False
-
         self.executor = ThreadPoolExecutor(
             max_workers=2
         )  # Adjust max_workers based on your requirement
-
         self.agent_thread = []
-
         self.mapper = []
-
         self.execute_task = "perform the task"
-
-        self.consumerAgent = output_consumer_agent
-
+        self.consumerAgent= output_consumer_agent[0]
+        self.consumerAgentList = output_consumer_agent
         self.timerNameLLM = "LLM_TIMER"
-
         self.NoOfFeedbackMsgs = 0
-
         self.MAX_NoOfFeedbackMsgs = 1
         self.role = role
-
         self.feedback = feedback
         self.goal = goal
-
         self.backstory = backstory
-
         self.capability = capability
-
         self.agent_type = agent_type
-
         self.multiplicity = multiplicity
-
         self.task = task
         self.output_consumer_agent = output_consumer_agent
-
         self.HGI_Intf = HGI_Intf
         self.llm_api = llm_api
-
         self.timerValueLLM = llm_resp_timer_value
         self.tools_list = tools_list
-
         self.FeedBackMsgReceived = False
-
         self.llm: LLMBaseModel = llm
 
     def format_input(self, input_data):
         # Implement the logic to format input data
         pass
 
     def format_output(self, output_data):
         # Implement the logic to format output data
         pass
 
     def execute(self, messageList):
         # Implement the logic for the execution of the task
-
         message = messageList[0]
-
         if self.aggregator > 0:
             # overwrite the body of the first message with aggregated content
-
             message.body = self.onAggregationAction(
-                self.llm, self.output_consumer_agent, None, messageList
+                self.llm, self.consumerAgent, None, messageList
             )
 
         consumer = self.consumerAgent
-
         resp = f"sending mesage from {self.agentName}"
-
         if self.tools_list:
             logging.debug("Using tools")
-
             _tools = []
-
             for user_tool in self.tools_list:
                 tool_name = user_tool.name  # Assuming user_tool has a name attribute
-
                 if tool_name in TOOLS_DICT_MAPPING:
                     # If the tool exists in TOOLS_DICT, append its info
-
                     _tools.append(TOOLS_DICT_MAPPING[tool_name])
-
                 else:
                     # If the tool is not found, append a custom tool dictionary
-
                     _tools.append(
                         {
                             "category": "custom",
                             **user_tool.get_tool_info(),
                         }
                     )
 
             if self.tools_list:
                 print(f"\n      role being performed is { self.role } \n       ")
-
                 resp = tools_handler(
                     tools=_tools,
                     task_input={
                         "role": self.role,
                         "name": self.agentName,
                         "backstory": self.backstory,
                         "task": self.task,
                         "goal": self.goal,
                         "capability": self.capability,
                         "instructions": self.task,  # TODO: To be Removed or fixed as its redundant
                     },
                     llm=self.llm,
                 )
-
                 logging.info(f"resp from tools_handler : {resp}")
 
         elif self.capability == "search_executor":
             indices = search_string_in_list(self.tools_list, "duckduckgo-search")
-
             if indices:
                 results = getDuckduckgoSearchResults(self.goal + self.task)
-
                 print(f"executed duckduck search and results :{results}")
-
                 resp = f" {results}"
-
         elif (
             self.capability == "llm_task_executor"
         ):  # and (self.role=="SUMMARISER" or self.role=="EMAILER" or self.role=="Coder" or self.role=="Reviewer")):
             print(f"\n      role being performed is { self.role } \n       ")
-
             if not self.feedback or self.NoOfFeedbackMsgs < self.MAX_NoOfFeedbackMsgs:
                 resp = handleLLMTask(
                     message.body,
                     self.role,
                     self.backstory,
                     self.goal,
                     self.task,
                     self.llm,
                 )
-
             else:
                 logging.info("response for  final feedback ")
-
                 resp = message.body
-
         logging.debug(f"response of agent {self.agentName} is { resp}")
-
         # STOP THE TIMER
-
         self.mapper.timerStopMapper(agentName=self.agentName, timerName=self.timerNameLLM)
-
         # feedback is supported for only non aggregator agents
-
         if (
             self.feedback
             and self.aggregator == 0
             and self.NoOfFeedbackMsgs < self.MAX_NoOfFeedbackMsgs
         ):
             status = evalLLMResponse(resp)
-
             if not status:
                 self.NoOfFeedbackMsgs += 1
-
                 createAndSendFeedbackMessage(
                     self.agentName, message.srcAgent, message.body, self.mapper, resp
                 )
                 return
-
             else:
                 logging.debug("feedback on message is positive")
-
                 resp = message.body  # update the body with  original of the agent
 
         if self.HGI_Intf:
             logging.debug("...............executing human tool.....................\n")
-
             resp, feedback, actionself = self.HGI_Intf(self.agentName, resp, self.consumerAgent)
-
             logging.debug(f" the response from human tool:: {resp}")
-
+            
         if not consumer or consumer == "HGI":
-            logging.debug(f"final message to {consumer}= {resp}")
-
-            print(f"final OUTPUT for {consumer} ::{resp}")
-
-            logging.debug("before wake for exit..........")
-
-            wakeupMainForKill(main_condition)
+            if sendMessagetoHGI(consumer, resp):
+                logging.debug("before wake for exit..........")
+                wakeupMainForKill(main_condition)
 
         if consumer and consumer != "HGI":
             logging.debug(f"{self.agentName}..to.. {consumer} content:: {resp}")
-
-            createAndsendMessage(self.agentName, consumer, resp, self.mapper)
+            createAndsendMessage(self.agentName, consumer, resp, self.mapper, self.consumerAgentList)
 
     def run(self):
         myname = self.agentName
-
         logging.debug(f"I am agent {myname}")
-
         multiplicity = self.multiplicity
-
         msgList = []
-
         while True:
             message = self.pq.retrieve_first_message()
-
             if message:
                 msgList.append(message)
-
                 logging.debug(f"agent {myname} retrieved message: {message.__dict__}")
-
                 # print(message.__dict__)
-
                 logging.debug("appended received message to list for aggregation")
-
                 if len(msgList) == self.aggregator or self.aggregator == 0:
                     if self.creator and self.createAgentFlag == 0:
                         logging.debug(
-                            f"creating dynamic agent {self.output_consumer_agent} in {self.agentName}",
+                            f"creating dynamic agent {self.consumerAgent} in {self.agentName}",
                         )
-
                         functions_to_execute = [(Agent.start_agent, self.mapper)]
-
                         createDynamicAgent(self.creator, *functions_to_execute)
-
                         self.createAgentFlag = 1
-
                     self.mapper.timerStartMapper(
                         agentName=self.agentName,
                         timerName=self.timerNameLLM,
                         callback=example_callbackTimer,
                         timervalue=self.timerValueLLM,
                     )
-
                     self.execute(msgList)
-
                     msgList = []
-
             else:
                 logging.debug(f"{myname} agent found no messages from PQ .. going to wait.")
-
                 waitonConditionAgent(self.mapper, self.agentName, 100)
 
     def start_agent(self, mapper):
         # Start the agent in a new thread
-
         self.mapper = mapper  # python - call by value or reference????
-
         self.pq = mapper.get_PQ_by_name(self.agentName)
-
         self.condition = mapper.get_COND_by_name(self.agentName)
-
         self.agent_thread = threading.Thread(target=self.run)
-
         self.agent_thread.daemon = True
-
         self.agent_thread.start()
-
         logging.debug(f"Agent: {self.agentName} LLM: {self.llm}")
 
 
 # Example Usage:
 
 if __name__ == "__main__":
     # Example usage:
-
     # Start the agent in a new thread
-
     agent_list = ["RESEARCHER", "WRITER", "EMAILER"]
-
     mapper = NameIndexMapper()
-
     mapper.add_mapping(agent_list[0])
-
     mapper.add_mapping(agent_list[1])
-
     mapper.add_mapping(agent_list[2])
-
     agent1 = Agent(agentName=agent_list[0], consumerAgent=agent_list[1])
-
     agent2 = Agent(agentName=agent_list[1], consumerAgent=agent_list[2])
-
     agent3 = Agent(agentName=agent_list[2], consumerAgent=agent_list[0])
-
     # , role="RESEARCHER", goal="search for latest trends in Carona treatment", capability="INTERNET_SEARCHER", agent_type="STATIC",
-
     #                multiplicity=3, task="search internet for the goal", output_consumer_agent=agent_list[1],
-
     #               llm_api="gpt4", go_d_timer=10000, llm_resp_timer=20, tools_list=["Google", "Bing","DuckduckGo-search" ])
-
     agent1.start_agent(mapper)
-
     agent2.start_agent(mapper)
-
     agent3.start_agent(mapper)
-
     time.sleep(5)  # Simulating data availability after 5 seconds
-
     msg1 = "message for agent RESEARCHER from ENVIRONMENT "
-
     createAndsendMessage("ProfAgent", agent_list[0], msg1, mapper)
```

### Comparing `openagi-0.1.0b2/src/openagi/init_agent.py` & `openagi-0.1.0b3/src/openagi/init_agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,115 +1,73 @@
 import logging
 import sys
 import threading
-
+from openagi.tools.utils import Number_of_HGI, setGHGI
 from openagi.agent import (
     createAndsendMessageProfTrigger,
     getGMapper,
     main_condition,
     setGMapper,
     setGTimerList,
     waitonConditionMain,
 )
 from openagi.llms.base import LLMBaseModel
 from openagi.queue.message_broker import NameIndexMapper
 
-
+g_number_of_HGI = 0
 def verify_llm_attr(agent_object) -> bool:
     if not hasattr(agent_object, "llm"):
         raise ValueError(
             "LLM Attribute not set. Kindly set the llm either in `Agents` objects or in `kickOffAgents`"
         )
-
     llm_obj = agent_object.llm
-
     if not isinstance(llm_obj, LLMBaseModel):
         raise ValueError(
             "Invalid LLM object. It should be an instance of `openagi.llms.base.LLMBaseModel`"
         )
 
     return True
 
 
 def agentThreadsStart(agentObjectList, llm: LLMBaseModel = None):
     mapper = getGMapper()
-
     for obj in agentObjectList:
         if not obj.llm:
             obj.llm = llm
-
         verify_llm_attr(obj)
-
         obj.start_agent(mapper)
 
 
 def agentInitSystem(agent_list):
     logging.debug("kick-off of the program")
-
     mapper = NameIndexMapper()
-
     timerPool = mapper.timerPool
-
     setGTimerList(timerPool)
 
     for agent in agent_list:
         mapper.add_mapping(agent)
-
     setGMapper(mapper)
-
     timer_thread = threading.Thread(target=timerPool.run)
-
     timer_thread.daemon = True
-
     logging.info("timer demon started")
-
     timer_thread.start()
 
 
 def triggerAgent(agent_list, godTimerDuration):
     msg1 = "HGI sending trigger message to start the execution"
 
     mapper = getGMapper()
 
     for agent in agent_list:
         createAndsendMessageProfTrigger("profAgent", agent, msg1, mapper)
 
     waitonConditionMain(main_condition, godTimerDuration)
-
     logging.info("final exit")
-
     sys.exit()
 
-
-def kickOffAgents2(AgentObjects, triggerAgentObjectsList):
-    agent_list = []
-
-    # extract agent names
-
-    for agentObj in AgentObjects:
-        agent_list.append(agentObj.agentName)
-
-    agentInitSystem(agent_list=agent_list)
-
-    print(agent_list)
-
-    agentThreadsStart(agentObjectList=AgentObjects)
-
-    # extract - trigger agent list
-
-    triggerAgentList = []
-
-    for triggerObj in triggerAgentObjectsList:
-        triggerAgentList.append(triggerObj.agentName)
-
-    print(triggerAgentList)
-
-    triggerAgent(triggerAgentList, godTimerDuration=10000)
-
-
 def searchItemInList(DynamicAgentObjectsList, target):
     for item in DynamicAgentObjectsList:
         if item.agentName == target.agentName:
             # print("Found")
             return True
     return False
 
@@ -117,52 +75,38 @@
 def kickOffAgents(
     AgentObjects,
     triggerAgentObjectsList,
     DynamicAgentObjectsList=[],
     llm: LLMBaseModel = None,
 ):
     agent_list = []
-
+    NumberOfHGI = 0
     # extract agent names
-
     for agentObj in AgentObjects:
+        NumberOfHGI += Number_of_HGI(agentObj.output_consumer_agent)
         if not agentObj.llm:
             agentObj.llm = llm
-
         verify_llm_attr(agentObj)
-
         agent_list.append(agentObj.agentName)
-
+    setGHGI(NumberOfHGI)
+    logging.info(f"Total number of HGI agents: {NumberOfHGI}")
     agentInitSystem(agent_list=agent_list)
-
     print(agent_list)
-
     if not DynamicAgentObjectsList:
         agentThreadsStart(agentObjectList=AgentObjects, llm=llm)
-
     else:
         for item in AgentObjects:
             if not searchItemInList(DynamicAgentObjectsList, item):
                 # print("Not Found")
-
                 mapper = getGMapper()
-
                 if not item.llm:
                     item.llm = llm
-
                 verify_llm_attr(item)
-
                 item.start_agent(mapper)
-
     # extract - trigger agent list
-
     triggerAgentList = []
-
     for triggerObj in triggerAgentObjectsList:
         if not triggerObj.llm:
             triggerObj.llm = llm
-
         verify_llm_attr(triggerObj)
-
         triggerAgentList.append(triggerObj.agentName)
-
     triggerAgent(triggerAgentList, godTimerDuration=10000)
```

### Comparing `openagi-0.1.0b2/src/openagi/llms/azure.py` & `openagi-0.1.0b3/src/openagi/llms/azure.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/llms/base.py` & `openagi-0.1.0b3/src/openagi/llms/base.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/llms/openagi_main.py` & `openagi-0.1.0b3/src/openagi/llms/openagi_main.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/llms/openai.py` & `openagi-0.1.0b3/src/openagi/llms/openai.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/queue/message_broker.py` & `openagi-0.1.0b3/src/openagi/queue/message_broker.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/queue/pq.py` & `openagi-0.1.0b3/src/openagi/queue/pq.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/queue/timer_pool.py` & `openagi-0.1.0b3/src/openagi/queue/timer_pool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/base.py` & `openagi-0.1.0b3/src/openagi/tools/base.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/custom_tools/ProxyTool.py` & `openagi-0.1.0b3/src/openagi/tools/custom_tools/ProxyTool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/__init__.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/dalle_image_generator.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/dalle_image_generator.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/document_compare.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/document_compare.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/duckducksearch.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/duckducksearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/exa_search_tool.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/exa_search_tool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/github.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/github.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/gmail.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/gmail.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/google_finance_search.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/google_finance_search.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/google_serper_specific.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/google_serper_specific.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/googlejobsearch.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/googlejobsearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/googleserpersearch.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/googleserpersearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/nasa.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/nasa.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/open_weathermap.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/open_weathermap.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/polygon.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/polygon.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/serper_intermediate.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/serper_intermediate.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/sql.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/sql.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/wikipedia_tool.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/wikipedia_tool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/xorbits.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/xorbits.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/yahoofinancenews.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/yahoofinancenews.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/integrations/youtubesearch.py` & `openagi-0.1.0b3/src/openagi/tools/integrations/youtubesearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/tools_db.py` & `openagi-0.1.0b3/src/openagi/tools/tools_db.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/tools/utils.py` & `openagi-0.1.0b3/src/openagi/tools/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 
 from exa_py import Exa
 from langchain.agents import (
     tool,
 )
-
+import threading
 from openagi.tools.integrations.duckducksearch import getDuckduckgoSearchResults
 from openagi.utils.yamlParse import read_yaml_config
 
+g_num_of_HGI = 0
+lock = threading.Lock()
 
 def getToolExecutionResults(
     agentName, role, goal, backstrory, task, capability, tools_list, llm_api
 ):
     if capability == "search_executor":
         indices = search_string_in_list(tools_list, "duckduckgo-search")
         if indices:
@@ -35,14 +37,45 @@
     """
     indices = []
     for index, item in enumerate(my_list):
         if item == target_string:
             indices.append(index)
     return indices
 
+def Number_of_HGI(my_list):
+    """
+    Search for a HGI in the list.
+
+    Parameters:
+    - my_list (list): The list to search through.
+
+    Returns:
+    - list: A list of indices where the target string is found.
+    """
+    target = "HGI"
+    count = 0
+    for item in my_list:
+        if item == target:
+            count += 1
+    return count
+
+def setGHGI(value):
+    global g_num_of_HGI
+    g_num_of_HGI = value
+    logging.debug(f"Number of HGI set to: {g_num_of_HGI}")
+    
+def isLastHGI():
+    global g_num_of_HGI
+    with lock:
+        g_num_of_HGI -= 1
+        logging.debug(f"Number of HGI reduced to: {g_num_of_HGI}")
+        if g_num_of_HGI == 0:
+            return True
+        else:
+            return False
 
 def ExaAdvToolSetup():
     exa = Exa(api_key=read_yaml_config("EXA_API_KEY", raise_exception=True))
 
     @tool
     def search(query: str, include_domains=None, start_published_date=None):
         """Search for a webpage based on the query.
```

### Comparing `openagi-0.1.0b2/src/openagi/utils/extraction.py` & `openagi-0.1.0b3/src/openagi/utils/extraction.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/utils/llmTasks.py` & `openagi-0.1.0b3/src/openagi/utils/llmTasks.py`

 * *Files identical despite different names*

### Comparing `openagi-0.1.0b2/src/openagi/utils/yamlParse.py` & `openagi-0.1.0b3/src/openagi/utils/yamlParse.py`

 * *Files identical despite different names*

