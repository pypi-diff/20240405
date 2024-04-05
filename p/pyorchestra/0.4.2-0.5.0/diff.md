# Comparing `tmp/pyorchestra-0.4.2.tar.gz` & `tmp/pyorchestra-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorchestra-0.4.2.tar", max compression
+gzip compressed data, was "pyorchestra-0.5.0.tar", max compression
```

## Comparing `pyorchestra-0.4.2.tar` & `pyorchestra-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rwxr-xr-x   0        0        0     7652 2024-04-03 12:34:58.681928 pyorchestra-0.4.2/LICENSE
--rwxr-xr-x   0        0        0    25622 2024-04-03 12:34:58.681928 pyorchestra-0.4.2/README.md
--rwxr-xr-x   0        0        0       62 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/__init__.py
--rwxr-xr-x   0        0        0      265 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/__init__.py
--rwxr-xr-x   0        0        0     1045 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/job.py
--rwxr-xr-x   0        0        0      844 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/run.py
--rwxr-xr-x   0        0        0      208 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/schedule_definition.py
--rwxr-xr-x   0        0        0     1294 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/task.py
--rwxr-xr-x   0        0        0      656 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/main.py
--rwxr-xr-x   0        0        0     7682 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/routers/jobs.py
--rwxr-xr-x   0        0        0      519 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/routers/tags.py
--rwxr-xr-x   0        0        0      603 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/routers/tasks.py
--rwxr-xr-x   0        0        0     1839 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/backend.py
--rwxr-xr-x   0        0        0    19404 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/core.py
--rwxr-xr-x   0        0        0      873 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/formatting.py
--rwxr-xr-x   0        0        0     1455 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/models.py
--rwxr-xr-x   0        0        0    10731 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/scheduling.py
--rwxr-xr-x   0        0        0     1104 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    26496 1970-01-01 00:00:00.000000 pyorchestra-0.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     7652 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/LICENSE
+-rwxr-xr-x   0        0        0    25622 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/README.md
+-rwxr-xr-x   0        0        0       62 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/__init__.py
+-rwxr-xr-x   0        0        0      265 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/__init__.py
+-rwxr-xr-x   0        0        0     2514 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/job.py
+-rwxr-xr-x   0        0        0      844 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/run.py
+-rwxr-xr-x   0        0        0      655 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/schedule_definition.py
+-rwxr-xr-x   0        0        0     1294 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/task.py
+-rwxr-xr-x   0        0        0      656 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/main.py
+-rwxr-xr-x   0        0        0    10221 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/routers/jobs.py
+-rwxr-xr-x   0        0        0      519 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/routers/tags.py
+-rwxr-xr-x   0        0        0      603 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/routers/tasks.py
+-rwxr-xr-x   0        0        0     1839 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/backend.py
+-rwxr-xr-x   0        0        0    19474 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/core.py
+-rwxr-xr-x   0        0        0      873 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/formatting.py
+-rwxr-xr-x   0        0        0      168 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/job.py
+-rwxr-xr-x   0        0        0     1575 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/models.py
+-rwxr-xr-x   0        0        0    10720 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/scheduling.py
+-rwxr-xr-x   0        0        0     1104 2024-04-05 14:15:22.448179 pyorchestra-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    26496 1970-01-01 00:00:00.000000 pyorchestra-0.5.0/PKG-INFO
```

### Comparing `pyorchestra-0.4.2/LICENSE` & `pyorchestra-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.2/README.md` & `pyorchestra-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.2/orchestra/api/dto/run.py` & `pyorchestra-0.5.0/orchestra/api/dto/run.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.2/orchestra/api/dto/task.py` & `pyorchestra-0.5.0/orchestra/api/dto/task.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.2/orchestra/api/main.py` & `pyorchestra-0.5.0/orchestra/api/main.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.2/orchestra/api/routers/jobs.py` & `pyorchestra-0.5.0/orchestra/api/routers/jobs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 from typing import Annotated
 
 from fastapi import APIRouter, Body, Path, Query, Response, status
-
-from orchestra.api.dto import JobDTO, ScheduleDefinitionDTO, RunDTO
+from orchestra.api.dto import RunDTO, JobDTO, ScheduleDefinitionDTO
 from orchestra.core import instance
