# Comparing `tmp/ieeh-power-system-data-model-1.5.0.tar.gz` & `tmp/ieeh-power-system-data-model-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieeh-power-system-data-model-1.5.0.tar", last modified: Thu Jul  6 07:22:52 2023, max compression
+gzip compressed data, was "ieeh-power-system-data-model-1.5.1.tar", last modified: Tue Jul 25 09:54:58 2023, max compression
```

## Comparing `ieeh-power-system-data-model-1.5.0.tar` & `ieeh-power-system-data-model-1.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      348 2023-07-06 07:21:54.195411 ieeh-power-system-data-model-1.5.0/AUTHORS.md
--rw-r--r--   0        0        0     1568 2023-07-06 07:21:54.195411 ieeh-power-system-data-model-1.5.0/LICENSE
--rw-r--r--   0        0        0     2641 2023-07-06 07:21:54.195411 ieeh-power-system-data-model-1.5.0/README.md
--rw-r--r--   0        0        0        1 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/__init__.py
--rw-r--r--   0        0        0     1367 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/base.py
--rw-r--r--   0        0        0      615 2023-07-06 07:22:44.064108 ieeh-power-system-data-model-1.5.0/psdm/meta.py
--rw-r--r--   0        0        0        1 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/__init__.py
--rw-r--r--   0        0        0     1080 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/active_power.py
--rw-r--r--   0        0        0     3687 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/case.py
--rw-r--r--   0        0        0     5311 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/controller.py
--rw-r--r--   0        0        0      432 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/external_grid.py
--rw-r--r--   0        0        0      539 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/load.py
--rw-r--r--   0        0        0      889 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/reactive_power.py
--rw-r--r--   0        0        0      367 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/transformer.py
--rw-r--r--   0        0        0        1 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/__init__.py
--rw-r--r--   0        0        0      491 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/active_power.py
--rw-r--r--   0        0        0     1956 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/branch.py
--rw-r--r--   0        0        0      337 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/characteristic.py
--rw-r--r--   0        0        0      364 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/coupler.py
--rw-r--r--   0        0        0      697 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/external_grid.py
--rw-r--r--   0        0        0      361 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/fuse.py
--rw-r--r--   0        0        0     4776 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/load.py
--rw-r--r--   0        0        0     1305 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/load_model.py
--rw-r--r--   0        0        0      320 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/node.py
--rw-r--r--   0        0        0      486 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/reactive_power.py
--rw-r--r--   0        0        0      363 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/switch.py
--rw-r--r--   0        0        0      699 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/topology.py
--rw-r--r--   0        0        0     2275 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/transformer.py
--rw-r--r--   0        0        0     1081 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/windings.py
--rw-r--r--   0        0        0        1 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology_case/__init__.py
--rw-r--r--   0        0        0      425 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology_case/case.py
--rw-r--r--   0        0        0      399 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology_case/element_state.py
--rw-r--r--   0        0        0     2680 2023-07-06 07:22:44.088109 ieeh-power-system-data-model-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1441 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_active_power.py
--rw-r--r--   0        0        0      659 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_branch.py
--rw-r--r--   0        0        0     8953 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_controller.py
--rw-r--r--   0        0        0     1449 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_reactive_power.py
--rw-r--r--   0        0        0     2336 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_topology_load.py
--rw-r--r--   0        0        0     3127 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      348 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/AUTHORS.md
+-rw-r--r--   0        0        0     1568 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2641 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/README.md
+-rw-r--r--   0        0        0        1 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/base.py
+-rw-r--r--   0        0        0      615 2023-07-25 09:54:49.864510 ieeh-power-system-data-model-1.5.1/psdm/meta.py
+-rw-r--r--   0        0        0        1 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/active_power.py
+-rw-r--r--   0        0        0     3687 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/case.py
+-rw-r--r--   0        0        0     5246 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/controller.py
+-rw-r--r--   0        0        0      432 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/external_grid.py
+-rw-r--r--   0        0        0      539 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/load.py
+-rw-r--r--   0        0        0      889 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/reactive_power.py
+-rw-r--r--   0        0        0      367 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/transformer.py
+-rw-r--r--   0        0        0        1 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/__init__.py
+-rw-r--r--   0        0        0      491 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/active_power.py
+-rw-r--r--   0        0        0     1956 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/branch.py
+-rw-r--r--   0        0        0      337 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/characteristic.py
+-rw-r--r--   0        0        0      364 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/coupler.py
+-rw-r--r--   0        0        0      697 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/external_grid.py
+-rw-r--r--   0        0        0      361 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/fuse.py
+-rw-r--r--   0        0        0     4776 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/load.py
+-rw-r--r--   0        0        0     1305 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/load_model.py
+-rw-r--r--   0        0        0      320 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/node.py
+-rw-r--r--   0        0        0      486 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/reactive_power.py
+-rw-r--r--   0        0        0      363 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/switch.py
+-rw-r--r--   0        0        0      699 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/topology.py
+-rw-r--r--   0        0        0     2275 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/transformer.py
+-rw-r--r--   0        0        0     1081 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology/windings.py
+-rw-r--r--   0        0        0        1 2023-07-25 09:53:54.259816 ieeh-power-system-data-model-1.5.1/psdm/topology_case/__init__.py
+-rw-r--r--   0        0        0      425 2023-07-25 09:53:54.263816 ieeh-power-system-data-model-1.5.1/psdm/topology_case/case.py
+-rw-r--r--   0        0        0      399 2023-07-25 09:53:54.263816 ieeh-power-system-data-model-1.5.1/psdm/topology_case/element_state.py
+-rw-r--r--   0        0        0     2680 2023-07-25 09:54:49.900510 ieeh-power-system-data-model-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1441 2023-07-25 09:53:54.263816 ieeh-power-system-data-model-1.5.1/tests/test_active_power.py
+-rw-r--r--   0        0        0      659 2023-07-25 09:53:54.263816 ieeh-power-system-data-model-1.5.1/tests/test_branch.py
+-rw-r--r--   0        0        0     8953 2023-07-25 09:53:54.263816 ieeh-power-system-data-model-1.5.1/tests/test_controller.py
+-rw-r--r--   0        0        0     1449 2023-07-25 09:53:54.263816 ieeh-power-system-data-model-1.5.1/tests/test_reactive_power.py
+-rw-r--r--   0        0        0     2336 2023-07-25 09:53:54.263816 ieeh-power-system-data-model-1.5.1/tests/test_topology_load.py
+-rw-r--r--   0        0        0     3127 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.5.1/PKG-INFO
```

### Comparing `ieeh-power-system-data-model-1.5.0/LICENSE` & `ieeh-power-system-data-model-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/README.md` & `ieeh-power-system-data-model-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/base.py` & `ieeh-power-system-data-model-1.5.1/psdm/base.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/meta.py` & `ieeh-power-system-data-model-1.5.1/psdm/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import typing as t
 import uuid
 
 import pydantic
 
 from psdm.base import Base
 
