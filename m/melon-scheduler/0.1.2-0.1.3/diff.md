# Comparing `tmp/melon_scheduler-0.1.2.tar.gz` & `tmp/melon_scheduler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melon_scheduler-0.1.2.tar", max compression
+gzip compressed data, was "melon_scheduler-0.1.3.tar", max compression
```

## Comparing `melon_scheduler-0.1.2.tar` & `melon_scheduler-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,27 @@
--rw-r--r--   0        0        0     2108 2023-06-27 22:02:19.451664 melon_scheduler-0.1.2/README.md
--rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.2/melon/__init__.py
--rw-r--r--   0        0        0     4366 2023-06-30 13:07:13.877474 melon_scheduler-0.1.2/melon/calendar.py
--rw-r--r--   0        0        0      337 2023-06-30 14:09:58.520159 melon_scheduler-0.1.2/melon/config.py
--rw-r--r--   0        0        0      401 2023-06-26 13:37:58.951726 melon_scheduler-0.1.2/melon/libscheduler.rs
--rw-r--r--   0        0        0     7310 2023-06-30 13:04:39.283709 melon_scheduler-0.1.2/melon/melon.py
--rw-r--r--   0        0        0     6262 2023-06-30 12:22:34.016082 melon_scheduler-0.1.2/melon/scheduler.py
--rw-r--r--   0        0        0     6489 2023-06-30 12:44:19.705982 melon_scheduler-0.1.2/melon/todo.py
--rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.2/melongui/__init__.py
--rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.2/melongui/assets/complete.png
--rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.2/melongui/assets/complete.svg
--rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.2/melongui/calendarlist.py
--rw-r--r--   0        0        0     4882 2023-06-29 19:52:23.397332 melon_scheduler-0.1.2/melongui/mainwindow.py
--rw-r--r--   0        0        0     5980 2023-06-27 19:31:46.233422 melon_scheduler-0.1.2/melongui/taskitemdelegate.py
--rw-r--r--   0        0        0     5417 2023-06-26 15:51:18.939957 melon_scheduler-0.1.2/melongui/tasklist.py
--rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.2/melongui/taskwidgets.py
--rw-r--r--   0        0        0     1057 2023-06-30 14:10:42.091424 melon_scheduler-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 melon_scheduler-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2108 2023-06-27 22:02:19.451664 melon_scheduler-0.1.3/README.md
+-rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.3/melon/__init__.py
+-rw-r--r--   0        0        0     4581 2023-06-30 17:27:21.260501 melon_scheduler-0.1.3/melon/calendar.py
+-rw-r--r--   0        0        0      554 2023-07-01 15:24:46.251746 melon_scheduler-0.1.3/melon/config.py
+-rw-r--r--   0        0        0     8528 2023-07-01 21:33:46.176496 melon_scheduler-0.1.3/melon/melon.py
+-rw-r--r--   0        0        0       91 2023-07-01 17:20:32.719529 melon_scheduler-0.1.3/melon/scheduler/__init__.py
+-rw-r--r--   0        0        0     2130 2023-07-01 23:15:52.115000 melon_scheduler-0.1.3/melon/scheduler/base.py
+-rw-r--r--   0        0        0      860 2023-07-01 20:04:35.083343 melon_scheduler-0.1.3/melon/scheduler/cpp.py
+-rw-r--r--   0        0        0     4409 2023-07-01 20:04:02.823397 melon_scheduler-0.1.3/melon/scheduler/libcppscheduler.cpp
+-rw-r--r--   0        0        0      444 2023-07-01 19:54:02.564583 melon_scheduler-0.1.3/melon/scheduler/libcppscheduler.pyi
+-rw-r--r--   0        0        0      444 2023-07-01 14:38:21.981201 melon_scheduler-0.1.3/melon/scheduler/libscheduler.pyi
+-rw-r--r--   0        0        0     3728 2023-07-01 17:33:44.781423 melon_scheduler-0.1.3/melon/scheduler/libscheduler.rs
+-rw-r--r--   0        0        0     4514 2023-07-01 22:10:30.415308 melon_scheduler-0.1.3/melon/scheduler/numba.py
+-rw-r--r--   0        0        0     6077 2023-07-01 22:58:26.628198 melon_scheduler-0.1.3/melon/scheduler/purepython.py
+-rw-r--r--   0        0        0      866 2023-07-01 17:30:04.006010 melon_scheduler-0.1.3/melon/scheduler/rust.py
+-rw-r--r--   0        0        0     6768 2023-07-01 22:26:24.282641 melon_scheduler-0.1.3/melon/todo.py
+-rw-r--r--   0        0        0     1502 2023-07-01 22:38:29.259935 melon_scheduler-0.1.3/melon/visualise.py
+-rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.3/melongui/__init__.py
+-rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.3/melongui/assets/complete.png
+-rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.3/melongui/assets/complete.svg
+-rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.3/melongui/calendarlist.py
+-rw-r--r--   0        0        0     4886 2023-06-30 17:10:21.279889 melon_scheduler-0.1.3/melongui/mainwindow.py
+-rw-r--r--   0        0        0     5980 2023-06-27 19:31:46.233422 melon_scheduler-0.1.3/melongui/taskitemdelegate.py
+-rw-r--r--   0        0        0     5783 2023-07-01 22:05:47.643986 melon_scheduler-0.1.3/melongui/tasklist.py
+-rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.3/melongui/taskwidgets.py
+-rw-r--r--   0        0        0     1257 2023-07-01 23:23:50.324341 melon_scheduler-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 melon_scheduler-0.1.3/PKG-INFO
```

### Comparing `melon_scheduler-0.1.2/README.md` & `melon_scheduler-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.2/melon/calendar.py` & `melon_scheduler-0.1.3/melon/calendar.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,34 +92,38 @@
         }
 
     def sync(self):
         """Synchronise me"""
         assert self.name is not None
         assert self.syncable is not None
         updated, deleted = self.syncable.sync()