+from orchestra.job import StatefulJob
 from orchestra.models import Run
 
+
 router = APIRouter(prefix="/api")
 
 
-@router.get("/jobs", tags=["jobs"])
-async def get_jobs(tags: Annotated[str | None, Query(description="Comma separated tags to filter scheduled jobs")] = None,
-                   any_tag: Annotated[bool, Query(description="Set to true to match if only at least one tag has to match")] = False,
-                   include_paused: Annotated[bool, Query(description="Set to true to include paused jobs when searching for a match")] = True) -> list[JobDTO]:
-    tags: set[str] = set(tags.split(",")) if tags else set()
-    return list(map(lambda job: JobDTO.map(job), instance.get_jobs(tags, any_tag, include_paused=include_paused)))
+def filter_jobs(tags: list[str] | None = None,
+                name_fragment: str | None = None,
+                job_names: list[str] | None = None,
+                any_tag: bool = False,
+                is_paused: bool | None = None) -> set[StatefulJob]:
+    tags: set[str] = set(tags) if tags else set()
+    name_fragment: str = name_fragment or ""
+
+    results: set[StatefulJob] = set()
+
+    for stateful_job in instance.get_jobs(tags, any_tag, is_paused):
+        if name_fragment not in stateful_job.job.alias:
+            continue
+
+        if job_names and stateful_job.job.alias not in job_names:
+            continue
+
+        results.add(stateful_job)
+
+    return results
 
 
 @router.post("/jobs", tags=["jobs"], status_code=201)
 async def schedule_new_job(module: Annotated[str, Body()], schedule_definition: ScheduleDefinitionDTO):
     module_definition = [
         {"module": module,
          "schedules": [
@@ -31,57 +46,80 @@
                      "timezone": schedule_definition.timezone or "utc"
                  }
              }
          ]}]
     instance.add_schedules(module_definition, attempt_resume=schedule_definition.resume or False)
 
 
+@router.get("/jobs", tags=["jobs"])
+async def get_jobs(tags: Annotated[list[str] | None, Query(description="Optional list of tags to filter scheduled jobs")] = None,
+                   name_fragment: Annotated[str | None, Query(description="Optional string to filter scheduled jobs' names")] = None,
+                   job_names: Annotated[list[str] | None, Query(description="An optional set of exact job names to match")] = None,
+                   any_tag: Annotated[bool, Query(description="Set to true to match if only at least one tag has to match")] = False,
+                   is_paused: Annotated[bool | None, Query(description="Filter jobs by their state when searching for a match")] = None) -> list[JobDTO]:
+    jobs = filter_jobs(tags, name_fragment, job_names, any_tag, is_paused)
+    return list(map(lambda job: JobDTO.map(job), jobs))
+
+
 @router.delete("/jobs", tags=["jobs"])
-async def delete_scheduled_jobs_matching_tags(tags: Annotated[str | None, Query(description="Comma separated tags to filter scheduled jobs")] = None,
-                                              any_tag: Annotated[bool, Query(description="Set to true to match if only at least one tag has to match")] = False,
-                                              include_paused: Annotated[bool, Query(description="Set to true to include paused jobs when searching for a match")] = False) -> list[JobDTO]:
-    tags: set[str] = set(tags.split(",")) if tags else set()
-    return list(map(lambda job: JobDTO.map(job), instance.delete_jobs_with_tags(tags, any_tag, include_paused)))
+async def delete_scheduled_jobs(tags: Annotated[list[str] | None, Body(description="Optional list of tags to filter scheduled jobs")] = None,
+                                name_fragment: Annotated[str | None, Body(description="Optional string to filter scheduled jobs' names")] = None,
+                                job_names: Annotated[list[str] | None, Body(description="An optional set of exact job names to match")] = None,
+                                any_tag: Annotated[bool, Body(description="Set to true to match if only at least one tag has to match")] = False,
+                                is_paused: Annotated[bool | None, Body(description="Filter jobs by their state when searching for a match")] = None) -> list[JobDTO]:
+    jobs = filter_jobs(tags, name_fragment, job_names, any_tag, is_paused)
+    return list(map(lambda job: JobDTO.map(job), instance.delete_jobs(jobs)))
 
 
 @router.post("/jobs/trigger", tags=["jobs"])
