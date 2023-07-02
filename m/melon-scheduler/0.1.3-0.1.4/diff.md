# Comparing `tmp/melon_scheduler-0.1.3.tar.gz` & `tmp/melon_scheduler-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melon_scheduler-0.1.3.tar", max compression
+gzip compressed data, was "melon_scheduler-0.1.4.tar", max compression
```

## Comparing `melon_scheduler-0.1.3.tar` & `melon_scheduler-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2108 2023-06-27 22:02:19.451664 melon_scheduler-0.1.3/README.md
--rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.3/melon/__init__.py
--rw-r--r--   0        0        0     4581 2023-06-30 17:27:21.260501 melon_scheduler-0.1.3/melon/calendar.py
--rw-r--r--   0        0        0      554 2023-07-01 15:24:46.251746 melon_scheduler-0.1.3/melon/config.py
--rw-r--r--   0        0        0     8528 2023-07-01 21:33:46.176496 melon_scheduler-0.1.3/melon/melon.py
--rw-r--r--   0        0        0       91 2023-07-01 17:20:32.719529 melon_scheduler-0.1.3/melon/scheduler/__init__.py
--rw-r--r--   0        0        0     2130 2023-07-01 23:15:52.115000 melon_scheduler-0.1.3/melon/scheduler/base.py
--rw-r--r--   0        0        0      860 2023-07-01 20:04:35.083343 melon_scheduler-0.1.3/melon/scheduler/cpp.py
--rw-r--r--   0        0        0     4409 2023-07-01 20:04:02.823397 melon_scheduler-0.1.3/melon/scheduler/libcppscheduler.cpp
--rw-r--r--   0        0        0      444 2023-07-01 19:54:02.564583 melon_scheduler-0.1.3/melon/scheduler/libcppscheduler.pyi
--rw-r--r--   0        0        0      444 2023-07-01 14:38:21.981201 melon_scheduler-0.1.3/melon/scheduler/libscheduler.pyi
--rw-r--r--   0        0        0     3728 2023-07-01 17:33:44.781423 melon_scheduler-0.1.3/melon/scheduler/libscheduler.rs
--rw-r--r--   0        0        0     4514 2023-07-01 22:10:30.415308 melon_scheduler-0.1.3/melon/scheduler/numba.py
--rw-r--r--   0        0        0     6077 2023-07-01 22:58:26.628198 melon_scheduler-0.1.3/melon/scheduler/purepython.py
--rw-r--r--   0        0        0      866 2023-07-01 17:30:04.006010 melon_scheduler-0.1.3/melon/scheduler/rust.py
--rw-r--r--   0        0        0     6768 2023-07-01 22:26:24.282641 melon_scheduler-0.1.3/melon/todo.py
--rw-r--r--   0        0        0     1502 2023-07-01 22:38:29.259935 melon_scheduler-0.1.3/melon/visualise.py
--rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.3/melongui/__init__.py
--rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.3/melongui/assets/complete.png
--rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.3/melongui/assets/complete.svg
--rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.3/melongui/calendarlist.py
--rw-r--r--   0        0        0     4886 2023-06-30 17:10:21.279889 melon_scheduler-0.1.3/melongui/mainwindow.py
--rw-r--r--   0        0        0     5980 2023-06-27 19:31:46.233422 melon_scheduler-0.1.3/melongui/taskitemdelegate.py
--rw-r--r--   0        0        0     5783 2023-07-01 22:05:47.643986 melon_scheduler-0.1.3/melongui/tasklist.py
--rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.3/melongui/taskwidgets.py
--rw-r--r--   0        0        0     1257 2023-07-01 23:23:50.324341 melon_scheduler-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 melon_scheduler-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2279 2023-07-02 11:26:12.884681 melon_scheduler-0.1.4/README.md
+-rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.4/melon/__init__.py
+-rw-r--r--   0        0        0     4581 2023-06-30 17:27:21.260501 melon_scheduler-0.1.4/melon/calendar.py
+-rw-r--r--   0        0        0      681 2023-07-02 11:05:41.555029 melon_scheduler-0.1.4/melon/config.py
+-rw-r--r--   0        0        0     8578 2023-07-02 11:45:02.258976 melon_scheduler-0.1.4/melon/melon.py
+-rw-r--r--   0        0        0       91 2023-07-01 17:20:32.719529 melon_scheduler-0.1.4/melon/scheduler/__init__.py
+-rw-r--r--   0        0        0     2429 2023-07-02 10:51:28.366522 melon_scheduler-0.1.4/melon/scheduler/base.py
+-rw-r--r--   0        0        0      970 2023-07-02 12:20:57.232115 melon_scheduler-0.1.4/melon/scheduler/cpp.py
+-rw-r--r--   0        0        0     3714 2023-07-02 12:02:14.719308 melon_scheduler-0.1.4/melon/scheduler/libcppscheduler.cpp
+-rw-r--r--   0        0        0      444 2023-07-01 19:54:02.564583 melon_scheduler-0.1.4/melon/scheduler/libcppscheduler.pyi
+-rw-r--r--   0        0        0      444 2023-07-01 14:38:21.981201 melon_scheduler-0.1.4/melon/scheduler/libscheduler.pyi
+-rw-r--r--   0        0        0     3728 2023-07-01 17:33:44.781423 melon_scheduler-0.1.4/melon/scheduler/libscheduler.rs
+-rw-r--r--   0        0        0     4515 2023-07-02 11:59:28.735931 melon_scheduler-0.1.4/melon/scheduler/numba.py
+-rw-r--r--   0        0        0     6140 2023-07-02 11:49:50.126459 melon_scheduler-0.1.4/melon/scheduler/purepython.py
+-rw-r--r--   0        0        0      974 2023-07-02 12:20:39.156160 melon_scheduler-0.1.4/melon/scheduler/rust.py
+-rw-r--r--   0        0        0     6792 2023-07-02 11:45:14.654954 melon_scheduler-0.1.4/melon/todo.py
+-rw-r--r--   0        0        0     1605 2023-07-02 11:27:59.016568 melon_scheduler-0.1.4/melon/visualise.py
+-rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.4/melongui/__init__.py
+-rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.4/melongui/assets/complete.png
+-rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.4/melongui/assets/complete.svg
+-rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.4/melongui/calendarlist.py
+-rw-r--r--   0        0        0     4749 2023-07-02 11:46:56.334773 melon_scheduler-0.1.4/melongui/mainwindow.py
+-rw-r--r--   0        0        0     5948 2023-07-02 11:46:31.918816 melon_scheduler-0.1.4/melongui/taskitemdelegate.py
+-rw-r--r--   0        0        0     5793 2023-07-02 11:46:43.370796 melon_scheduler-0.1.4/melongui/tasklist.py
+-rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.4/melongui/taskwidgets.py
+-rw-r--r--   0        0        0     1354 2023-07-02 12:21:37.564015 melon_scheduler-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 melon_scheduler-0.1.4/PKG-INFO
```

### Comparing `melon_scheduler-0.1.3/README.md` & `melon_scheduler-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 Another challenge is to encode task dependencies i.e. task B requiring the completion of task A beforehand.
 
 Coding-wise this will include the algorithm itself, appropriate configuration and furthermore, I would like to integrate the system with a CalDAV endpoint for use with my personal calendar, making it accessible through a GUI (separated from the Python interface, so that one would be able to run the algorithm without).
 Of course there will be tests and documentation on how to set things up, use the library on its own and how to install the GUI application.
 An extension would be for the scheduler to learn about task properties based on user behaviour when rescheduling, etc. (detecting procrastination of an important task) and perhaps optimising suggestions based on that.
 
 As performance might become an issue for MCMC, we will attempt the use of low-level languages such as C++ in combination with tools such as pybind11, to outsource short performance-critical code sections away from Python to another language?