-        self.syncable.objects = [
-            todo if isinstance(todo, Todo) else Todo.upgrade(todo, self.name) for todo in self.syncable.objects
-        ]
+        self.syncable.upgradeObjects(self.name)
         logging.info(
             f"Synced {self.name:48} ({len(updated)} updated and {len(deleted)} deleted entries.) "
             f"In total, we have {len(self.syncable)} objects."
         )
 
 
 class Syncable(caldav.SynchronizableCalendarObjectCollection):
     """The synchronisable collection of CalDAV objects, handling efficient syncs between server and client."""
 
     calendar: Calendar
     objects: Iterable[Todo]
     sync_token: str
 
+    def upgradeObjects(self, calendarName: str):
+        """Converts all objects in self.objects to Todos."""
+        self.objects = [todo if isinstance(todo, Todo) else Todo.upgrade(todo, calendarName) for todo in self.objects]
+
     @staticmethod
-    def upgrade(synchronisable: caldav.SynchronizableCalendarObjectCollection) -> "Syncable":
+    def upgrade(synchronisable: caldav.SynchronizableCalendarObjectCollection, calendarName: str) -> "Syncable":
         """Upgrades the third-party caldav.SynchronizableCalendarObjectCollection to a Syncable
 
         Args:
             synchronisable (caldav.SynchronizableCalendarObjectCollection): the original instance
 
         Returns:
             (Syncable): the syncable
         """
-        return Syncable(synchronisable.calendar, synchronisable.objects, synchronisable.sync_token)  # type: ignore
+        syncable = Syncable(synchronisable.calendar, synchronisable.objects, synchronisable.sync_token)  # type: ignore
+        syncable.upgradeObjects(calendarName)
+        return syncable
```

### Comparing `melon_scheduler-0.1.2/melon/melon.py` & `melon_scheduler-0.1.3/melon/melon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,88 @@
 """This file is the main entry point of the melon package, containing the Melon class,
 the main point of contact for users of this package. It can be initialised like this:
 
 melon = Melon()
-melon.startup()
+melon.autoInit()
 """
 import datetime
 import json
 import logging
 import uuid
 from typing import Iterable, Mapping
 
 import caldav
 import caldav.lib.url
 import icalendar
 
 from .calendar import Calendar, Syncable
 from .config import CONFIG, CONFIG_FOLDER