-async def trigger_scheduled_jobs_matching_tags(tags: Annotated[str | None, Query(description="Comma separated tags to filter scheduled jobs")] = None,
-                                               any_tag: Annotated[bool, Query(description="Set to true to match if only at least one tag has to match")] = True,
-                                               include_paused: Annotated[bool, Query(description="Set to true to include paused jobs when searching for a match")] = True) -> list[JobDTO]:
-    tags: set[str] = set(tags.split(",")) if tags else set()
-    return list(map(lambda job: JobDTO.map(job), await instance.trigger_jobs_with_tags(tags, any_tag, include_paused)))
-
-
-@router.post("/jobs/pause", tags=["jobs"])
-async def pause_scheduled_jobs_matching_tags(tags: Annotated[str | None, Query(description="Comma separated tags to filter scheduled jobs")] = None,
-                                             any_tag: Annotated[bool, Query(description="Set to true to match if only at least one tag has to match")] = True) -> list[JobDTO]:
-    tags: set[str] = set(tags.split(",")) if tags else set()
-    return list(map(lambda job: JobDTO.map(job), instance.pause_jobs_with_tags(tags, any_tag)))
-
-
-@router.post("/jobs/resume", tags=["jobs"])
-async def resume_scheduled_jobs_matching_tags(tags: Annotated[str | None, Query(description="Comma separated tags to filter scheduled jobs")] = None,
-                                              any_tag: Annotated[bool, Query(description="Set to true to match if only at least one tag has to match")] = True) -> list[JobDTO]:
-    tags: set[str] = set(tags.split(",")) if tags else set()
-    return list(map(lambda job: JobDTO.map(job), instance.resume_jobs_with_tags(tags, any_tag)))
+async def trigger_scheduled_jobs(tags: Annotated[list[str] | None, Body(description="Optional list of tags to filter scheduled jobs")] = None,
+                                 name_fragment: Annotated[str | None, Body(description="Optional string to filter scheduled jobs' names")] = None,
+                                 job_names: Annotated[list[str] | None, Body(description="An optional set of exact job names to match")] = None,
+                                 any_tag: Annotated[bool, Body(description="Set to true to match if only at least one tag has to match")] = False,
+                                 is_paused: Annotated[bool | None, Body(description="Filter jobs by their state when searching for a match")] = None) -> list[JobDTO]:
+    jobs = filter_jobs(tags, name_fragment, job_names, any_tag, is_paused)
+    return list(map(lambda job: JobDTO.map(job), await instance.trigger_jobs(jobs)))
+
+
+@router.put("/jobs/pause", tags=["jobs"])
+async def pause_scheduled_jobs(tags: Annotated[list[str] | None, Body(description="Optional list of tags to filter scheduled jobs")] = None,
+                               name_fragment: Annotated[str | None, Body(description="Optional string to filter scheduled jobs' names")] = None,
+                               job_names: Annotated[list[str] | None, Body(description="An optional set of exact job names to match")] = None,
+                               any_tag: Annotated[bool, Body(description="Set to true to match if only at least one tag has to match")] = False,
+                               is_paused: Annotated[bool | None, Body(description="Filter jobs by their state when searching for a match")] = None) -> list[JobDTO]:
+    jobs = filter_jobs(tags, name_fragment, job_names, any_tag, is_paused)
+    return list(map(lambda job: JobDTO.map(job), instance.pause_jobs(jobs)))
+
+
+@router.put("/jobs/resume", tags=["jobs"])
+async def resume_scheduled_jobs(tags: Annotated[list[str] | None, Body(description="Optional list of tags to filter scheduled jobs")] = None,
+                                name_fragment: Annotated[str | None, Body(description="Optional string to filter scheduled jobs' names")] = None,
+                                job_names: Annotated[list[str] | None, Body(description="An optional set of exact job names to match")] = None,
+                                any_tag: Annotated[bool, Body(description="Set to true to match if only at least one tag has to match")] = False,
+                                is_paused: Annotated[bool | None, Body(description="Filter jobs by their state when searching for a match")] = None) -> list[JobDTO]:
+    jobs = filter_jobs(tags, name_fragment, job_names, any_tag, is_paused)
+    return list(map(lambda job: JobDTO.map(job), instance.resume_jobs(jobs)))
 
 
 @router.get("/jobs/{job_name}", tags=["jobs"], status_code=status.HTTP_200_OK)
 async def get_job_by_name(job_name: Annotated[str, Path(description="The name of the job to for which to fetch runs")], response: Response) -> JobDTO | str:
     if instance.job_exists(job_name):