-VERSION = "1.5.0"
+VERSION = "1.5.1"
 
 
 class Meta(Base):
     version: t.ClassVar[str] = VERSION
     name: str
     date: datetime.date  # date of export
     id: uuid.UUID = pydantic.Field(default_factory=uuid.uuid4)  # noqa: A003
```

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/active_power.py` & `ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/active_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/case.py` & `ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/case.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/controller.py` & `ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # :author: Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
 import enum
-import typing as t
 
 import pydantic
 
 from psdm.base import Base
 from psdm.base import CosphiDir
 
 
@@ -33,84 +32,80 @@
     B = "B"
     C = "C"
     AB = "AB"
     BC = "BC"
     CA = "CA"
 
 
-class ControlType(Base):
-    control_strategy: t.ClassVar[ControlStrategy]
-
-
-class ControlQConst(ControlType):
+class ControlQConst(Base):
     # q-setpoint control mode
     q_set: float  # Setpoint of reactive power. Counted demand based.
 
-    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.Q_CONST
+    control_strategy: ControlStrategy = ControlStrategy.Q_CONST
 
 
-class ControlUConst(ControlType):
+class ControlUConst(Base):
     # u-setpoint control mode
     u_set: float = pydantic.Field(ge=0)  # Setpoint of voltage.
     u_meas_ref: ControlledVoltageRef = ControlledVoltageRef.POS_SEQ  # voltage reference
 
-    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.U_CONST
+    control_strategy: ControlStrategy = ControlStrategy.U_CONST
 
 
-class ControlTanphiConst(ControlType):
+class ControlTanphiConst(Base):
     # cos(phi) control mode
     cosphi_dir: CosphiDir
     cosphi: float = pydantic.Field(ge=0, le=1)  # cos(phi) for calculation of Q in relation to P.
 
-    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.TANPHI_CONST
+    control_strategy: ControlStrategy = ControlStrategy.TANPHI_CONST
 
 
-class ControlCosphiConst(ControlType):
+class ControlCosphiConst(Base):
     # cos(phi) control mode
     cosphi_dir: CosphiDir
     cosphi: float = pydantic.Field(ge=0, le=1)  # cos(phi) for calculation of Q in relation to P.
 
-    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.COSPHI_CONST
+    control_strategy: ControlStrategy = ControlStrategy.COSPHI_CONST
 
 
-class ControlCosphiP(ControlType):
+class ControlCosphiP(Base):
     # cos(phi(P)) control mode
     cosphi_ue: float = pydantic.Field(
         ge=0,
         le=1,
     )  # under excited: cos(phi) for calculation of Q in relation to P.
     cosphi_oe: float = pydantic.Field(
         ge=0,
         le=1,
     )  # over excited: cos(phi) for calculation of Q in relation to P.
     p_threshold_ue: float = pydantic.Field(le=0)  # under excited: threshold for P.
     p_threshold_oe: float = pydantic.Field(le=0)  # over excited: threshold for P.
 
-    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.COSPHI_P
+    control_strategy: ControlStrategy = ControlStrategy.COSPHI_P
 
 
-class ControlCosphiU(ControlType):
+class ControlCosphiU(Base):
     # cos(phi(U)) control mode
     cosphi_ue: float = pydantic.Field(
         ...,
         ge=0,
         le=1,
     )  # under excited: cos(phi) for calculation of Q in relation to P.
     cosphi_oe: float = pydantic.Field(
         ...,
         ge=0,
         le=1,
     )  # over excited: cos(phi) for calculation of Q in relation to P.
     u_threshold_ue: float = pydantic.Field(..., ge=0)  # under excited: threshold for U.
     u_threshold_oe: float = pydantic.Field(..., ge=0)  # over excited: threshold for U.
 
-    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.COSPHI_U
+    control_strategy: ControlStrategy = ControlStrategy.COSPHI_U
 
 
-class ControlQU(ControlType):
+class ControlQU(Base):
     # Q(U) characteristic control mode
     m_tg_2015: float = pydantic.Field(
         ...,
         ge=0,
     )  # Droop/Slope based on technical guideline VDE-AR-N 4120:2015: '%/kV'-value --> Q = m_% * Pr * dU_kV
     m_tg_2018: float = pydantic.Field(
         ...,
@@ -124,38 +119,50 @@
     u_deadband_low: float = pydantic.Field(
         ...,
         ge=0,
     )  # Width of lower deadband (U_Q0 - U_1_low): per unit value related to Un
     q_max_ue: float = pydantic.Field(..., ge=0)  # Under excited limit of Q: absolut value
     q_max_oe: float = pydantic.Field(..., ge=0)  # Over excited limit of Q: absolut value
 
-    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.Q_U
+    control_strategy: ControlStrategy = ControlStrategy.Q_U
 
 
 def validate_pos(value: float | None) -> float | None:
     if value is not None and value < 0:
         raise ValueError
 
     return value
 
 
-class ControlQP(ControlType):
+class ControlQP(Base):
     # Q(P) characteristic control mode
     q_p_characteristic_name: str
     q_max_ue: float | None = None  # Under excited limit of Q: absolut value
     q_max_oe: float | None = None  # Over excited limit of Q: absolut value
 
-    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.Q_P
+    control_strategy: ControlStrategy = ControlStrategy.Q_P
 
     @pydantic.field_validator("q_max_ue", mode="before")
     def validate_q_max_ue(cls, v: float | None) -> float | None:
         return validate_pos(v)
 
     @pydantic.field_validator("q_max_oe", mode="before")
     def validate_q_max_oe(cls, v: float | None) -> float | None:
         return validate_pos(v)
 
 
-class Controller(ControlType):
+ControlTypeType = (
+    ControlQConst
+    | ControlUConst
+    | ControlTanphiConst
+    | ControlCosphiConst
+    | ControlCosphiP
+    | ControlCosphiU
+    | ControlQU
+    | ControlQP
+)
+
+
+class Controller(Base):
     node_target: str  # the controlled node (which can be differ from node the load is connected to)
-    control_type: ControlType | None = None
+    control_type: ControlTypeType | None = None
     external_controller_name: str | None = None  # if external controller is specified --> name
```

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/load.py` & `ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/load.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/reactive_power.py` & `ieeh-power-system-data-model-1.5.1/psdm/steadystate_case/reactive_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/topology/branch.py` & `ieeh-power-system-data-model-1.5.1/psdm/topology/branch.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/topology/external_grid.py` & `ieeh-power-system-data-model-1.5.1/psdm/topology/external_grid.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/topology/load.py` & `ieeh-power-system-data-model-1.5.1/psdm/topology/load.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/topology/load_model.py` & `ieeh-power-system-data-model-1.5.1/psdm/topology/load_model.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/topology/topology.py` & `ieeh-power-system-data-model-1.5.1/psdm/topology/topology.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/topology/transformer.py` & `ieeh-power-system-data-model-1.5.1/psdm/topology/transformer.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/psdm/topology/windings.py` & `ieeh-power-system-data-model-1.5.1/psdm/topology/windings.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/pyproject.toml` & `ieeh-power-system-data-model-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "loguru",
     "pydantic>=2.0",
 ]
 description = "A data model for describing power systems"
 name = "ieeh-power-system-data-model"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.5.0"