-from .scheduler import MCMCScheduler, TimeSlot
+from .scheduler.base import AbstractScheduler, Task, TimeSlot
+from .scheduler.purepython import MCMCScheduler
 from .todo import Todo
 
 
 class Melon:
     """The Melon class, wrapping a caldav client and principal, loading specifics from the config.
     Through me, users have access to calendars and todos.
     I also handle load, sync and store functionality.
     """
 
     HIDDEN_CALENDARS = ("calendar", None)
 
-    def __init__(self) -> None:
-        """
+    def __init__(
+        self,
+        url=CONFIG["client"]["url"],
+        username=CONFIG["client"]["username"],
+        password=CONFIG["client"]["password"],
+    ) -> None:
+        """Initialises the Melon client
+
         Args:
+            url (str, optional): URL to the CalDAV server. Defaults to CONFIG["client"]["url"].
+            username (str, optional): Username. Defaults to CONFIG["client"]["username"].
+            password (str, optional): Password. Defaults to CONFIG["client"]["password"].
         """
-        self.client = caldav.DAVClient(
-            CONFIG["client"]["url"],
-            username=CONFIG["client"]["username"],
-            password=CONFIG["client"]["password"],
-        )
-        self.principal = None
+        self.client = caldav.DAVClient(url=url, username=username, password=password)
         self.calendars: dict[str, Calendar] = {}
+        self.principal = None
+        self.max_calendars: int | None = None  # the highest number of calendars to load. Useful for testing.
 
     def connect(self):
         """
         Args:
         """
         self.principal = self.client.principal()
         logging.info("Obtained principal")
 
         all_calendars = self.principal.calendars()
+        if self.max_calendars is not None:
+            all_calendars = all_calendars[: self.max_calendars]
         self.calendars = {cal.name: Calendar(cal) for cal in all_calendars if cal.name not in self.HIDDEN_CALENDARS}
         logging.info(f"Obtained {len(self.calendars)} calendars")
 
     def _load_syncable_tasks(self, calendar):
         """
         Args:
             calendar: Argument
         """
         for object in calendar.syncable:
             if "vtodo" in object.vobject_instance.contents:
                 assert isinstance(object, Todo)
                 self.addOrUpdateTask(object)
 
-    def initialFetch(self):
+    def fetch(self):
         """
         Args:
         """
         if not self.calendars:
             self.connect()
         for calendar in self.calendars.values():
-            calendar.syncable = Syncable.upgrade(calendar.objects_by_sync_token(load_objects=True))
+            assert calendar.name is not None
+            calendar.syncable = Syncable.upgrade(calendar.objects_by_sync_token(load_objects=True), calendar.name)
             self._load_syncable_tasks(calendar)
             logging.info(f"Fetched {len(calendar.syncable)} full objects!")
 
     def store(self):
         """
         Args:
         """
@@ -92,25 +102,27 @@
         with open(CONFIG_FOLDER / "synctokens.json") as f:
             data = json.load(f)
         for file in CONFIG_FOLDER.glob("*.dav"):
             name = file.stem  # filename corresponds to the calendar name
             self.calendars[name] = Calendar.loadFromFile(
                 self.client, self.principal, name, data[name]["token"], data[name]["url"]
             )
+            if self.max_calendars is not None and len(self.calendars) >= self.max_calendars:
+                break
         logging.info(f"Loaded {len(self.calendars)} calendars from disk.")
         for calendar in self.calendars.values():
             self._load_syncable_tasks(calendar)
 
-    def init(self):
+    def autoInit(self):
         """
         Args:
         """
         tokensfile = CONFIG_FOLDER / "synctokens.json"
         if not tokensfile.exists():
-            self.initialFetch()
+            self.fetch()
         else:
             self.load()
 
     def syncCalendar(self, calendar: Calendar):
         """
         Args:
             calendar: Argument
