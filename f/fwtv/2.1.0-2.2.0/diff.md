# Comparing `tmp/fwtv-2.1.0.tar.gz` & `tmp/fwtv-2.2.0.tar.gz`

## Comparing `fwtv-2.1.0.tar` & `fwtv-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 fwtv-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/__init__.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/main.py
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/verifier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/objects/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/objects/async_converter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/widgets/__init__.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/widgets/login_widget.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/widgets/settings_widget.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/widgets/table_widget.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 fwtv-2.1.0/src/fwtv/widgets/working_time_widget.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 fwtv-2.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fwtv-2.1.0/LICENSE
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fwtv-2.1.0/README.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 fwtv-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 fwtv-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 fwtv-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/__init__.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/main.py
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/verifier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/objects/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/objects/async_converter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/widgets/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/widgets/login_widget.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/widgets/settings_widget.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/widgets/table_widget.py
+-rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 fwtv-2.2.0/src/fwtv/widgets/working_time_widget.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 fwtv-2.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fwtv-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fwtv-2.2.0/README.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 fwtv-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 fwtv-2.2.0/PKG-INFO
```

### Comparing `fwtv-2.1.0/CHANGELOG.md` & `fwtv-2.2.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # Changelog
 All notable changes to fwtv module will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0)
 
+## [2.2.0] - 2023-08-07
+
+## Added
+
+- extra window showing all attendances that lead to this verification failure
+- tolerance can be configured though input now
+
 ## [2.1.0] - 2023-04-08
 
 ### Changed
 
 - Choose between teams and single employee and made combobox editable
 - Renamed labels to `Affected Day(s)`, `Cumulated Break` and `Cumulated Attendance`
 - Avoid duplications by resetting `current_attendances` list
```

### Comparing `fwtv-2.1.0/src/fwtv/main.py` & `fwtv-2.2.0/src/fwtv/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 from factorialhr import endpoints
 from PySide6.QtWidgets import QApplication
 from PySide6.QtWidgets import QMessageBox
 from PySide6.QtWidgets import QVBoxLayout
 from PySide6.QtWidgets import QWidget
 
+import fwtv
 from fwtv.objects import async_converter
 from fwtv.widgets import login_widget
 from fwtv.widgets import working_time_widget
 
 
 class MainWindow(QWidget):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.setWindowTitle("Factorial working time verification")
+        self.setWindowTitle(f"Factorial working time verification - version {fwtv.__version__}")
         self.qv = QVBoxLayout()
         self.login = login_widget.LoginWidget(self)
         self.qv.addWidget(self.login)
 
         self.verification_widget = working_time_widget.WorkingTimeWidget(self)
         self.qv.addWidget(self.verification_widget)
```

### Comparing `fwtv-2.1.0/src/fwtv/verifier.py` & `fwtv-2.2.0/src/fwtv/verifier.py`

 * *Files identical despite different names*

### Comparing `fwtv-2.1.0/src/fwtv/objects/async_converter.py` & `fwtv-2.2.0/src/fwtv/objects/async_converter.py`

 * *Files identical despite different names*

### Comparing `fwtv-2.1.0/src/fwtv/widgets/login_widget.py` & `fwtv-2.2.0/src/fwtv/widgets/login_widget.py`

 * *Files identical despite different names*

### Comparing `fwtv-2.1.0/src/fwtv/widgets/settings_widget.py` & `fwtv-2.2.0/src/fwtv/widgets/settings_widget.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from PySide6.QtCore import QDate
 from PySide6.QtWidgets import QComboBox
 from PySide6.QtWidgets import QDateEdit
+from PySide6.QtWidgets import QDoubleSpinBox
 from PySide6.QtWidgets import QHBoxLayout
 from PySide6.QtWidgets import QLabel
 from PySide6.QtWidgets import QSizePolicy
 from PySide6.QtWidgets import QWidget
 
 
 class TeamOrEmployeeSettingWidget(QWidget):
@@ -33,21 +34,41 @@
         self.date.setCalendarPopup(True)
         self.date.setDisplayFormat("yyyy-MM-dd")
         self.qh.addWidget(self.date)
 
         self.setLayout(self.qh)
 
 
+class ToleranceWidget(QWidget):
+    def __init__(self, default: int, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.qh = QHBoxLayout(self)
+        self.label = QLabel("Tolerance", self)
+        self.qh.addWidget(self.label)
+
+        self.tolerance = QDoubleSpinBox(self)
+        self.tolerance.setSingleStep(1)
+        self.tolerance.setDecimals(0)
+        self.tolerance.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Minimum)
+        self.tolerance.setValue(default)
+        self.qh.addWidget(self.tolerance)
+
+        self.setLayout(self.qh)
+
+
 class SettingsWidget(QWidget):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.qh = QHBoxLayout(self)
         self.team_selector = TeamOrEmployeeSettingWidget(self)
         self.qh.addWidget(self.team_selector)
 
         self.start_picker = DateSettingWidget("Start on", QDate.currentDate().addMonths(-1), self)
         self.qh.addWidget(self.start_picker)
 
         self.end_picker = DateSettingWidget("End on", QDate.currentDate(), self)
         self.qh.addWidget(self.end_picker)
 