-        return JobDTO.map(instance.get_job_by_name(job_name, include_paused=True))
+        return JobDTO.map(instance.get_job_by_name(job_name))
     else:
         response.status_code = status.HTTP_404_NOT_FOUND
         return f"Job {job_name} does not exist"
 
 
 @router.get("/jobs/{job_name}/runs", tags=["jobs"], status_code=status.HTTP_200_OK)
-async def get_runs_of_job(job_name: Annotated[str, Path(description="The name of the job to for which to fetch runs")], response: Response, page_size: int = 50, page: int = 1) -> list[RunDTO] | str:
+async def get_runs_of_job(job_name: Annotated[str, Path(description="The name of the job to for which to fetch runs")], response: Response,
+                          run_status: Annotated[str, Query(description="Filter the runs of the job to this status, leave empty to not filter")] = "",
+                          page_size: Annotated[int, Query(description="The amount of runs returned per page")] = 50,
+                          page: Annotated[int, Query(description="The page of results to return")] = 1) -> list[RunDTO] | str:
     if instance.job_exists(job_name):
-        return list(map(lambda run: RunDTO.map(run), instance.get_runs_of_a_job(job_name, page_size, page)))
+        return list(map(lambda run: RunDTO.map(run), instance.get_runs_of_a_job(job_name, run_status, page_size, page)))
     else:
         response.status_code = status.HTTP_404_NOT_FOUND
         return f"Job {job_name} does not exist"
 
 
 @router.get("/jobs/{job_name}/runs/{run_id}", tags=["jobs"], status_code=status.HTTP_200_OK)
 async def get_run_of_job_by_id(job_name: Annotated[str, Path(description="The name of the job to for which to fetch runs")],
```

### Comparing `pyorchestra-0.4.2/orchestra/api/routers/tags.py` & `pyorchestra-0.5.0/orchestra/api/routers/tags.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.2/orchestra/api/routers/tasks.py` & `pyorchestra-0.5.0/orchestra/api/routers/tasks.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.2/orchestra/backend.py` & `pyorchestra-0.5.0/orchestra/backend.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.2/orchestra/core.py` & `pyorchestra-0.5.0/orchestra/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import datetime
 import importlib
 import logging
-from typing import Callable
+from typing import Callable, Any
 
 import celery
 import pytz
 import uvicorn
 from celery import Celery
 from celery.backends.database import session_cleanup
 from rich import box
@@ -18,14 +18,15 @@
 from scheduler.asyncio import Scheduler
 from scheduler.asyncio.job import Job
 from scheduler.trigger.core import Weekday
 from sqlalchemy import select
 from sqlalchemy.orm import joinedload
 
 from orchestra.formatting import pretty_print_block, get_job_state
+from orchestra.job import StatefulJob
 from orchestra.models import Run, TimingAwareTask
 from orchestra.scheduling import Schedule
 
 logging.basicConfig(
     level="INFO", format="%(message)s", datefmt="[%X]", handlers=[RichHandler(rich_tracebacks=True, tracebacks_show_locals=True)]
 )
 
@@ -104,41 +105,36 @@
                 task.cancel()
 
             await asyncio.wait(pending_tasks)
 
         except (asyncio.CancelledError, KeyboardInterrupt):
             logger.warning("User-requested shutdown.")
 
-    def get_job_by_name(self, job_name: str, include_paused: bool = False) -> Job | None:
-        for job in self.apply_state_to_jobs(self.scheduler.jobs.union(self.paused_jobs if include_paused else [])):
-            if job.alias == job_name:
-                return job
-
-    def wrap_celery_task(self, job_name: str, task: celery.Task, additional_options: dict):
+    def wrap_celery_task(self, job_name: str, task: celery.Task, additional_options: dict) -> Callable:
         async def celery_task():
             task_meta = task.apply_async(**additional_options)
             logger.debug(f"Triggered job {job_name}")
             task_meta.created_date = datetime.datetime.now(tz=pytz.utc)
 
             session = self.backend.ResultSession()
             with session_cleanup(session):
                 trigger_timestamp = datetime.datetime.now(tz=pytz.utc)
-                job = self.get_job_by_name(job_name, include_paused=True)
-                if job is None:
+                stateful_job = self.get_job_by_name(job_name)
+                if stateful_job is None:
                     logger.critical(f"Unknown job with name {job_name}")
 
                 module_name, _, task_name = task.name.rpartition(".")
 
                 scheduler_log = Run(
                     job=job_name,
                     module=module_name,
                     task=task_name,
                     task_id=task_meta.id,
-                    schedule=job.type.name if job.max_attempts != 1 else "ONCE",
-                    timezone=job.datetime.tzinfo.zone,
+                    schedule=stateful_job.job.type.name if stateful_job.job.max_attempts != 1 else "ONCE",
+                    timezone=stateful_job.job.datetime.tzinfo.zone,
                     triggered_date=trigger_timestamp,
                 )
                 session.add(scheduler_log)
                 session.commit()
 
         celery_task.__name__ = task.name
         return celery_task
@@ -149,23 +145,24 @@
         task: celery.Task = getattr(module, task_name)
 
         return self.wrap_celery_task(job_name, task, additional_options)
 
     def schedule_celery_task(self, job_name: str, task: Callable, schedule: Callable[..., Job], timing: datetime.datetime | datetime.timedelta | datetime.time | Weekday,
                              tags: set[str] | None = None, attempt_resume: bool = False, additional_options: dict = None):
         module_name, _, task_name = task.name.rpartition(".")  # type:ignore
-        self.schedule_job(job_name=job_name, module_name=module_name, task_name=task_name, schedule=schedule, timing=timing, tags=tags, attempt_resume=attempt_resume, additional_options=additional_options)
+        self.schedule_job(job_name=job_name, module_name=module_name, task_name=task_name, schedule=schedule, timing=timing, tags=tags, attempt_resume=attempt_resume,
+                          additional_options=additional_options)
 
     async def create_schedule(self, module_definitions: list[dict] = None, loop=None) -> None:
         self.scheduler = self.scheduler or Scheduler(tzinfo=pytz.utc, loop=self.get_event_loop(loop))
         if module_definitions is not None:
             self.add_schedules(module_definitions)
 
     def schedule_job(self, job_name: str, module_name: str, task_name: str, schedule: Callable[..., Job], timing: datetime.datetime | datetime.timedelta | datetime.time | Weekday,
-                     tags: set[str] | None = None, attempt_resume: bool = False, additional_options: dict = None):
+                     tags: set[str] | None = None, attempt_resume: bool = False, additional_options: dict = None, schedule_definition: Any = None):
         session = self.backend.ResultSession()
         with session_cleanup(session):
             resume_parameters: dict = {}
             if attempt_resume:
                 logs = (
                     select(Run)
                     .where(Run.job == job_name)
@@ -194,23 +191,26 @@
                                 pytz.timezone(last_run.timezone)
                             )
 
                             resume_parameters = {
                                 "start": next_run_local - datetime.timedelta(seconds=timing.total_seconds())
                             }
 