@@ -136,14 +148,19 @@
                 continue
             for object in calendar.syncable.objects:
                 if object.uid is None or not object.isTodo():
                     continue
                 yield object
 
     def allIncompleteTasks(self) -> Iterable[Todo]:
+        """Returns all incomplete todos
+
+        Yields:
+            Iterator[Iterable[Todo]]: incomplete todos
+        """
         for todo in self.allTasks():
             if todo.isIncomplete():
                 yield todo
 
     def getTask(self, uid: str) -> Todo:
         """Returns task with given UID
 
@@ -163,16 +180,16 @@
 
     def findTask(self, string: str) -> Iterable[Todo]:
         """Finds a task given a search query
 
         Args:
             string (str): the search query.
 
-        Returns:
-            Iterable[Todo]: the generated search results.
+        Yields:
+            Iterator[Iterable[Todo]]: the generated search results.
         """
         for object in self.allTasks():
             if string in object.data and object.isTodo():
                 yield object
 
     def addOrUpdateTask(self, todo: Todo):
         """
@@ -199,24 +216,33 @@
             event.add("dtstart", slot.timestamp)
             event.add("dtend", slot.end)
             event.add("dtstamp", datetime.datetime.now())
             event.add("uid", uuid.uuid4())
             schedule.add_component(event)
         return schedule
 
-    def scheduleAllAndExport(self, file: str):
+    def tasksToSchedule(self) -> list[Task]:
+        """Returns all incomplete tasks as scheduler.Task objects
+
+        Returns:
+            list[Task]: _description_
+        """
+        return list(map(Todo.toTask, self.allIncompleteTasks()))
+
+    def scheduleAllAndExport(self, file: str, Scheduler: type[AbstractScheduler] = MCMCScheduler):
         """Runs the scheduler on all tasks and exports as an ICS file.
 
         Args:
             file (str): filesystem path that the ics file should be exported to
         """
         logging.info("Initialising scheduler.")
-        scheduler = MCMCScheduler(list(map(Todo.toTask, self.allIncompleteTasks())))
+        scheduler = Scheduler(self.tasksToSchedule())
         logging.info(f"Scheduling {len(scheduler.tasks)} now.")
         schedule = scheduler.schedule()
         logging.info("Exporting.")
         export = self.exportScheduleAsCalendar(schedule)
         logging.info("Export calendar created.")
         # print(export.to_ical().decode().replace("\r\n", "\n"))
         with open(file, "wb") as f:
             f.write(export.to_ical())
         logging.info("Finished export.")
+        return scheduler
```

### Comparing `melon_scheduler-0.1.2/melon/scheduler.py` & `melon_scheduler-0.1.3/melon/scheduler/purepython.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,24 @@
 """The scheduler algorithm"""
-import dataclasses
 import math
 import random
 from datetime import date, datetime, time, timedelta
 from typing import Iterable, Mapping
 
-import tqdm
 
-INITIAL_TEMPERATURE = 0.2
-
-
-@dataclasses.dataclass
-class Task:
-    """Slim struct representing a task"""
-
-    uid: str  # unique identifier of the task
-    duration: float  # estimated, in hours
-    priority: int  # between 1 and 9
-    location: str  # string indicating the location
-
-
-@dataclasses.dataclass
-class TimeSlot:
-    """Slim struct representing a time slot, so an event consisting of a start and end date."""
-
-    timestamp: datetime
-    duration: float  # in hours
-
-    @property
-    def timedelta(self) -> timedelta:
-        """
-        Returns:
-            timedelta: the duration as a datetime.timedelta instance
-        """
-        return timedelta(hours=self.duration)
-
-    @property
-    def end(self) -> datetime:
-        """
-        Returns:
-            datetime: the end timestamp of this time slot
-        """
-        return self.timestamp + self.timedelta
+from .base import DAY_LENGTH, INITIAL_TEMPERATURE, SWEEP_EXPONENT, AbstractScheduler, Task, TimeSlot
 
 
 class AvailabilityManager:
     """This class manages the user's availability in a calendar."""
 
     def __init__(self) -> None:
         """Initialises the availability manager according to defaults."""
         self.startOfDay = time(10, 0)  # start at 10am