+
+The task check icon is the logo of the \textit{Tasks.org} Free and Open Source Android App, which may be found [here](https://github.com/tasks/tasks/tree/main/graphics).
```

### Comparing `melon_scheduler-0.1.3/melon/calendar.py` & `melon_scheduler-0.1.4/melon/calendar.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.3/melon/config.py` & `melon_scheduler-0.1.4/melon/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,12 +4,21 @@
 try:
     import tomllib
 except ImportError:  # pragma: no cover
     import tomli as tomllib  # pragma: no cover
 
 CONFIG_FOLDER = pathlib.Path.home() / ".config" / "melon"
 CONFIG_FOLDER.mkdir(exist_ok=True)
+CONFIG_PATH = CONFIG_FOLDER / "config.toml"
 
 CONFIG = {"client": {"url": "http://localhost:8000/dav/user/calendars/", "username": None, "password": None}}
-if (CONFIG_FOLDER / "config.toml").exists():
-    with open(CONFIG_FOLDER / "config.toml", "rb") as f:
-        CONFIG = tomllib.load(f)
+
+
+def load_config():
+    """Loads, or re-loads, the configuration file."""
+    global CONFIG
+    if CONFIG_PATH.exists():
+        with open(CONFIG_PATH, "rb") as f:
+            CONFIG = tomllib.load(f)
+
+
+load_config()
```

### Comparing `melon_scheduler-0.1.3/melon/melon.py` & `melon_scheduler-0.1.4/melon/melon.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,37 +30,39 @@
     HIDDEN_CALENDARS = ("calendar", None)
 
     def __init__(
         self,
         url=CONFIG["client"]["url"],
         username=CONFIG["client"]["username"],
         password=CONFIG["client"]["password"],
+        maxCalendars: int | None = None,
     ) -> None:
         """Initialises the Melon client
 
         Args:
             url (str, optional): URL to the CalDAV server. Defaults to CONFIG["client"]["url"].
             username (str, optional): Username. Defaults to CONFIG["client"]["username"].
             password (str, optional): Password. Defaults to CONFIG["client"]["password"].
+            maxCalendars (int, optional): the highest number of calendars to load. Useful for testing.
         """
         self.client = caldav.DAVClient(url=url, username=username, password=password)
         self.calendars: dict[str, Calendar] = {}
         self.principal = None
-        self.max_calendars: int | None = None  # the highest number of calendars to load. Useful for testing.
+        self.maxCalendars: int | None = maxCalendars
 
     def connect(self):
         """
         Args:
         """
         self.principal = self.client.principal()
         logging.info("Obtained principal")
 
         all_calendars = self.principal.calendars()
-        if self.max_calendars is not None:
-            all_calendars = all_calendars[: self.max_calendars]
+        if self.maxCalendars is not None:
+            all_calendars = all_calendars[: self.maxCalendars]
         self.calendars = {cal.name: Calendar(cal) for cal in all_calendars if cal.name not in self.HIDDEN_CALENDARS}
         logging.info(f"Obtained {len(self.calendars)} calendars")
 
     def _load_syncable_tasks(self, calendar):
         """
         Args:
             calendar: Argument
@@ -102,15 +104,15 @@
         with open(CONFIG_FOLDER / "synctokens.json") as f:
             data = json.load(f)
         for file in CONFIG_FOLDER.glob("*.dav"):
             name = file.stem  # filename corresponds to the calendar name
             self.calendars[name] = Calendar.loadFromFile(
                 self.client, self.principal, name, data[name]["token"], data[name]["url"]
             )
-            if self.max_calendars is not None and len(self.calendars) >= self.max_calendars:
+            if self.maxCalendars is not None and len(self.calendars) >= self.maxCalendars:
                 break
         logging.info(f"Loaded {len(self.calendars)} calendars from disk.")
         for calendar in self.calendars.values():
             self._load_syncable_tasks(calendar)
 
     def autoInit(self):
         """
@@ -207,15 +209,14 @@
             icalendar.Calendar: the calendar containing events (time slots) proposed for the completion of tasks
         """
         schedule = icalendar.Calendar()
         schedule.add("prodid", "-//Melon//example.org//")
         schedule.add("version", "2.0")
         todos = {t.uid: t for t in self.allTasks()}
         for uid, slot in scheduling.items():
-            print("Adding", uid)
             event = icalendar.Event(summary=todos[uid].summary)
             event.add("dtstart", slot.timestamp)
             event.add("dtend", slot.end)
             event.add("dtstamp", datetime.datetime.now())
             event.add("uid", uuid.uuid4())
             schedule.add_component(event)
         return schedule
```

### Comparing `melon_scheduler-0.1.3/melon/scheduler/base.py` & `melon_scheduler-0.1.4/melon/scheduler/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The scheduler algorithm"""
 import dataclasses
 import random
-from datetime import datetime, timedelta
+from datetime import datetime, time, timedelta
 from typing import Mapping
 
+START_OF_DAY = time(10, 0)
 DAY_LENGTH = 14
 INITIAL_TEMPERATURE = 0.2
 SWEEP_EXPONENT = -1.0
 
 
 @dataclasses.dataclass
 class Task:
@@ -50,14 +51,22 @@
         """Initialises the scheduler, working on a set of pre-defined tasks.
 
         Args:
             tasks (list[Task]): the tasks to be scheduled
         """
         self.tasks = tasks
 
+    def uidTaskMap(self) -> Mapping[str, Task]:
+        """Generates a dictionary for task lookup by UID.
+
+        Returns:
+            Mapping[str, Task]: the dictionary keyed by UID of each task.
+        """
+        return {task.uid: task for task in self.tasks}
+
     def schedule(self) -> Mapping[str, TimeSlot]:
         """Schedules the tasks using an MCMC procedure.
 
         Returns:
             Mapping[str, TimeSlot]: the resulting map of Tasks to TimeSlots
         """
         raise NotImplementedError()
```

### Comparing `melon_scheduler-0.1.3/melon/scheduler/cpp.py` & `melon_scheduler-0.1.4/melon/scheduler/cpp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """The scheduler algorithm"""
 import dataclasses
 import pathlib
 import sys
-from datetime import datetime, timedelta
+from datetime import date, datetime, timedelta
 from typing import Mapping
 
-sys.path.append(str(pathlib.Path(__file__).resolve().parent.parent.parent / "build"))
-import libcppscheduler
+try:
+    import libcppscheduler
+except ImportError:
+    sys.path.append(str(pathlib.Path(__file__).resolve().parent.parent.parent / "build"))
+    import libcppscheduler
 
-from .base import AbstractScheduler, TimeSlot
+from .base import START_OF_DAY, AbstractScheduler, TimeSlot
 
 
 class CppMCMCScheduler(AbstractScheduler):
     """Markov Chain Monte-Carlo Task Scheduler, implemented in Rust."""
 
     def schedule(self) -> Mapping[str, TimeSlot]:
         """Runs the Rust implementation of the scheduler.
 
         Returns:
             Mapping[str, TimeSlot]: the resulting schedule
         """
-        start = datetime.now()  # equivalent to t = 0 for libcppscheduler
+        start = datetime.combine(date.today(), START_OF_DAY)  # equivalent to t = 0 for libcppscheduler
         result = libcppscheduler.schedule(list(map(dataclasses.astuple, self.tasks)))
         return {t[0]: TimeSlot(start + timedelta(hours=t[1]), t[2]) for t in result}
```

### Comparing `melon_scheduler-0.1.3/melon/scheduler/libcppscheduler.cpp` & `melon_scheduler-0.1.4/melon/scheduler/libcppscheduler.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     auto last = spread[spread.size() - 1];
     auto first = spread[0];
     double timePenalty = last.start + last.duration - first.start;
     return timePenalty;
   }
 
   State permuteState() {
-    // memcpy(new_, state, tasks.size() * sizeof(size_t)); // copy current configuration to new one
     State proposal = state; // copy current state
     size_t cityA_ = rand() % tasks.size();
     size_t cityB_ = rand() % tasks.size();
     size_t cityA = std::min(cityA_, cityB_);
     size_t cityB = std::max(cityA_, cityB_);
     for (size_t i = 0; i <= cityB - cityA; i++)
       proposal[cityA + i] = state[cityB - i];
@@ -86,27 +85,15 @@
       State proposal = permuteState();
       double delta = getEnergy(proposal) - energy;
       double acceptanceProbability = std::min(1.0, std::exp(-delta / (energy * temperature)));
       if (((double)rand() / RAND_MAX) < acceptanceProbability) {
         state = proposal;
         energy += delta;
       }
-      // memcpy(state, proposal, tasks.size() * sizeof(size_t));
-      // std::cout << " -> " << acceptanceProbability << std::endl;
-      E_sum += energy;
-      E_squared_sum += energy * energy;
     }