-            schedule(
+            job = schedule(
                 timing=timing,
                 handle=self.__create_job_from_celery_task_schedule(
                     job_name, module_name, task_name, additional_options or {}
                 ),
                 alias=job_name,
                 tags=tags or set(),
                 **resume_parameters,
             )
+
+            job.definition = schedule_definition or {}
+
             if "start" in resume_parameters:
                 logger.warning(
                     f"Job {job_name} was scheduled to run {timing}, resuming using {last_running_time_local}, tz={last_run.timezone} as reference time."
                     f" Next run at {next_run_local}, tz={last_run.timezone}"
                 )
             else:
                 logger.info(f"Job {job_name} was scheduled to run {timing}")
@@ -263,123 +263,122 @@
                 self.schedule_job(job_name=job_name,
                                   module_name=block_module,
                                   task_name=task_name,
                                   schedule=schedule.job_type,
                                   timing=schedule.get_timing(),
                                   tags=set(schedule_definition.get("tags", set())),
                                   attempt_resume=attempt_resume,
-                                  additional_options=schedule_definition.get("additional_options"))
+                                  additional_options=schedule_definition.get("additional_options"),
+                                  schedule_definition=schedule_definition)
 
-    @classmethod
-    def set_job_state_property(cls, job: Job, is_paused: bool) -> Job:
-        job.is_paused = is_paused
-        return job
-
-    def apply_state_to_jobs(self, jobs: set[Job]) -> set[Job]:
-        return set([self.set_job_state_property(job, is_paused=True if job in self.paused_jobs else False) for job in jobs])
-
-    def get_jobs(self, tags: set[str], any_tag: bool, include_paused: bool = True):
-        # contrary to what get_jobs' docstring says, get_job will not return all jobs when tag is an empty set
-        if len(tags) == 0:
-            active_jobs = self.scheduler.jobs
-        else:
-            active_jobs = set(filter(lambda job: job.tags.intersection(tags) if any_tag else job.tags == tags, self.scheduler.jobs))
+    def apply_state_to_jobs(self, jobs: set[Job]) -> set[StatefulJob]:
+        return set([StatefulJob(job, is_paused=True if job in self.paused_jobs else False) for job in jobs])
 