+version = "1.5.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/ieeh-tu-dresden/power-system-data-model"
 
@@ -102,15 +102,15 @@
 
 [tool.black]
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
-version = "1.5.0"
+version = "1.5.1"
 version_files = [
     ".zenodo.json:version",
     "CITATION.cff:cff-version",
     "psdm/meta.py:VERSION",
     "pyproject.toml:version",
 ]
```

### Comparing `ieeh-power-system-data-model-1.5.0/tests/test_active_power.py` & `ieeh-power-system-data-model-1.5.1/tests/test_active_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/tests/test_branch.py` & `ieeh-power-system-data-model-1.5.1/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/tests/test_controller.py` & `ieeh-power-system-data-model-1.5.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/tests/test_reactive_power.py` & `ieeh-power-system-data-model-1.5.1/tests/test_reactive_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/tests/test_topology_load.py` & `ieeh-power-system-data-model-1.5.1/tests/test_topology_load.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.5.0/PKG-INFO` & `ieeh-power-system-data-model-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieeh-power-system-data-model
-Version: 1.5.0
+Version: 1.5.1
 Summary: A data model for describing power systems
 Author-email: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>,Laura Fiedler <laura.fiedler1@tu-dresden.de>,Maximilian Schmidt <maximilian.schmidt@tu-dresden.de>,Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 Requires-Python: >=3.10
 Project-URL: Source, https://github.com/ieeh-tu-dresden/power-system-data-model
 Description-Content-Type: text/markdown
 
 # IEEH Power System Data Model
```

