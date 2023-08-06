# Comparing `tmp/ansys-api-dyna-0.2.0.tar.gz` & `tmp/ansys-api-dyna-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-dyna-0.2.0.tar", last modified: Wed Jun 21 06:09:05 2023, max compression
+gzip compressed data, was "ansys-api-dyna-0.3.0.tar", last modified: Sun Aug  6 23:11:55 2023, max compression
```

## Comparing `ansys-api-dyna-0.2.0.tar` & `ansys-api-dyna-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.707717 ansys-api-dyna-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-21 06:09:05.707717 ansys-api-dyna-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 06:09:05.707717 ansys-api-dyna-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/ansys/api/dyna/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/dynasolver.proto
--rw-r--r--   0 runner    (1001) docker     (123)    42399 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/kwprocess.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.707717 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:11:55.977925 ansys-api-dyna-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-06 23:11:32.000000 ansys-api-dyna-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-06 23:11:55.977925 ansys-api-dyna-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-06 23:11:32.000000 ansys-api-dyna-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-06 23:11:32.000000 ansys-api-dyna-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 23:11:55.977925 ansys-api-dyna-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-08-06 23:11:32.000000 ansys-api-dyna-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:11:55.973925 ansys-api-dyna-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:11:55.973925 ansys-api-dyna-0.3.0/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:11:55.973925 ansys-api-dyna-0.3.0/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:11:55.973925 ansys-api-dyna-0.3.0/src/ansys/api/dyna/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 23:11:32.000000 ansys-api-dyna-0.3.0/src/ansys/api/dyna/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-06 23:11:32.000000 ansys-api-dyna-0.3.0/src/ansys/api/dyna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 23:11:32.000000 ansys-api-dyna-0.3.0/src/ansys/api/dyna/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:11:55.973925 ansys-api-dyna-0.3.0/src/ansys/api/dyna/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-08-06 23:11:32.000000 ansys-api-dyna-0.3.0/src/ansys/api/dyna/v0/dynasolver.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    44210 2023-08-06 23:11:32.000000 ansys-api-dyna-0.3.0/src/ansys/api/dyna/v0/kwprocess.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:11:55.977925 ansys-api-dyna-0.3.0/src/ansys_api_dyna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-06 23:11:55.000000 ansys-api-dyna-0.3.0/src/ansys_api_dyna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-06 23:11:55.000000 ansys-api-dyna-0.3.0/src/ansys_api_dyna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 23:11:55.000000 ansys-api-dyna-0.3.0/src/ansys_api_dyna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 23:11:55.000000 ansys-api-dyna-0.3.0/src/ansys_api_dyna.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 23:11:55.000000 ansys-api-dyna-0.3.0/src/ansys_api_dyna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 23:11:55.000000 ansys-api-dyna-0.3.0/src/ansys_api_dyna.egg-info/top_level.txt
```

### Comparing `ansys-api-dyna-0.2.0/LICENSE` & `ansys-api-dyna-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-dyna-0.2.0/PKG-INFO` & `ansys-api-dyna-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-dyna
-Version: 0.2.0
-Summary: Autogenerated python gRPC interface package for ansys-api-dyna, built on 06:09:05 on 21 June 2023
+Version: 0.3.0
+Summary: Autogenerated python gRPC interface package for ansys-api-dyna, built on 23:11:55 on 06 August 2023
 Home-page: https://github.com/ansys/ansys-api-dyna
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-dyna-0.2.0/README.md` & `ansys-api-dyna-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-dyna-0.2.0/setup.py` & `ansys-api-dyna-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/dynasolver.proto` & `ansys-api-dyna-0.3.0/src/ansys/api/dyna/v0/dynasolver.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/kwprocess.proto` & `ansys-api-dyna-0.3.0/src/ansys/api/dyna/v0/kwprocess.proto`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,22 @@
 	float abstol = 4;
 }
 
 message ControlImplicitSolutionReply {
 	int32 answer = 1;
 }
 
+message ControlImplicitConsistentMassRequest {
+    int32 iflag = 1;
+}
+
+message ControlImplicitConsistentMassReply {
+	int32 answer = 1;
+}
+
 message ControlSPHRequest {
     int32 ncbs = 1;
 	int32 boxid = 2;
 	int32 idim = 3;
 	int32 nmneigh = 4;
 	int32 form = 5;
 	float maxv = 6;
@@ -682,16 +690,17 @@
 }
 
 message DefineCurveReply {
 	int32 id = 1;
 }
 
 message DefineCurveFunctionRequest {
-    int32 lcid = 1;
-	string function = 2;
+	string title = 1;
+    int32 lcid = 2;
+	string function = 3;
 }
 
 message DefineCurveFunctionReply {
 	int32 id = 1;
 }
 
 message DefineVectorRequest {
@@ -931,25 +940,41 @@
 	float pr = 4;
 }
 
 message MatRigidDiscreteReply {
 	int32 mid = 1;
 }
 
+//MAT_001
 message MatElasticRequest {
 	int32 mid = 1;
 	float ro = 2;
 	float e = 3;
 	float pr = 4;
 }
 
 message MatElasticReply {
 	int32 mid = 1;
 }
 
+//MAT_003
+message MatPlasticKinematicRequest {
+	int32 mid = 1;
+	float ro = 2;
+	float e = 3;
+	float pr = 4;
+	float sigy = 5;
+	float etan = 6;
+	float beta = 7;
+}
+
+message MatPlasticKinematicReply {
+	int32 mid = 1;
+}
+
 message MatElasticPlasticThermalRequest {
 	int32 mid = 1;
 	float ro = 2;
 	repeated float ti = 3;
 	repeated float ei = 4;
 	repeated float pri = 5;
 	repeated float alphai = 6;
@@ -1000,14 +1025,28 @@
 	int32 numint = 8;
 }
 
 message MatModifiedPiecewiseLinearPlasticityReply {
 	int32 mid = 1;
 }
 
+//MAT_063
+message MatCrushableFoamRequest {
+	int32 mid = 1;
+	float ro = 2;
+	float e = 3;
+	float pr = 4;
+	int32 lcid = 5;
+	float tsl = 6;
+}
+
+message MatCrushableFoamReply {
+	int32 mid = 1;
+}
+
 message MatFabricRequest {
 	int32 mid = 1;
 	float ro = 2;
 	float ea = 3;
 	float eb = 4;
 	float prba = 5;
 	float prab = 6;
@@ -1125,28 +1164,42 @@
 }
 
 message MatSPHIncompressibleStructureReply {
 	int32 mid = 1;
 }
 
 //MATERIAL THERMAL
+//MAT_T01
 message MatThermalIsotropicRequest {
 	int32 mid = 1;
 	float tro = 2;
 	float tgrlc = 3;
 	float tgmult = 4;
 	//card2
 	float hc = 5;
 	float tc = 6;
 }
 
 message MatThermalIsotropicReply {
 	int32 mid = 1;
 }
 
+//MAT_T02
+message MatThermalOrthotropicRequest {
+	int32 mid = 1;
+	float hc = 2;
+	float k1 = 3;
+	float k2 = 4;
+	float k3 = 5;
+}
+
+message MatThermalOrthotropicReply {
+	int32 mid = 1;
+}
+
 //EOS
 message EOSLinearPolynomialRequest {
 	repeated float ci = 1;
 	float e0 = 2;
 	float v0 = 3;
 }
 
@@ -1755,14 +1808,25 @@
 	float sigma = 3;
 }
 
 message EMMat004Reply {
 	int32 answer = 1;
 }
 
+message EMMat006Request {
+    int32 mid = 1;
+	int32 mtype = 2;
+	float sigp = 3;
+	float sign = 4;
+}
+
+message EMMat006Reply {
+	int32 mid = 1;
+}
+
 message EMIsopotentialRequest {
     int32 isoid = 1;
 	int32 settype = 2;
 	int32 setid = 3;
 }
 
 message EMIsopotentialReply {
@@ -1782,14 +1846,35 @@
     float v0 = 9;
 }
 
 message EMIsopotentialConnectReply {
 	int32 id = 1;
 }
 
+message EMRandlesBatmacRequest {
+    int32 rdlid = 1;
+	int32 rdltype = 2;
+	int32 rdlarea = 3;
+	int32 psid = 4;
+	//card2
+	float q = 5;
+	float cq = 6;
+	float socinit = 7;
+	//card3
+	repeated float chargedirparam = 8;
+	//card4
+	float temp = 9;
+    int32 frther = 10;
+	int32 r0toth = 11;
+}
+
+message EMRandlesBatmacReply {
+	int32 rdlid = 1;
+}
+
 message EMIsopotentialRogoRequest {
     int32 isoid = 1;
 	int32 settype = 2;
 	int32 setid = 3;
 }
 
 message EMIsopotentialRogoReply {
@@ -1949,14 +2034,15 @@
 	rpc CreateControlThermalSolver(ControlThermalSolverRequest) returns (ControlThermalSolverReply) {}
     rpc CreateControlThermalTimestep(ControlThermalTimestepRequest) returns (ControlThermalTimestepReply) {}
 	rpc CreateControlImplicitGeneral(ControlImplicitGeneralRequest) returns (ControlImplicitGeneralReply) {}
 	rpc CreateControlImplicitAuto(ControlImplicitAutoRequest) returns (ControlImplicitAutoReply) {}
 	rpc CreateControlImplicitDynamic(ControlImplicitDynamicRequest) returns (ControlImplicitDynamicReply) {}
 	rpc CreateControlImplicitEigenvalue(ControlImplicitEigenvalueRequest) returns (ControlImplicitEigenvalueReply) {}
 	rpc CreateControlImplicitSolution(ControlImplicitSolutionRequest) returns (ControlImplicitSolutionReply) {}
+	rpc CreateControlImplicitConsistentMass(ControlImplicitConsistentMassRequest) returns (ControlImplicitConsistentMassReply) {}
 	rpc CreateControlSPH(ControlSPHRequest) returns (ControlSPHReply) {}
 	
 	
 	//---DATABASE
 	rpc CreateDBBinary(DBBinaryRequest) returns (DBBinaryReply) {}
 	rpc CreateDBAscii(DBAsciiRequest) returns (DBAsciiReply) {}
 	rpc CreateDBSALE(DBSALERequest) returns (DBSALEReply) {}
@@ -1988,31 +2074,34 @@
 	rpc CreateLoadBody(LoadBodyRequest) returns (LoadBodyReply) {}
 
 	//---MATERIAL
 	rpc CreateMatEM(MatEMRequest) returns (MatEMReply) {}
 	rpc CreateMatRigid(MatRigidRequest) returns (MatRigidReply) {}
 	rpc CreateMatRigidDiscrete(MatRigidDiscreteRequest) returns (MatRigidDiscreteReply) {}
 	rpc CreateMatElastic(MatElasticRequest) returns (MatElasticReply) {}
+	rpc CreateMatPlasticKinematic(MatPlasticKinematicRequest) returns (MatPlasticKinematicReply) {}
 	rpc CreateMatElasticPlasticThermal(MatElasticPlasticThermalRequest) returns (MatElasticPlasticThermalReply) {}
 	rpc CreateMatSpotweld(MatSpotweldRequest) returns (MatSpotweldReply) {}
     rpc CreateMatPiecewiseLinearPlasticity(MatPiecewiseLinearPlasticityRequest) returns (MatPiecewiseLinearPlasticityReply) {}
 	rpc CreateMatModifiedPiecewiseLinearPlasticity(MatModifiedPiecewiseLinearPlasticityRequest) returns (MatModifiedPiecewiseLinearPlasticityReply) {}
+	rpc CreateMatCrushableFoam(MatCrushableFoamRequest) returns (MatCrushableFoamReply) {}
 	rpc CreateMatFabric(MatFabricRequest) returns (MatFabricReply) {}
 	rpc CreateMatSpringNonlinearElastic(MatSpringNonlinearElasticRequest) returns (MatSpringNonlinearElasticReply) {}
 	rpc CreateMatDamperViscous(MatDamperViscousRequest) returns (MatDamperViscousReply) {}
 	rpc CreateMatDamperNonlinearViscous(MatDamperNonlinearViscousRequest) returns (MatDamperNonlinearViscousReply) {}
 	rpc CreateMatNull(MatNullRequest) returns (MatNullReply) {}
 	rpc CreateMatJohnsonCook(MatJohnsonCookRequest) returns (MatJohnsonCookReply) {}
 	rpc CreateMatHighExplosiveBurn(MatHighExplosiveBurnRequest) returns (MatHighExplosiveBurnReply) {}
 	rpc CreateMatVacuum(MatVacuumRequest) returns (MatVacuumReply) {}
 	rpc CreateMatAddErosion(MatAddErosionRequest) returns (MatAddErosionReply) {}
  	rpc CreateMatSPHIncompressibleFluid(MatSPHIncompressibleFluidRequest) returns (MatSPHIncompressibleFluidReply) {}
 	rpc CreateMatSPHIncompressibleStructure(MatSPHIncompressibleStructureRequest) returns (MatSPHIncompressibleStructureReply) {}
 	rpc CreateMatThermalIsotropic(MatThermalIsotropicRequest) returns (MatThermalIsotropicReply) {}
-	
+	rpc CreateMatThermalOrthotropic(MatThermalOrthotropicRequest) returns (MatThermalOrthotropicReply) {}
+
 	//---EOS
     rpc CreateEOSLinearPolynomial(EOSLinearPolynomialRequest) returns (EOSLinearPolynomialReply) {}
     rpc CreateEOSJWL(EOSJWLRequest) returns (EOSJWLReply) {}
 	rpc CreateEOSGruneisen(EOSGruneisenRequest) returns (EOSGruneisenReply) {}
 
 	
 	//---DEFINE
@@ -2108,16 +2197,18 @@
 	rpc CreateEMControlContact(EMControlContactRequest) returns (EMControlContactReply) {}
 	rpc CreateEMContact(EMContactRequest) returns (EMContactReply) {}
 	rpc CreateEMCircuitRogo(EMCircuitRogoRequest) returns (EMCircuitRogoReply) {}
 	rpc CreateEMCircuit(EMCircuitRequest) returns (EMCircuitReply) {}
 	rpc CreateEMMat001(EMMat001Request) returns (EMMat001Reply) {}
 	rpc CreateEMMat002(EMMat002Request) returns (EMMat002Reply) {}
 	rpc CreateEMMat004(EMMat004Request) returns (EMMat004Reply) {}
+	rpc CreateEMMat006(EMMat006Request) returns (EMMat006Reply) {}
 	rpc CreateEMIsopotential(EMIsopotentialRequest) returns (EMIsopotentialReply) {}
 	rpc CreateEMIsopotentialConnect(EMIsopotentialConnectRequest) returns (EMIsopotentialConnectReply) {}
+	rpc CreateEMRandlesBatmac(EMRandlesBatmacRequest) returns (EMRandlesBatmacReply) {}
 	rpc CreateEMIsopotentialRogo(EMIsopotentialRogoRequest) returns (EMIsopotentialRogoReply) {}
 	rpc CreateEMSolverBem(EMSolverBemRequest) returns (EMSolverBemReply) {}
 	rpc CreateEMSolverFem(EMSolverFemRequest) returns (EMSolverFemReply) {}
 	rpc CreateEMSolverBemMat(EMSolverBemMatRequest) returns (EMSolverBemMatReply) {}
 	rpc CreateEMSolverFemBemMonolithic(EMSolverFemBemMonolithicRequest) returns (EMSolverFemBemMonolithicReply) {}
 	rpc CreateEMOutput(EMOutputRequest) returns (EMOutputReply) {}
 	rpc CreateEMDatabaseGlobalEnergy(EMDatabaseGlobalEnergyRequest) returns (EMDatabaseGlobalEnergyReply) {}
```

### Comparing `ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/PKG-INFO` & `ansys-api-dyna-0.3.0/src/ansys_api_dyna.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-dyna
-Version: 0.2.0
-Summary: Autogenerated python gRPC interface package for ansys-api-dyna, built on 06:09:05 on 21 June 2023
+Version: 0.3.0
+Summary: Autogenerated python gRPC interface package for ansys-api-dyna, built on 23:11:55 on 06 August 2023
 Home-page: https://github.com/ansys/ansys-api-dyna
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