-        paused_jobs = set()
-        if include_paused:
-            paused_jobs = self.get_paused_jobs(tags, any_tag=any_tag)
+    def get_jobs(self, tags: set[str] | None = None, any_tag: bool = True, is_paused: bool | None = None) -> set[StatefulJob]:
+        tags = tags or set()
+        if is_paused is None:
+            jobs = self.paused_jobs.union(self.scheduler.jobs)
+        else:
+            jobs = self.paused_jobs if is_paused else self.scheduler.jobs
 
-        return self.apply_state_to_jobs(active_jobs.union(paused_jobs))
+        if len(tags) > 0:
+            jobs = set(filter(lambda job: job.tags.intersection(tags) if any_tag else job.tags == tags, jobs))
 
-    def job_exists(self, job_name: str):
-        return self.get_job_by_name(job_name, include_paused=True) is not None
+        return self.apply_state_to_jobs(jobs)
 
-    def get_paused_jobs(self, tags: set[str], any_tag: bool):
-        if len(tags) == 0:
-            return self.paused_jobs
-        return self.apply_state_to_jobs(set(filter(lambda job: job.tags.intersection(tags) if any_tag else job.tags == tags, self.paused_jobs)))
+    def job_exists(self, job_name: str) -> bool:
+        return self.get_job_by_name(job_name) is not None
+
+    def get_jobs_by_state(self, is_paused: bool | None) -> set[StatefulJob]:
+        match is_paused:
+            case None:
+                return self.apply_state_to_jobs(self.scheduler.jobs.union(self.paused_jobs))
+            case True:
+                return self.apply_state_to_jobs(self.paused_jobs)
+            case False:
+                return self.apply_state_to_jobs(self.scheduler.jobs)
+
+    def get_job_by_name(self, job_name: str) -> StatefulJob | None:
+        for stateful_job in self.get_jobs():
+            if stateful_job.job.alias == job_name:
+                return stateful_job
 
-    def pause_job(self, job_name: str):
-        job = self.get_job_by_name(job_name)
+    def pause_job(self, job_name: str) -> StatefulJob:
+        job = self.get_job_by_name(job_name).job
         assert job is not None
         self.scheduler.delete_job(job)
         self.paused_jobs.add(job)
         logger.info(f"Paused job {job_name}")
-        return self.set_job_state_property(job, is_paused=True)
-
-    def pause_jobs_with_tags(self, tags: set[str], any_tag: bool):
-        jobs_to_pause = self.get_jobs(tags, any_tag, include_paused=False)
-
-        for job in jobs_to_pause:
-            self.pause_job(job.alias)
+        return StatefulJob(job, is_paused=True)
 