+        self.tolerance_selector = ToleranceWidget(1)
+        self.qh.addWidget(self.tolerance_selector)
+
         self.setLayout(self.qh)
```

### Comparing `fwtv-2.1.0/src/fwtv/widgets/working_time_widget.py` & `fwtv-2.2.0/src/fwtv/widgets/working_time_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 from fwtv import verifier
 from fwtv.widgets import settings_widget
 from fwtv.widgets import table_widget
 
 
 def get_errors(
-    start: datetime.date, end: datetime.date, attendances: list[models.Attendance], employees: list[models.Employee]
+    start: datetime.date,
+    end: datetime.date,
+    attendances: list[models.Attendance],
+    employees: list[models.Employee],
+    tolerance: int,
 ) -> tuple[dict[str, list[str]], dict[str, list[verifier.Error]]]:
     preconditions: dict[str, list[str]] = collections.defaultdict(list)
     employee_errors: dict[str, list[verifier.Error]] = collections.defaultdict(list)
     for employee in employees:
         name = employee.full_name
         employee_attendances: list[verifier.Attendance] = []
 
@@ -38,21 +42,21 @@
                 )
                 employee_attendances.append(a)
             except ValueError as e:
                 preconditions[name].append(str(e))
                 continue
 
         errors = verifier.verify_attendances(employee_attendances)
-        # ignore all errors where the time attended is 1 min above the limit, as factorial's automated time tracking
-        # is not precises enough
+        # ignore all errors where the time attended is the tolerance above the limit, as factorial's automated time
+        # tracking is not precises enough
         errors = [
             e
             for e in errors
-            if e.time_attended != datetime.timedelta(hours=6, minutes=1)
-            and e.time_attended != datetime.timedelta(hours=9, minutes=1)
+            if e.time_attended > datetime.timedelta(hours=6, minutes=tolerance)
+            and e.time_attended > datetime.timedelta(hours=9, minutes=tolerance)
         ]
         if errors:
             employee_errors[name] = errors
     return preconditions, employee_errors
 
 
 class WorkingTimeWidget(QWidget):
@@ -74,14 +78,15 @@
         self.qv.addWidget(self.failures_table)
 
         self.setLayout(self.qv)
 
         self.settings_widget.team_selector.selector.currentIndexChanged.connect(self.update_data)
         self.settings_widget.start_picker.date.dateChanged.connect(self.update_data)
         self.settings_widget.end_picker.date.dateChanged.connect(self.update_data)
+        self.settings_widget.tolerance_selector.tolerance.valueChanged.connect(self.update_data)
 
         self.update_data()
 
     def set_data(
         self, teams: list[models.Team], attendances: list[models.Attendance], employees: list[models.Employee]
     ):
         self.attendances = attendances
@@ -112,19 +117,14 @@
             employees = [selection]
 
         preconditions, errors = get_errors(
             self.settings_widget.start_picker.date.date().toPython(),
             self.settings_widget.end_picker.date.date().toPython(),
             self.attendances,
             employees,
+            int(self.settings_widget.tolerance_selector.tolerance.value()),
         )
         entries = collections.defaultdict(list)
         for k in preconditions.keys():
             entries[k] = [preconditions[k]]
         self.preconditions_table.set_data(entries)
-        entries = collections.defaultdict(list)
-        for name, error in errors.items():
-            for e in error:
-                affected_days = [str(day) for day in e.days_affected]
-                affected_days.sort()
-                entries[name].append([", ".join(affected_days), e.reason, str(e.break_time), str(e.time_attended)])
-        self.failures_table.set_data(entries)
+        self.failures_table.set_data(errors)
```

### Comparing `fwtv-2.1.0/.gitignore` & `fwtv-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fwtv-2.1.0/LICENSE` & `fwtv-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fwtv-2.1.0/README.md` & `fwtv-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fwtv-2.1.0/pyproject.toml` & `fwtv-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fwtv-2.1.0/PKG-INFO` & `fwtv-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwtv
-Version: 2.1.0
+Version: 2.2.0
 Summary: Verification that attendances comply with german rules. Also provide an integration to the api of FactorialHR
 Project-URL: Homepage, https://github.com/leon1995/fwtv
 Project-URL: Bug Tracker, https://github.com/leon1995/fwtv/issues
 Author-email: Leon Budnick <y6q6ea9w@mail-proxy.org>
 License-File: LICENSE
 Keywords: FactorialHR,HR,Working time
 Classifier: Development Status :: 5 - Production/Stable
```