-        self.defaultDayLength = 14  # going all the way to 2am
+        self.defaultDayLength = DAY_LENGTH  # going all the way to 2am
 
     def startingSlot(self) -> TimeSlot:
         """Starting slot, starting at 10am today
 
         Returns:
             TimeSlot: the first working slot
         """
@@ -83,97 +47,106 @@
         Yields:
             Iterator[tuple[str, TimeSlot]]: pairs of (UID, TimeSlot), returned in chronological order
         """
         slot = self.startingSlot()
         stamp = slot.timestamp
         for task in tasks:
             if task.duration > self.defaultDayLength:
-                raise ValueError(
+                raise RuntimeError(
                     "You are trying to schedule a task longer than any working slot."
                     "Split it into smaller chunks! Automatic splitting is not supported."
                 )
             taskDuration = timedelta(hours=task.duration)
             if stamp + taskDuration > slot.end:
                 slot = self.generateNextSlot(slot)
                 stamp = slot.timestamp
             yield (task.uid, TimeSlot(stamp, taskDuration.total_seconds() / 3600))
             stamp += taskDuration
 
-    def isAvailable(self, timeslot: TimeSlot) -> bool:
-        """Returns whether the given timeslot could fully fit within the designated timeframe.
-
-        Args:
-            timeslot (TimeSlot): the timeframe
-
-        Returns:
-            bool: whether the task fits
-        """
-        return False
 
-
-class MCMCScheduler:
+class MCMCScheduler(AbstractScheduler):
     """MCMC class to schedule tasks to events in a calendar."""
 
     State = tuple[int, ...]  # using literal ellipsis to indicate a homogenous tuple of ints
 
     def __init__(self, tasks: list[Task]) -> None:
         """Initialises the MCMC scheduler, working on a set of pre-defined tasks.
 
         Args:
             tasks (list[Task]): the tasks to be scheduled
         """
-        self.tasks = tasks
+        super().__init__(tasks)
         self.availability = AvailabilityManager()
         self.state = tuple(range(len(self.tasks)))  # initialise in order
         self.temperature = 1.0
+        self._log = []
 
     def permuteState(self) -> State:
         """Proposes a new state to use instead of the old state.
 
         Returns:
             State: the new state, a list of indices within self.tasks representing traversal order
         """
         newState = list(self.state)
         indexA = random.randrange(len(newState))
         indexB = random.randrange(len(newState))
-        newState[indexA] = indexB
-        newState[indexB] = indexA
-        # print(newState)
+        indexAValue = self.state[indexA]
+        newState[indexA] = self.state[indexB]
+        newState[indexB] = indexAValue
         return tuple(newState)
 
     def computeEnergy(self, state: State) -> float:
         """For the given state, compute an MCMC energy (the lower, the better)
 
         Args:
             state (State): state of the MCMC algorithm
 
         Returns:
             float: the energy / penalty for this state
         """
         spread = list(self.availability.spreadTasks(self.tasks[i] for i in state))
         totalTimePenalty = (spread[-1][1].end - spread[0][1].timestamp).total_seconds() / 3600
-        priorityPenalty = sum(position * self.tasks[state[position]].priority for position in range(len(state)))
+        priorityPenalty = sum(
+            math.sqrt(position) * self.tasks[state[position]].priority for position in range(len(state))
+        )
+        commutePenalty = 0
+        for position in range(1, len(state)):
+            previous = self.tasks[state[position - 1]]
+            current = self.tasks[state[position]]
+            if previous.location == 0 or current.location == 0:
+                continue  # hybrid tasks can be done from anywhere, so do not penalise
+            if previous.location != current.location:
+                commutePenalty += 4
         allOnTime = True  # TODO: check with due date
-        return totalTimePenalty + priorityPenalty
+        # print(totalTimePenalty, priorityPenalty, commutePenalty)
+        return totalTimePenalty + priorityPenalty + commutePenalty
 
     def mcmcSweep(self):
         """Performs a full MCMC sweep"""
         energy = self.computeEnergy(self.state)
-        for i in tqdm.tqdm(range(len(self.tasks) ** 2)):
+        E_sum, E_squared_sum = 0, 0
+        steps = len(self.tasks) ** 2
+        for i in range(steps):
             newState = self.permuteState()
             delta = self.computeEnergy(newState) - energy
             acceptanceProbability = min(math.exp(-delta / (energy * self.temperature)), 1)
-            print(f"New state with energy {energy + delta} (delta {delta}), accepted with {acceptanceProbability}.")
+            # print(f"New state with energy {energy + delta} (delta {delta}), accepted with {acceptanceProbability}.")
             if random.random() < acceptanceProbability:
                 self.state = newState
                 energy += delta
+            E_sum += energy
+            E_squared_sum += energy**2
+        E_avg = E_sum / steps
+        E_var = E_squared_sum / steps - E_avg**2
+        self._log.append((self.temperature, E_avg, E_var))
 
     def schedule(self) -> Mapping[str, TimeSlot]:
         """Schedules the tasks using an MCMC procedure.
 
         Returns:
             Mapping[str, TimeSlot]: the resulting map of Tasks to TimeSlots
         """
         for k in range(1, 11):
+            self.temperature = INITIAL_TEMPERATURE * k**SWEEP_EXPONENT
             self.mcmcSweep()
-            self.temperature = INITIAL_TEMPERATURE * k ** (-1)
+        print("Final State", self.state)
         return dict(self.availability.spreadTasks(self.tasks[i] for i in self.state))
```

### Comparing `melon_scheduler-0.1.2/melon/todo.py` & `melon_scheduler-0.1.3/melon/todo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """This module contains the Todo class."""
 import datetime
+import re
 from typing import Literal
 
 import caldav
 import caldav.lib.url
 import icalendar.cal
 import icalendar.prop
 import vobject
 
-from melon.scheduler import Task
+from melon.scheduler.base import Task
 
 NEW_TASK_TEXT = "An exciting new task!"
 MIDNIGHT = datetime.time(0, 0)
 
 
 class Todo(caldav.Todo):
     """A class representing todos (= tasks), subclassing the caldav.Todo object which in turn stores VTODO data."""
@@ -166,15 +167,22 @@
     def toTask(self) -> Task:
         """Converts this Todo into the scheduler-compatible Task struct.
 
         Returns:
             Task: a melon.scheduler.Task
         """
         assert self.uid is not None
-        return Task(self.uid, 1, self.priority, "work")
+        location = 0
+        if "home" in self.summary:
+            location = 1
+        elif "work" in self.summary:
+            location = 2
+        match = re.search(r"\b([\d\,\.])+h\b", self.summary)
+        hours = float(match.group(1)) if match else 1
+        return Task(self.uid, hours, self.priority, location)
 
     def __lt__(self, other: "Todo") -> bool:
         """Compares two todos in terms of ordering
 
         Args:
             other (Todo): the instance to compare with