-        return self.apply_state_to_jobs(jobs_to_pause)
-
-    def resume_job(self, job_name: str) -> Job:
-        job = self.get_job_by_name(job_name, include_paused=True)
-        assert job is not None
-        self.paused_jobs.remove(job)
-        task = self.scheduler._Scheduler__loop.create_task(self.scheduler._Scheduler__supervise_job(job))
-        self.scheduler._Scheduler__jobs[job] = task
-        logger.info(f"Resumed job {job_name}")
-        return self.set_job_state_property(job, is_paused=False)
-
-    def resume_jobs_with_tags(self, tags: set[str], any_tag: bool):
-        jobs_to_resume = self.get_paused_jobs(tags, any_tag)
-
-        for job in jobs_to_resume:
-            self.resume_job(job.alias)
-
-        return self.apply_state_to_jobs(jobs_to_resume)
-
-    def delete_job(self, job_name: str) -> Job | None:
-        job = self.get_job_by_name(job_name, True)
-        if job in self.paused_jobs:
-            self.paused_jobs.remove(job)
+    def pause_jobs(self, jobs_to_pause: set[StatefulJob]) -> set[StatefulJob]:
+        for stateful_job in jobs_to_pause:
+            self.pause_job(stateful_job.job.alias)
+
+        return self.apply_state_to_jobs(set(map(lambda state: state.job, jobs_to_pause)))
+
+    def resume_job(self, job_name: str) -> StatefulJob:
+        stateful_job = self.get_job_by_name(job_name)
+        if stateful_job.is_paused:
+            self.paused_jobs.remove(stateful_job.job)
+            task = self.scheduler._Scheduler__loop.create_task(self.scheduler._Scheduler__supervise_job(stateful_job.job))
+            self.scheduler._Scheduler__jobs[stateful_job.job] = task
+            logger.info(f"Resumed job {job_name}")
+
+        return StatefulJob(stateful_job.job, is_paused=False)
+
+    def resume_jobs(self, jobs_to_resume: set[StatefulJob]) -> set[StatefulJob]:
+        for stateful_job in jobs_to_resume:
+            self.resume_job(stateful_job.job.alias)
+
+        return self.apply_state_to_jobs(set(map(lambda state: state.job, jobs_to_resume)))
+
+    def delete_job(self, job_name: str) -> StatefulJob | None:
+        stateful_job = self.get_job_by_name(job_name)
+        if stateful_job.is_paused:
+            self.paused_jobs.remove(stateful_job.job)
         else:
-            self.scheduler.delete_job(job)
+            self.scheduler.delete_job(stateful_job.job)
+
+        return stateful_job
 
-        return job
+    def delete_jobs(self, jobs_to_delete: set[StatefulJob]) -> set[StatefulJob]:
+        for stateful_job in jobs_to_delete:
+            if stateful_job.is_paused:
+                self.paused_jobs.remove(stateful_job.job)
+            else:
+                self.scheduler.delete_job(stateful_job.job)
 
-    def delete_jobs_with_tags(self, tags: set[str], any_tag: bool, include_paused: bool = True):
-        active_jobs_to_delete = self.apply_state_to_jobs(self.get_jobs(tags, any_tag, include_paused=False))
-        self.scheduler.delete_jobs(tags, any_tag)
-
-        paused_jobs_to_delete = set()
-        if include_paused:
-            paused_jobs_to_delete = self.apply_state_to_jobs(self.get_jobs(tags, any_tag, include_paused=True))
-            for job in paused_jobs_to_delete:
-                self.delete_job(job.alias)
-        return active_jobs_to_delete.union(paused_jobs_to_delete)
+        return jobs_to_delete
 
     async def trigger_job(self, job_name: str):
-        job = self.get_job_by_name(job_name, include_paused=True)
+        job = self.get_job_by_name(job_name).job
         assert job is not None
         await job.handle()
         logger.info(f"Job {job_name} triggered manually")
-        if job.max_attempts == 1:
-            self.scheduler.delete_job(job)
-
-    async def trigger_jobs_with_tags(self, tags: set[str], any_tag: bool, include_paused: bool):
-        jobs_to_trigger = self.apply_state_to_jobs(self.get_jobs(tags, any_tag, include_paused))
 
+    async def trigger_jobs(self, jobs_to_trigger: set[StatefulJob]) -> set[StatefulJob]:
         async with asyncio.TaskGroup() as tg:
-            [tg.create_task(job.handle()) for job in jobs_to_trigger]
+            [tg.create_task(stateful_job.job.handle()) for stateful_job in jobs_to_trigger]
 
-        for job in jobs_to_trigger:
-            logger.info(f"Job {job.alias} triggered manually")
-            if job.max_attempts == 1:
-                self.scheduler.delete_job(job)
+        for stateful_job in jobs_to_trigger:
+            logger.info(f"Job {stateful_job.job.alias} triggered manually")
 
         return jobs_to_trigger
 