-    double E_avg = E_sum / steps;
-    double E_var = E_squared_sum / steps - E_avg * E_avg;
-    // if (print_raw)
-    //   std::cout << temperature << ", " << E_avg << ", " << E_var << ", ";
-    // else {
-    //   std::cout << "Average energy for T = " << temperature << ": " << E_avg << std::endl;
-    //   std::cout << "Variance for       T = " << temperature << ": " << E_var << std::endl;
-    // }
   }
 
   void mcmcSimulate(size_t iterations) {
     for (size_t j = 0; j < iterations; j++) {
       mcmcSweep(tasks.size() * tasks.size());
       temperature = INITIAL_TEMPERATURE * std::pow(j + 1, -SWEEP_EXPONENT);
     }
@@ -117,15 +104,15 @@
   auto scheduler = MCMCScheduler();
   for (auto it = tasks.begin(); it != tasks.end(); ++it) {
     // unpack the tuple assuming it has exactly 4 elements (uid, duration, priority, location)
     auto tupleIterator = it->cast<py::tuple>().begin();
     auto task = Task{(tupleIterator++)->cast<std::string>(), (tupleIterator++)->cast<float>(),
         (tupleIterator++)->cast<int>(), tupleIterator->cast<int>()};
     scheduler.tasks.push_back(task);
-    std::cout << task.uid << ": " << task.duration << ", " << task.priority << ", " << task.location << std::endl;
+    // std::cout << task.uid << ": " << task.duration << ", " << task.priority << ", " << task.location << std::endl;
   }
   scheduler.initState();
   scheduler.mcmcSimulate(10);
   auto result = py::list();
   auto spread = scheduler.spreadTasks(scheduler.state);
   for (size_t i = 0; i < spread.size(); i++) {
     result.append(py::make_tuple(spread[i].uid, spread[i].start, spread[i].duration));
```

### Comparing `melon_scheduler-0.1.3/melon/scheduler/libscheduler.rs` & `melon_scheduler-0.1.4/melon/scheduler/libscheduler.rs`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.3/melon/scheduler/numba.py` & `melon_scheduler-0.1.4/melon/scheduler/numba.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """The scheduler algorithm"""
 import dataclasses
 import math
 import random
-from datetime import datetime, timedelta
+from datetime import date, datetime, timedelta
 from typing import Mapping, Sequence
 
 import numba
 from numba.typed.typedlist import List as NumbaList
 
-from .base import DAY_LENGTH, INITIAL_TEMPERATURE, SWEEP_EXPONENT, AbstractScheduler, TimeSlot
+from .base import DAY_LENGTH, INITIAL_TEMPERATURE, START_OF_DAY, SWEEP_EXPONENT, AbstractScheduler, TimeSlot
 
 State = list[int]
 
 
 @numba.njit()
 def spreadTasks(tasks: Sequence[tuple[str, float, int, int]]) -> Sequence[tuple[str, float, float]]:
     """Spreads the given list of tasks across the available slots in the calendar, in order.
@@ -107,23 +107,22 @@
     Returns:
         Sequence[tuple[str, float, float]]: vector of allocated timeslots (uid, timestamp, duration)
     """
     state = list(range(len(tasks)))
     for k in range(1, 11):
         temperature = INITIAL_TEMPERATURE * k**SWEEP_EXPONENT
         state = mcmcSweep(tasks, state, temperature)
-    print("Final State", state)
     return spreadTasks([tasks[i] for i in state])
 
 
 class NumbaMCMCScheduler(AbstractScheduler):
     """Markov Chain Monte-Carlo Task Scheduler, implemented in Python with numba speed-up."""
 
     def schedule(self) -> Mapping[str, TimeSlot]:
         """Runs the Rust implementation of the scheduler.
 
         Returns:
             Mapping[str, TimeSlot]: the resulting schedule
         """
-        start = datetime.now()  # equivalent to t = 0 for libscheduler
+        start = datetime.combine(date.today(), START_OF_DAY)  # equivalent to t = 0
         result = schedule(NumbaList(map(dataclasses.astuple, self.tasks)))
         return {t[0]: TimeSlot(start + timedelta(hours=t[1]), t[2]) for t in result}
```

### Comparing `melon_scheduler-0.1.3/melon/scheduler/purepython.py` & `melon_scheduler-0.1.4/melon/scheduler/purepython.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """The scheduler algorithm"""
+import logging
 import math
 import random
-from datetime import date, datetime, time, timedelta
+from datetime import date, datetime, timedelta
 from typing import Iterable, Mapping
 
-
-from .base import DAY_LENGTH, INITIAL_TEMPERATURE, SWEEP_EXPONENT, AbstractScheduler, Task, TimeSlot
+from .base import DAY_LENGTH, INITIAL_TEMPERATURE, START_OF_DAY, SWEEP_EXPONENT, AbstractScheduler, Task, TimeSlot
 
 
 class AvailabilityManager:
     """This class manages the user's availability in a calendar."""
 
     def __init__(self) -> None:
         """Initialises the availability manager according to defaults."""
-        self.startOfDay = time(10, 0)  # start at 10am
+        self.startOfDay = START_OF_DAY  # start at 10am
         self.defaultDayLength = DAY_LENGTH  # going all the way to 2am
 
     def startingSlot(self) -> TimeSlot:
         """Starting slot, starting at 10am today
 
         Returns:
             TimeSlot: the first working slot
@@ -74,15 +74,15 @@
         Args:
             tasks (list[Task]): the tasks to be scheduled
         """
         super().__init__(tasks)
         self.availability = AvailabilityManager()
         self.state = tuple(range(len(self.tasks)))  # initialise in order
         self.temperature = 1.0
-        self._log = []
+        self.energyLog = []
 
     def permuteState(self) -> State:
         """Proposes a new state to use instead of the old state.
 
         Returns:
             State: the new state, a list of indices within self.tasks representing traversal order
         """
@@ -133,20 +133,20 @@
             if random.random() < acceptanceProbability:
                 self.state = newState
                 energy += delta
             E_sum += energy
             E_squared_sum += energy**2
         E_avg = E_sum / steps
         E_var = E_squared_sum / steps - E_avg**2
-        self._log.append((self.temperature, E_avg, E_var))
+        self.energyLog.append((self.temperature, E_avg, E_var))
 
     def schedule(self) -> Mapping[str, TimeSlot]:
         """Schedules the tasks using an MCMC procedure.
 
         Returns:
             Mapping[str, TimeSlot]: the resulting map of Tasks to TimeSlots
         """
         for k in range(1, 11):
             self.temperature = INITIAL_TEMPERATURE * k**SWEEP_EXPONENT
             self.mcmcSweep()
-        print("Final State", self.state)
+        logging.info("Final State of the MCMC simulation", self.state)
         return dict(self.availability.spreadTasks(self.tasks[i] for i in self.state))
```

### Comparing `melon_scheduler-0.1.3/melon/scheduler/rust.py` & `melon_scheduler-0.1.4/melon/scheduler/rust.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """The scheduler algorithm"""
 import dataclasses
 import pathlib
 import sys
-from datetime import datetime, timedelta
+from datetime import date, datetime, timedelta
 from typing import Mapping
 
-sys.path.append(str(pathlib.Path(__file__).resolve().parent.parent.parent / "target" / "release"))
-import libscheduler
+try:
+    import libscheduler
+except ImportError:
+    sys.path.append(str(pathlib.Path(__file__).resolve().parent.parent.parent / "target" / "release"))
+    import libscheduler
 
-from .base import AbstractScheduler, TimeSlot
+
+from .base import START_OF_DAY, AbstractScheduler, TimeSlot
 
 
 class RustyMCMCScheduler(AbstractScheduler):
     """Markov Chain Monte-Carlo Task Scheduler, implemented in Rust."""
 
     def schedule(self) -> Mapping[str, TimeSlot]:
         """Runs the Rust implementation of the scheduler.
 
         Returns:
             Mapping[str, TimeSlot]: the resulting schedule
         """
-        start = datetime.now()  # equivalent to t = 0 for libscheduler
+        start = datetime.combine(date.today(), START_OF_DAY)  # equivalent to t = 0 for libscheduler
         result = libscheduler.schedule(list(map(dataclasses.astuple, self.tasks)))
         return {t[0]: TimeSlot(start + timedelta(hours=t[1]), t[2]) for t in result}
```

### Comparing `melon_scheduler-0.1.3/melon/todo.py` & `melon_scheduler-0.1.4/melon/todo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module contains the Todo class."""
 import datetime
+import logging
 import re
 from typing import Literal
 
 import caldav
 import caldav.lib.url
 import icalendar.cal
 import icalendar.prop
@@ -151,15 +152,15 @@
             handle_rrule (bool, optional): Argument
                 (default is True)
             rrule_mode (Literal['safe', 'this_and_future'], optional): Argument
                 (default is 'safe')
 
         """
         super().complete(completion_timestamp, handle_rrule, rrule_mode)
-        print("Task completed.")
+        logging.info("Task completed.")
 
     def isTodo(self) -> bool:
         """
         Returns:
             bool: whether this object is a VTODO or not (i.e. an event or journal).
         """
         return "vtodo" in self.vobject_instance.contents
@@ -173,15 +174,15 @@
         assert self.uid is not None
         location = 0
         if "home" in self.summary:
             location = 1
         elif "work" in self.summary:
             location = 2
         match = re.search(r"\b([\d\,\.])+h\b", self.summary)
-        hours = float(match.group(1)) if match else 1
+        hours = float(match.group(1)) if match else 1.0
         return Task(self.uid, hours, self.priority, location)
 
     def __lt__(self, other: "Todo") -> bool:
         """Compares two todos in terms of ordering
 
         Args:
             other (Todo): the instance to compare with
```

### Comparing `melon_scheduler-0.1.3/melon/visualise.py` & `melon_scheduler-0.1.4/melon/visualise.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""A collection of (quality measure) visualisation helpers."""
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 
 
 def priorityChart(data, title):
     """Plots a helpful priority chart
@@ -23,15 +24,15 @@
         ax.plot(angles, d, "o-", linewidth=2, color=c)
         ax.fill(angles, d, alpha=0.25, color=c)
         ax.set_thetagrids(angles * 180 / np.pi, labels)
         ax.set_ylim(0, 1.0)
         ax.grid(True)
 
 
-def plotConvergence(data: np.ndarray, filename: str):
+def plotConvergence(data: np.ndarray, filename: str | None):
     """Plots convergence data to a file
 
     Args:
         data (np.array): data of temp, E_avg, E_var
         filename (str): path to file
     """
     fig = plt.figure()
@@ -39,8 +40,9 @@
     axes.plot(data[:, 1])
     axes.set_xlabel("Iteration")
     axes.set_ylabel("$E_{avg}$")
     axes: matplotlib.axes.Axes = fig.add_subplot(2, 1, 2)
     axes.plot(data[:, 2])
     axes.set_xlabel("Iteration")
     axes.set_ylabel("$E_{var}$")
-    fig.savefig(filename)  # type: ignore
+    if filename is not None:
+        fig.savefig(filename)  # type: ignore
```

### Comparing `melon_scheduler-0.1.3/melongui/assets/complete.png` & `melon_scheduler-0.1.4/melongui/assets/complete.png`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.3/melongui/assets/complete.svg` & `melon_scheduler-0.1.4/melongui/assets/complete.svg`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.3/melongui/calendarlist.py` & `melon_scheduler-0.1.4/melongui/calendarlist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.3/melongui/mainwindow.py` & `melon_scheduler-0.1.4/melongui/mainwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,28 +112,25 @@
             self.tasklistView.setCalendarFilter(item.text())
 
     def keyPressEvent(self, event: QKeyEvent):
         """
         Args:
             event (QKeyEvent): Argument
         """
-        # print("Key Event", event)
         if event.modifiers() == Qt.KeyboardModifier.ControlModifier:
             if event.key() == Qt.Key.Key_W:
                 self.close()
             elif event.key() == Qt.Key.Key_S:
                 self.sync()
             elif event.key() == Qt.Key.Key_H:
                 self.calendarlistView.setCurrentRow(0)
             elif event.key() == Qt.Key.Key_Plus:
                 self.tasklistView.addEmptyTask()
             elif event.key() == Qt.Key.Key_Return:
                 self.threadPool.start(self.melon.scheduleAllAndExport)
-        # if Qt.Key.Key_A <= event.key() <= Qt.Key.Key_Z:
-        #     self.searchWidget.setFocus()
         return super().keyPressEvent(event)
 
     def showInfoMessage(self, msg: str):
         """
         Args:
             msg (str): Argument
         """
```

### Comparing `melon_scheduler-0.1.3/melongui/taskitemdelegate.py` & `melon_scheduler-0.1.4/melongui/taskitemdelegate.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         Returns:
             Callable: the event handler
         """
 
         def actualHandler():
             """I am called to perform the actual parsing."""
             text = edit.text()
-            print("Edit", text)
             results = dateparser.search.search_dates(text)
             if results:
                 token, stamp = results[0]
                 label.setText(stamp.strftime("%d.%m.%Y"))
             else:
                 label.clear()
```

### Comparing `melon_scheduler-0.1.3/melongui/tasklist.py` & `melon_scheduler-0.1.4/melongui/tasklist.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         logging.info("... saved!")
         self.melon.syncCalendar(self.melon.calendars[todo.calendarName])
         logging.debug("... and synced!")
 
     def addEmptyTask(self):
         """Add an empty task to the bottom for editing and saving later."""
         if self._currentCalendarName is None:
-            print("Please select a calendar first!")
+            logging.warning("Please select a calendar first!")
             return
         calendar = self.melon.calendars[self._currentCalendarName]
         todo = calendar.createTodo()
         item = self.addTask(todo)
         self.sortItems()
         self.removeItemWidget(item)
         self.scrollToItem(item)
```

### Comparing `melon_scheduler-0.1.3/melongui/taskwidgets.py` & `melon_scheduler-0.1.4/melongui/taskwidgets.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.3/pyproject.toml` & `melon_scheduler-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [tool.poetry]
 name = "melon-scheduler"
-version = "0.1.3"
+version = "0.1.4"
 description = "Schedules Todos into your Calendar"
-authors = ["MrP01 <peter@waldert.at>"]
+authors = ["redacted"]
 readme = "README.md"
-packages = [
-  { include = "melon" },
-  { include = "melongui" },
-]
+packages = [{ include = "melon" }, { include = "melongui" }]
 
 [tool.poetry.dependencies]
 python = "^3.10, <3.12"
 caldav = "^1.2.1"
 dateparser = "^1.1.8"
 tqdm = "^4.65.0"
 tomli = { version = "^2.0.1", python = "<3.11" }
@@ -39,15 +36,20 @@
 
 [tool.ruff]
 line-length = 120
 select = ["I001"]
 exclude = [".git", "**/__pycache__"]
 
 [tool.nitpick]
-style = ["github://MrP01/lint-me-now/nitpick-base-style.toml", "github://MrP01/lint-me-now/nitpick-python-style.toml"]
+style = [
+  "github://MrP01/lint-me-now/nitpick-base-style.toml",
+  "github://MrP01/lint-me-now/nitpick-python-style.toml",
+  "github://MrP01/lint-me-now/nitpick-c-cpp-style.toml",
+  "github://MrP01/lint-me-now/nitpick-latex-style.toml"
+]
 
 [tool.interrogate]
 exclude = ["stuff"]
 
 [tool.coverage.run]
 omit = ["melon/scheduler/numba.py"]
```

### Comparing `melon_scheduler-0.1.3/PKG-INFO` & `melon_scheduler-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: melon-scheduler
-Version: 0.1.3
+Version: 0.1.4
 Summary: Schedules Todos into your Calendar
-Author: MrP01
-Author-email: peter@waldert.at
+Author: redacted
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
 Provides-Extra: numba
 Provides-Extra: plots
@@ -36,7 +35,9 @@
 
 Coding-wise this will include the algorithm itself, appropriate configuration and furthermore, I would like to integrate the system with a CalDAV endpoint for use with my personal calendar, making it accessible through a GUI (separated from the Python interface, so that one would be able to run the algorithm without).
 Of course there will be tests and documentation on how to set things up, use the library on its own and how to install the GUI application.
 An extension would be for the scheduler to learn about task properties based on user behaviour when rescheduling, etc. (detecting procrastination of an important task) and perhaps optimising suggestions based on that.
 
 As performance might become an issue for MCMC, we will attempt the use of low-level languages such as C++ in combination with tools such as pybind11, to outsource short performance-critical code sections away from Python to another language?
 
+The task check icon is the logo of the \textit{Tasks.org} Free and Open Source Android App, which may be found [here](https://github.com/tasks/tasks/tree/main/graphics).
+
```