```

### Comparing `melon_scheduler-0.1.2/melongui/assets/complete.png` & `melon_scheduler-0.1.3/melongui/assets/complete.png`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.2/melongui/assets/complete.svg` & `melon_scheduler-0.1.3/melongui/assets/complete.svg`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.2/melongui/calendarlist.py` & `melon_scheduler-0.1.3/melongui/calendarlist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.2/melongui/mainwindow.py` & `melon_scheduler-0.1.3/melongui/mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         layout.addWidget(self.tasklistView, 1, 2)
         self.setLayout(layout)
 
     def start(self):
         """
         Args:
         """
-        self.melon.init()
+        self.melon.autoInit()
         self.tasklistView.sortItems()
         self.calendarlistView.populate(self.melon.calendars.values())
         # QTimer.singleShot(200, self.sync)
 
     def sync(self):
         """
         Args:
```

### Comparing `melon_scheduler-0.1.2/melongui/taskitemdelegate.py` & `melon_scheduler-0.1.3/melongui/taskitemdelegate.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.2/melongui/tasklist.py` & `melon_scheduler-0.1.3/melongui/tasklist.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,90 +31,92 @@
         self.setDragEnabled(True)
         self.setVerticalScrollMode(QtWidgets.QListWidget.ScrollMode.ScrollPerPixel)
         self.itemChanged.connect(self.onItemChange)
         self._currentCalendarName = None
         self.addAddButton()
 
     def mouseDoubleClickEvent(self, event: QMouseEvent) -> None:
-        """
+        """Handles mouse double click
+
         Args:
             event (QMouseEvent): Argument
         """
         item = self.itemAt(event.position().toPoint())
         self.removeItemWidget(item)
         self.editItem(item)
 
     def addTask(self, task: Todo) -> OrderableTaskItem:
-        """
+        """Adds a Todo to the list
+
         Args:
             task (Todo): Argument
 
         Returns:
             (MyListWidgetItem):
         """
         item = OrderableTaskItem(task.summary)
         item.setData(UserRole, task)
         item.setFlags(item.flags() | Qt.ItemFlag.ItemIsEditable | Qt.ItemFlag.ItemIsDragEnabled)
         self.addItem(item)
         self.attachTaskWidget(item)
         return item
 
     def attachTaskWidget(self, item):
-        """
+        """For a given ListWidgetItem, attaches a task widget
+
         Args:
             item: Argument
         """
         widget = TaskOverlayWidget(parent=self)
         widget.completionBtn.clicked.connect(lambda: self.completeTask(item))
         self.setItemWidget(item, widget)
 
     def completeTask(self, item: QtWidgets.QListWidgetItem):
-        """
+        """Completes the task associated with the given item.
+
         Args:
             item (QListWidgetItem): Argument
         """
         task: Todo = item.data(UserRole)
         task.complete()
         self.takeItem(self.row(item))
 
     def addAddButton(self):
-        """
-        Args:
-        """
+        """Adds the task creation button at the bottom of the list."""
         self._addTaskItem = OrderableTaskItem("Add Task")
         self._addTaskItem.setData(Qt.ItemDataRole.EditRole, "add-task")
         self.addItem(self._addTaskItem)
         addButton = QtWidgets.QPushButton(QIcon.fromTheme("list-add"), "Add Task")
         addButton.clicked.connect(self.addEmptyTask)
         self.setItemWidget(self._addTaskItem, addButton)
 
     def setCalendarFilter(self, calendarName):
-        """
+        """Only shows tasks for the given calendar.
+
         Args:
             calendarName: Argument
         """
         for i in range(self.count()):
             item = self.item(i)
             if calendarName is not None and item.data(UserRole) is not None:
                 item.setHidden(item.data(UserRole).calendarName != calendarName)
             else:
                 item.setHidden(False)
         self.sortItems()
         self._currentCalendarName = calendarName
 
     def clearCalendarFilter(self):
-        """
-        Args:
-        """
+        """Clears the calendar filter, hence shows all tasks"""
         for i in range(self.count()):
             self.item(i).setHidden(False)
         self._currentCalendarName = None
 
     def onItemChange(self, item: QtWidgets.QListWidgetItem):