-    def get_runs_of_a_job(self, job_name: str, page_size: int, page: int) -> list[Run]:
+    def get_runs_of_a_job(self, job_name: str, run_status: str, page_size: int, page: int) -> list[Run]:
         session = self.backend.ResultSession()
         with session_cleanup(session):
-            runs: list[Run] = list(session.scalars(select(Run).where(Run.job == job_name).order_by(Run.triggered_date.desc()).offset((page - 1) * page_size).limit(page_size).options(joinedload(Run.task_object))))
+            if run_status == "pending":
+                runs = list(session.scalars(select(Run).where(Run.job == job_name, ~Run.task_status.has()).order_by(Run.triggered_date.desc()).options(joinedload(Run.task_object))))
+            else:
+                runs: list[Run] = list(
+                    session.scalars(
+                        select(Run).where(Run.job == job_name, Run.task_status == run_status.upper()).order_by(Run.triggered_date.desc()).offset((page - 1) * page_size).limit(
+                            page_size).options(joinedload(Run.task_object))))
             return runs
 
     def get_run_of_a_job_by_id(self, job_name: str, run_id: int) -> Run | None:
         session = self.backend.ResultSession()
         with session_cleanup(session):
             run: Run = next(session.scalars(select(Run).where(Run.job == job_name, Run.id == run_id).limit(1).options(joinedload(Run.task_object))), None)
             return run
```

### Comparing `pyorchestra-0.4.2/orchestra/formatting.py` & `pyorchestra-0.5.0/orchestra/formatting.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.2/orchestra/models.py` & `pyorchestra-0.5.0/orchestra/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 from enum import Enum
 
 import sqlalchemy as sa
 from celery.backends.database.models import TaskExtended, ResultModelBase
-from sqlalchemy import TIMESTAMP, Text, ForeignKey
+from sqlalchemy import TIMESTAMP
+from sqlalchemy.ext.associationproxy import association_proxy
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 
 class TimingAwareTask(TaskExtended):
     """Task result/status."""
     __tablename__ = 'celery_taskmeta'
     __table_args__ = {'sqlite_autoincrement': True, 'extend_existing': True}
@@ -33,15 +34,16 @@
     module: Mapped[str]
     task: Mapped[str]
     task_id: Mapped[str]
     schedule: Mapped[str]
     timezone: Mapped[str | None]
     triggered_date: Mapped[datetime] = sa.Column(TIMESTAMP(timezone=True))
 
-    task_object = relationship("TimingAwareTask", primaryjoin='foreign(Run.task_id) == TimingAwareTask.task_id')
+    task_object = relationship("TimingAwareTask", primaryjoin='foreign(Run.task_id) == TimingAwareTask.task_id', uselist=False)
+    task_status = association_proxy('task_object', 'status')
 
 
 class Status(str, Enum):
     pending = "pending"
     started = "started"
     success = "success"
     failure = "failure"
```

### Comparing `pyorchestra-0.4.2/orchestra/scheduling.py` & `pyorchestra-0.5.0/orchestra/scheduling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import re
-import sys
 from datetime import datetime, time, timedelta
 from typing import Callable, Optional
 
 import pytz.exceptions
 import scheduler.trigger as weekdays
 from pytz import timezone
 from scheduler import Scheduler
```

### Comparing `pyorchestra-0.4.2/pyproject.toml` & `pyorchestra-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyorchestra"
-version = "0.4.2"
+version = "0.5.0"
 description = "Orchestra is a job scheduler on top of Celery"
 authors = ["András Vidosits <andras@hyperplane.hu>"]
 readme = "README.md"
 license = "LGPLv3"
 repository = "https://github.com/vidosits/orchestra"
 packages = [
 	{ include = "orchestra" },
```

### Comparing `pyorchestra-0.4.2/PKG-INFO` & `pyorchestra-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorchestra
-Version: 0.4.2
+Version: 0.5.0
 Summary: Orchestra is a job scheduler on top of Celery
 Home-page: https://github.com/vidosits/orchestra
 License: LGPLv3
 Author: András Vidosits
 Author-email: andras@hyperplane.hu
 Requires-Python: >=3.11.7,<4.0.0
 Classifier: License :: Other/Proprietary License
```