-        """
+        """Called when an item's value changes. Handles saving of the underlying object.
+
         Args:
             item (QListWidgetItem): Argument
         """
         todo: Todo = item.data(UserRole)
         if todo.calendarName is None:
             raise ValueError("The item's associated todo does not have a calendar.")
 
@@ -133,37 +135,35 @@
         todo.summary = text.strip()
         todo.save()
         logging.info("... saved!")
         self.melon.syncCalendar(self.melon.calendars[todo.calendarName])
         logging.debug("... and synced!")
 
     def addEmptyTask(self):
-        """
-        Args:
-        """
+        """Add an empty task to the bottom for editing and saving later."""
         if self._currentCalendarName is None:
             print("Please select a calendar first!")
             return
         calendar = self.melon.calendars[self._currentCalendarName]
         todo = calendar.createTodo()
         item = self.addTask(todo)
         self.sortItems()
         self.removeItemWidget(item)
         self.scrollToItem(item)
         self.editItem(item)
 
     def keyPressEvent(self, event: QKeyEvent) -> None:
-        """
+        """Handles keypresses.
+
         Args:
             event (QKeyEvent): Argument
         """
-        # if event.key() == Qt.Key.Key_Plus:
-        #     self.addEmptyTask()
         return super().keyPressEvent(event)
 
     def delegateEditorDestroyed(self, index):
-        """
+        """When the editor is destroyed, re-attach the item widget
+
         Args:
             index: Argument
         """
         if self.itemWidget(self.itemFromIndex(index)) is None:
             self.attachTaskWidget(self.itemFromIndex(index))
```

### Comparing `melon_scheduler-0.1.2/melongui/taskwidgets.py` & `melon_scheduler-0.1.3/melongui/taskwidgets.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.2/pyproject.toml` & `melon_scheduler-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "melon-scheduler"
-version = "0.1.2"
+version = "0.1.3"
 description = "Schedules Todos into your Calendar"
 authors = ["MrP01 <peter@waldert.at>"]
 readme = "README.md"
 packages = [
   { include = "melon" },
   { include = "melongui" },
 ]
@@ -12,27 +12,31 @@
 [tool.poetry.dependencies]
 python = "^3.10, <3.12"
 caldav = "^1.2.1"
 dateparser = "^1.1.8"
 tqdm = "^4.65.0"
 tomli = { version = "^2.0.1", python = "<3.11" }
 pyside6 = { version = "<6.5", optional = true }
+numba = { version = "^0.57.1", optional = true }
+matplotlib = { version = "^3.7.1", optional = true }
 
 [tool.poetry.extras]
 gui = ["pyside6"]
+numba = ["numba"]
+plots = ["matplotlib"]
 
 [tool.poetry.group.dev.dependencies]
-ipython = "^8.14.0"
 dill = "^0.3.6"
 interrogate = "^1.5.0"
-sphinx = "^7.0.1"
-recommonmark = "^0.7.1"
+invoke = "^2.1.3"
+ipython = "^8.14.0"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
-invoke = "^2.1.3"
+recommonmark = "^0.7.1"
+sphinx = "^7.0.1"
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 select = ["I001"]
@@ -40,10 +44,13 @@
 
 [tool.nitpick]
 style = ["github://MrP01/lint-me-now/nitpick-base-style.toml", "github://MrP01/lint-me-now/nitpick-python-style.toml"]
 
 [tool.interrogate]
 exclude = ["stuff"]
 
+[tool.coverage.run]
+omit = ["melon/scheduler/numba.py"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `melon_scheduler-0.1.2/PKG-INFO` & `melon_scheduler-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: melon-scheduler
-Version: 0.1.2
+Version: 0.1.3
 Summary: Schedules Todos into your Calendar
 Author: MrP01
 Author-email: peter@waldert.at
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
+Provides-Extra: numba
+Provides-Extra: plots
 Requires-Dist: caldav (>=1.2.1,<2.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0) ; extra == "plots"
+Requires-Dist: numba (>=0.57.1,<0.58.0) ; extra == "numba"
 Requires-Dist: pyside6 (<6.5) ; extra == "gui"
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Melon UI
```

