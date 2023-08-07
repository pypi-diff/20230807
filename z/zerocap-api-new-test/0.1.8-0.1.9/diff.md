# Comparing `tmp/zerocap_api_new_test-0.1.8.tar.gz` & `tmp/zerocap_api_new_test-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zerocap_api_new_test-0.1.8.tar", last modified: Tue Aug  1 03:43:52 2023, max compression
+gzip compressed data, was "dist/zerocap_api_new_test-0.1.9.tar", last modified: Fri Aug  4 03:13:17 2023, max compression
```

## Comparing `zerocap_api_new_test-0.1.8.tar` & `zerocap_api_new_test-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/
--rw-rw-rw-   0        0        0    11523 2023-07-26 06:34:57.000000 zerocap_api_new_test-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0    19690 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    15434 2023-07-31 02:13:00.000000 zerocap_api_new_test-0.1.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2133 2023-08-01 03:43:02.000000 zerocap_api_new_test-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test/
--rw-rw-rw-   0        0        0      126 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test/__init__.py
--rw-rw-rw-   0        0        0     8141 2023-08-01 03:35:19.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test/main.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/
--rw-rw-rw-   0        0        0    19690 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/top_level.txt
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/
+-rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-26 06:32:00.000000 zerocap_api_new_test-0.1.9/LICENSE.txt
+-rw-r--r--   0 gao        (501) staff       (20)    19147 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)    14970 2023-07-31 02:28:33.000000 zerocap_api_new_test-0.1.9/README.rst
+-rw-r--r--   0 gao        (501) staff       (20)       38 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/setup.cfg
+-rw-r--r--   0 gao        (501) staff       (20)     2056 2023-08-04 03:12:45.000000 zerocap_api_new_test-0.1.9/setup.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/zerocap_api_new_test/
+-rw-r--r--   0 gao        (501) staff       (20)      121 2023-07-31 00:59:59.000000 zerocap_api_new_test-0.1.9/zerocap_api_new_test/__init__.py
+-rw-r--r--   0 gao        (501) staff       (20)     7917 2023-08-04 03:06:02.000000 zerocap_api_new_test-0.1.9/zerocap_api_new_test/main.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/zerocap_api_new_test.egg-info/
+-rw-r--r--   0 gao        (501) staff       (20)    19147 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/zerocap_api_new_test.egg-info/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      312 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/zerocap_api_new_test.egg-info/SOURCES.txt
+-rw-r--r--   0 gao        (501) staff       (20)        1 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/zerocap_api_new_test.egg-info/dependency_links.txt
+-rw-r--r--   0 gao        (501) staff       (20)       19 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/zerocap_api_new_test.egg-info/requires.txt
+-rw-r--r--   0 gao        (501) staff       (20)       21 2023-08-04 03:13:17.000000 zerocap_api_new_test-0.1.9/zerocap_api_new_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_new_test-0.1.8/LICENSE.txt` & `zerocap_api_new_test-0.1.9/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `zerocap_api_new_test-0.1.8/PKG-INFO` & `zerocap_api_new_test-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,589 +1,590 @@
-Metadata-Version: 2.1
-Name: zerocap_api_new_test
-Version: 0.1.8
-Summary: zerocap_api
-Home-page: https://zerocap.com/
-Author: zerocap
-Author-email: jiayu.gao@eigen.capital
-License: MIT
-Platform: all
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
-# zerocap-api-new-test 
-
-# <a href="#testapi">Jump restapi</a>
-# <a href="#test">Jump websocket</a>
-
-
-
-```
-
-描述介绍
-
-sdk install
-pip install zerocap-api-new-test 
-。
-。
-。
-
-```
-
-
-
-# <a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi </a>
-#### <a href="https://dma-api.defi.wiki/redoc" target="_blank">接口文档</a> 
-
-```
-from zerocap_api_new_test import ZerocapRestClient
-import uuid
-import time
-
-# API key and secret required, 联系zerocap进行注册
-apiKey = "coinroutes" 
-apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
-```
-
-#### 1. Create an order
-<!--post https://dma-api.defi.wiki/orders/create_order-->
-
-```
-
-client = ZerocapRestClient(apiKey, apiSecret)
-client_order_id = str(uuid.uuid4())
-
-result = client.create_order(
-                    symbol='USDT/AUD', 
-                    side='buy', 
-                    type='market', 
-                    amount='100', 
-                    price='1000', 
-                    client_order_id=client_order_id, 
-                    note='this is test', 
-                    third_identity_id='ZCStreamingLiquidity1')
-
-```
-
-
-请求参数:
-
-| Parameter       | required  | data type | describe        | Value range  |
-|-----------------|-----------|-----------|-----------------|--------------|
-| symbol          | true      | string    | Instrument      | USDT/AUD     |
-| side            | true      | string    | Side            | buy sell     |
-| type            | true      | string    | Type            | market limit |
-| amount          | true      | string    | Quantity        |              |
-| price           | true      | string    | Price           |              |
-| client_order_id | true      | string    | Client order id |              |
-| note | true      | string    | note  |              |
-| third_identity_id | true      | string    | third_identity_id |              |
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-{
-    "symbol": "USDT/AUD",
-    "side": "buy",
-    "type": "market",
-    "amount": "1000",
-    "price": "1000",
-    "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
-    "account_vault": {
-        "third_identity_id": "918d7125916c13191f3674e",
-        "api_key": "***",
-        "signature": "***",
-        "note": ""
-    }
-}
-
-```
-
-响应数据:
-
-| Parameter          | required | data type | describe        | Value range |
-|--------------------|----------|-----------|-----------------|-------------|
-| id                 | true     | long      | Transaction ID  |             |
-| clientOrderId      | true     | string    | Client order id |             |
-| datatime           | true     | string    | Time            |             |
-| timestamp          | true     | string    | Time            |             |
-| lastTradeTimestamp | true     | long      | Time            |             |
-| status             | true     | string    | Status          |             |
-| type               | true     | string    | Type            |             |
-| timeInForce        | true     | string    | timeInForce     |             |
-| side               | true     | string    | Side            |             |
-| price              | true     | string    | Price           |             |
-| average            | true     | string    | average         |             |
-| amount             | true     | string    | Quantity        |             |
-| filled             | true     | string    | filled          |             |
-| remaining          | true     | string    | remaining       |             |
-| cost               | true     | string    | cost            |             |
-| transferId         | true     | string    | transferId      |             |
-| trades             | true     | string    | trades          |             |
-
-
-响应例子:
-
-```
-
- {
-    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
-    "clientOrderId": "e7f80d34-0d80-4256-9de3-cd37310a55dabe",
-    "datatime": "2023-07-28 09:19:45",
-    "timestamp": "1690535984000",
-    "lastTradeTimestamp": "1690535984000",
-    "status": "closed",
-    "symbol": "USDT/AUD",
-    "type": "Market",
-    "timeInForce": "FOK",
-    "side": "buy",
-    "price": "21.1",
-    "average": "1.685133171",
-    "amount": "9",
-    "filled": "9",
-    "remaining": "0",
-    "cost": "15.16619854",
-    "transferId": "12424971-f51d-4144-a205-9e306eb6351c",
-    "trades": [
-        {
-            "id": "12424971-f51d-4144-a205-9e306eb6351c",
-            "timestamp": "1690535984000",
-            "datetime": "2023-07-28 09:19:45",
-            "symbol": "USDT/AUD",
-            "order": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
-            "type": "market",
-            "side": "buy",
-            "takerOrMaker": "taker",
-            "price": "1.685133171",
-            "amount": "9",
-            "cost": "15.16619854",
-            "orderFrom": "coinroutes"
-        }
-    ]
-}
-
-```
-
-
-
-
-#### 2. Fetch specific orders
-<!--post https://dma-api.defi.wiki/orders/fetch_order-->
-```
-result = client.fetch_order(id='')
-```
-
-请求参数:
-
-
-| Parameter       | required | data type | describe       | Value range  |
-|-----------------|----------|-----------|----------------|--------------|
-| id              | true     | string    | Transaction ID |              |
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-{
-    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
-    "account_vault": {
-        "third_identity_id": "918d7125916c13191f3674e",
-        "api_key": "***",
-        "signature": "***",
-        "note": ""
-    }
-}
-
-```
-
-响应数据 接口报错 待定:
-
-
-| Parameter     | required | data type | describe       | Value range |
-|---------------|----------|-----------|----------------|-------------|
-| id            | true     | string    | Transaction ID |             |
-
-
-响应例子:
-
-```
-
-{
-	"order_list": [
-		{
-			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
-			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
-			"datatime": "2023-07-31 02:12:23",
-			"timestamp": "1690516007000",
-			"last_trade_timestamp": "1690516007000",
-			"status": "rejected",
-			"symbol": "USDT/AUD",
-			"type": "market",
-			"time_in_force": "FOK",
-			"side": "buy",
-			"price": "1000",
-			"average": "",
-			"amount": "1000",
-			"filled": "",
-			"remaining": "",
-			"cost": "",
-			"transfer_id": "",
-			"fee": "",
-			"trades": []
-		}
-	],
-	"status": "success",
-	"total": 3864,
-	"page": "1"
-}
-
-```
-
-
-#### 3. Batch fetch order
-<!--post https://dma-api.defi.wiki/orders/fetch_orders-->
-
-```
-result = client.fetch_orders(symbol='USDT/AUD', end_datetime=int(time.time() * 1000),
-                             start_datetime=int(time.time() * 1000 - 10*86400*1000),
-                             limit=10)
-```
-
-
-
-请求参数:
-
-| Parameter      | required | data type | describe        | Value range |
-|----------------|----------|-----------|-----------------|-------------|
-| symbol         | true     | string    | symbol          |             |
-| start_datetime | true     | string    | start_datetime  |             |
-| end_datetime   | true     | string    | end_datetime    |             |
-| page           | true     | string    | page            |             |
-| limit          | true     | string    | limit           |             |
-| ids            | true     | string    | Transaction ids(null character string or id1,id2...) |   |
-| status         | true     | string    | status          |             |
-| sort_order     | true     | string    | sort_order      |             |
-| order_type     | true     | string    | order_type      |             |
-| side           | true     | string    | side            |             |
-
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-{
-    "symbol": "",
-    "start_datetime": 0,
-    "end_datetime": 0,
-    "page": 0,
-    "limit": 0,
-    "ids": "",
-    "status": "",
-    "sort_order": "",
-    "order_type": "",
-    "side": "",
-    "account_vault": {
-        "third_identity_id": "918d7125916c13191f3674e",
-        "api_key": "***",
-        "signature": "***",
-        "note": ""
-    }
-}
-
-```
-
-响应数据 接口报错 待定:
-
-
-
-| Parameter     | required | data type | describe       | Value range |
-|---------------|----------|-----------|----------------|-------------|
-| id            | true     | string    | Transaction ID |             |
-| account_vault | true     | json      |  accountVault  |             |
-
-
-
-响应例子:
-
-```
-
-{
-	"order_list": [
-		{
-			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
-			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
-			"datatime": "2023-07-31 02:12:23",
-			"timestamp": "1690516007000",
-			"last_trade_timestamp": "1690516007000",
-			"status": "rejected",
-			"symbol": "USDT/AUD",
-			"type": "market",
-			"time_in_force": "FOK",
-			"side": "buy",
-			"price": "1000",
-			"average": "",
-			"amount": "1000",
-			"filled": "",
-			"remaining": "",
-			"cost": "",
-			"transfer_id": "",
-			"fee": "",
-			"trades": []
-		}
-	],
-	"status": "success",
-	"total": 3864,
-	"page": "1"
-}
-
-```
-
-
-
-## <span id='test'>websocket</span>
-
-```
-from zerocap_api_new_test import ZerocapWebsocketClient
-
-# API key and secret required, 联系zerocap进行注册
-apiKey = "***" 
-apiSecret = "***"
-
-signature = hmac.new(apiSecret.encode("utf-8"), apiKey.encode("utf-8"), hashlib.sha256).hexdigest()
-
-```
-
-#### 1. Subscribe to Market data
-
-<!--websocket wss://dma-api.defi.wiki/ws/GetMarket-->
-
-```
-market_connect = websocket.get_market()
-
-while True:
-    # Get  messages
-    message = websocket.get_message(market_connect)
-
-    print(f"Receiving message from server: \n{message}")
-
-```
-
-请求参数:
-
-| Parameter     | required | data type | describe                | Value range |
-|---------------|----------|-----------|-------------------------|-------------|
-| api_key       | true     | string    | key                     |             |
-| signature     | true     | long      | Cryptographic signature |             |
-| data_type     | true     | string    | Subscribed Channels     | price       |
-
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-wss://dma-api.defi.wiki/ws/GetMarket?api_key=***&signature=***&data_type=price
-
-```
-
-
-响应数据:
-
-
-| Parameter          | required | data type | describe      | Value range        |
-|--------------------|----------|-----------|---------------|--------------------|
-| type               | true     | long      | type          |                    |
-| channel            | true     | string    | channel       | dma_price_USDT/AUD |
-| data               | true     | jsonstr   | data          |                    |
-| data['sell_price'] | true     | string    | sell price    |                    |
-| data['buy_price']  | true     | string    | buy price     |                    |
-| data['datetime']   | true     | string    | time          |                    |
-| data['timestamp']  | true     | string    | time          |                    |
-| message            | false    | string    | description   | Is price open      |
-
-
-响应例子:
-
-```
-
-{
-    "type": "message",
-    "channel": "dma_price_USDT/AUD",
-    "data": "{
-        \"sell_price\": \"1.322544321902561296\",
-        \"buy_price\": \"1.668209315127094362\",
-        \"datetime\": \"2023-07-28 10:03:40\",
-        \"timestamp\": \"1690538620.1056492\"
-        }"
-}
-
-{
-    "type": "message",
-    "channel": "dma_price_USDT/AUD",
-    "data": "{
-        \"message\":\"Price stream unavailable.\"
-        }"
-}
-
-# Heartbeat neglect
-{"type":"message","channel":"","data":"{\"ok\": \"ok\"}"}
-
-```
-
-#### 2.  Subscribe Order updates or transaction records
-
-
-<!--websocket url:   wss://dma-api.defi.wiki/ws/GetOrdersInfo-->
-
-```
-orders_connect = websocket.get_orders()
-
-while True:
-    # Get  messages
-    message = websocket.get_message(orders_connect)
-
-    print(f"Receiving message from server: \n{message}")
-
-```
-
-
-请求参数:
-
-
-| Parameter     | required | data type | describe                | Value range |
-|---------------|----------|-----------|-------------------------|-------------|
-| api_key       | true     | string    | key                     |             |
-| signature     | true     | long      | Cryptographic signature |             |
-| data_type     | true     | string    | Subscribed Channels     | order,trade |
-
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-wss://dma-api.defi.wiki/ws/GetOrdersInfo?api_key=***&signature=***&data_type=order,trade
-
-```
-
-
-channel: dma_order_info 响应数据:
-
-
-| Parameter             | required   | data type | describe      | Value range                    |
-|-----------------------|------------|-----------|---------------|--------------------------------|
-| type                  | true       | long      | type          |                                |
-| channel               | true       | string    | channel       | dma_order_info、dma_trader_info |
-| data                  | true       | jsonstr   | data          |                                |
-| data['OrderId']       | true       | str       | OrderId       |                                |
-| data['ClientOrderId'] | true       | str       | ClientOrderId |                                |
-| data['TxnAlias']      | true       | str       | TxnAlias      |                                |
-| data['TransferId']    | true       | str       | TransferId    |                                |
-| data['Symbol']        | true       | str       | Symbol        |                                |
-| data['Type']          | true       | str       | Type          |                                |
-| data['TimeInForce']   | true       | str       | TimeInForce   |                                |
-| data['Side']          | true       | str       | Side          |                                |
-| data['OrderId']       | true       | str       | OrderId       |                                |
-| data['Price']         | true       | str       | Price         |                                |
-| data['AveragePrice']  | true       | str       | AveragePrice  |                                |
-| data['Amount']        | true       | str       | Amount        |                                |
-| data['CreatedAt']     | true       | str       | CreatedAt     |                                |
-| data['UpdatedAt']     | true       | str       | UpdatedAt     |                                |
-| data['AccountId']     | true       | str       | AccountId     |                                |
-| data['VaultId']       | true       | str       | VaultId       |                                |
-| data['Note']          | true       | str       | Note          |                                |
-| data['Status']        | true       | str       | Status        |                                |
-| data['Average']       | true       | str       | Average       |                                |
-| data['Filled']        | true       | str       | Filled        |                                |
-| data['Remaining']     | true       | str       | Remaining     |                                |
-| data['Cost']          | true       | str       | Cost          |                                |
-| data['ExecPrice']     | true       | str       | ExecPrice     |                                |
-| data['OrderFrom']     | true       | str       | OrderFrom     |                                |
-
-
-响应例子:
-
-```
-
-{
-    "type":"message",
-    "channel":"dma_order_info",
-    "data":"{
-        \"OrderId\":\"d8be1f41-9e8e-4af0-899b-c1334916aa0e\",
-        \"ClientOrderId\":\"e7f80d34-0d80-4256-9de3-cd37310a55da\",
-        \"TxnAlias\":\"\",
-        \"TransferId\":\"\",
-        \"Symbol\":\"USDT/AUD\",
-        \"Type\":\"market\",
-        \"TimeInForce\":\"FOK\",
-        \"Side\":\"sell\",
-        \"Price\":\"1000\",
-        \"AveragePrice\":\"\",
-        \"Amount\":\"1000\",
-        \"CreatedAt\":1690538950000,
-        \"UpdatedAt\":1690538950000,
-        \"AccountId\":\"1ca36d2b-2103-45c7-a2e3-3b90825ba1b2\",
-        \"VaultId\":\"5175\",
-        \"Note\":\"yyy_test_create_order\",
-        \"Status\":\"open\",
-        \"Average\":\"0\",
-        \"Filled\":\"0\",
-        \"Remaining\":\"1000\",
-        \"Cost\":\"1000000\",
-        \"ExecPrice\":\"\",
-        \"OrderFrom\":\"coinroutes\"
-    }"
-}
-
-```
-
-channel: dma_trader_info 响应数据:
-
-
-| Parameter            | required   | data type | describe     | Value range                    |
-|----------------------|------------|-----------|--------------|--------------------------------|
-| type                 | true       | long      | type         |                                |
-| channel              | true       | string    | channel      | dma_order_info、dma_trader_info |
-| data                 | true       | jsonstr   | data         |                                |
-| data['id']           | true       | str       | id           |                                |
-| data['timestamp']    | true       | str       | timestamp    |                                |
-| data['datetime']     | true       | str       | datetime     |                                |
-| data['symbol']       | true       | str       | symbol       |                                |
-| data['order']        | true       | str       | order        |                                |
-| data['type']         | true       | str       | type         |                                |
-| data['side']         | true       | str       | side         |                                |
-| data['takerOrMaker'] | true       | str       | takerOrMaker |                                |
-| data['price']        | true       | str       | price        |                                |
-| data['amount']       | true       | str       | amount       |                                |
-| data['cost']         | true       | str       | cost         |                                |
-| data['orderFrom']    | true       | str       | orderFrom    |                                |
-
-
-响应例子:
-
-```
-
-{
-    "type":"message",
-    "pattern":null,
-    "channel":"dma_trade_info",
-    "data":"{
-        \"id\":\"60e2e941-070c-40e3-b2ef-4a8f6ad9f316\",
-        \"timestamp\":\"1690767892000\",
-        \"datetime\":\"2023-07-31 01:44:52\",
-        \"symbol\":\"USDT/AUD\",
-        \"order\":\"41969863-1f32-4eaa-b679-a5b0e6fb5542\",
-        \"type\":\"market\",
-        \"side\":\"sell\",
-        \"takerOrMaker\":\"taker\",
-        \"price\":\"1.662902412\",
-        \"amount\":\"101\",
-        \"cost\":\"167.9531436\",
-        \"orderFrom\":\"coinroutes\"
-    }"
-}
-
-```
+Metadata-Version: 2.1
+Name: zerocap_api_new_test
+Version: 0.1.9
+Summary: zerocap_api
+Home-page: https://zerocap.com/
+Author: zerocap
+Author-email: jiayu.gao@eigen.capital
+License: MIT
+Platform: all
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# zerocap-api-new-test 
+
+# <a href="#testapi">Jump restapi</a>
+# <a href="#test">Jump websocket</a>
+
+
+
+```
+
+描述介绍
+
+sdk install
+pip install zerocap-api-new-test 
+。
+。
+。
+
+```
+
+
+
+# <a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi </a>
+#### <a href="https://dma-api.defi.wiki/redoc" target="_blank">接口文档</a> 
+
+```
+from zerocap_api_new_test import ZerocapRestClient
+import uuid
+import time
+
+# API key and secret required, 联系zerocap进行注册
+apiKey = "coinroutes" 
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
+```
+
+#### 1. Create an order
+<!--post https://dma-uat-api.defi.wiki/v2/orders/create_order-->
+
+```
+
+client = ZerocapRestClient(apiKey, apiSecret)
+client_order_id = str(uuid.uuid4())
+
+result = client.create_order(
+                    symbol='USDT/AUD', 
+                    side='buy', 
+                    type='market', 
+                    amount='100', 
+                    price='1000', 
+                    client_order_id=client_order_id, 
+                    note='this is test', 
+                    third_identity_id='ZCStreamingLiquidity1')
+
+```
+
+
+请求参数:
+
+| Parameter       | required  | data type | describe        | Value range  |
+|-----------------|-----------|-----------|-----------------|--------------|
+| symbol          | true      | string    | Instrument      | USDT/AUD     |
+| side            | true      | string    | Side            | buy sell     |
+| type            | true      | string    | Type            | market limit |
+| amount          | true      | string    | Quantity        |              |
+| price           | true      | string    | Price           |              |
+| client_order_id | true      | string    | Client order id |              |
+| note | true      | string    | note  |              |
+| third_identity_id | true      | string    | third_identity_id |              |
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+{
+    "symbol": "USDT/AUD",
+    "side": "buy",
+    "type": "market",
+    "amount": "1000",
+    "price": "1000",
+    "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+    "account_vault": {
+        "third_identity_id": "918d7125916c13191f3674e",
+        "api_key": "***",
+        "signature": "***",
+        "note": ""
+    }
+}
+
+```
+
+响应数据:
+
+| Parameter          | required | data type | describe        | Value range |
+|--------------------|----------|-----------|-----------------|-------------|
+| id                 | true     | long      | Transaction ID  |             |
+| clientOrderId      | true     | string    | Client order id |             |
+| datatime           | true     | string    | Time            |             |
+| timestamp          | true     | string    | Time            |             |
+| lastTradeTimestamp | true     | long      | Time            |             |
+| status             | true     | string    | Status          |             |
+| type               | true     | string    | Type            |             |
+| timeInForce        | true     | string    | timeInForce     |             |
+| side               | true     | string    | Side            |             |
+| price              | true     | string    | Price           |             |
+| average            | true     | string    | average         |             |
+| amount             | true     | string    | Quantity        |             |
+| filled             | true     | string    | filled          |             |
+| remaining          | true     | string    | remaining       |             |
+| cost               | true     | string    | cost            |             |
+| transferId         | true     | string    | transferId      |             |
+| trades             | true     | string    | trades          |             |
+
+
+响应例子:
+
+```
+
+ {
+    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
+    "clientOrderId": "e7f80d34-0d80-4256-9de3-cd37310a55dabe",
+    "datatime": "2023-07-28 09:19:45",
+    "timestamp": "1690535984000",
+    "lastTradeTimestamp": "1690535984000",
+    "status": "closed",
+    "symbol": "USDT/AUD",
+    "type": "Market",
+    "timeInForce": "FOK",
+    "side": "buy",
+    "price": "21.1",
+    "average": "1.685133171",
+    "amount": "9",
+    "filled": "9",
+    "remaining": "0",
+    "cost": "15.16619854",
+    "transferId": "12424971-f51d-4144-a205-9e306eb6351c",
+    "trades": [
+        {
+            "id": "12424971-f51d-4144-a205-9e306eb6351c",
+            "timestamp": "1690535984000",
+            "datetime": "2023-07-28 09:19:45",
+            "symbol": "USDT/AUD",
+            "order": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
+            "type": "market",
+            "side": "buy",
+            "takerOrMaker": "taker",
+            "price": "1.685133171",
+            "amount": "9",
+            "cost": "15.16619854",
+            "orderFrom": "coinroutes"
+        }
+    ]
+}
+
+```
+
+
+
+
+#### 2. Fetch specific orders
+<!--post https://dma-uat-api.defi.wiki/v2/orders/fetch_order-->
+```
+result = client.fetch_order(id='')
+```
+
+请求参数:
+
+
+| Parameter       | required | data type | describe       | Value range  |
+|-----------------|----------|-----------|----------------|--------------|
+| id              | true     | string    | Transaction ID |              |
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+{
+    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
+    "account_vault": {
+        "third_identity_id": "918d7125916c13191f3674e",
+        "api_key": "***",
+        "signature": "***",
+        "note": ""
+    }
+}
+
+```
+
+响应数据 接口报错 待定:
+
+
+| Parameter     | required | data type | describe       | Value range |
+|---------------|----------|-----------|----------------|-------------|
+| id            | true     | string    | Transaction ID |             |
+
+
+响应例子:
+
+```
+
+{
+	"order_list": [
+		{
+			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
+			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+			"datatime": "2023-07-31 02:12:23",
+			"timestamp": "1690516007000",
+			"last_trade_timestamp": "1690516007000",
+			"status": "rejected",
+			"symbol": "USDT/AUD",
+			"type": "market",
+			"time_in_force": "FOK",
+			"side": "buy",
+			"price": "1000",
+			"average": "",
+			"amount": "1000",
+			"filled": "",
+			"remaining": "",
+			"cost": "",
+			"transfer_id": "",
+			"fee": "",
+			"trades": []
+		}
+	],
+	"status": "success",
+	"total": 3864,
+	"page": "1"
+}
+
+```
+
+
+#### 3. Batch fetch order
+<!--post https://dma-uat-api.defi.wiki/v2/orders/fetch_orders-->
+
+```
+result = client.fetch_orders(symbol='USDT/AUD', end_datetime=int(time.time() * 1000),
+                             start_datetime=int(time.time() * 1000 - 10*86400*1000),
+                             limit=10)
+```
+
+
+
+请求参数:
+
+| Parameter      | required | data type | describe        | Value range |
+|----------------|----------|-----------|-----------------|-------------|
+| symbol         | true     | string    | symbol          |             |
+| start_datetime | true     | string    | start_datetime  |             |
+| end_datetime   | true     | string    | end_datetime    |             |
+| page           | true     | string    | page            |             |
+| limit          | true     | string    | limit           |             |
+| ids            | true     | string    | Transaction ids(null character string or id1,id2...) |   |
+| status         | true     | string    | status          |             |
+| sort_order     | true     | string    | sort_order      |             |
+| order_type     | true     | string    | order_type      |             |
+| side           | true     | string    | side            |             |
+
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+{
+    "symbol": "",
+    "start_datetime": 0,
+    "end_datetime": 0,
+    "page": 0,
+    "limit": 0,
+    "ids": "",
+    "status": "",
+    "sort_order": "",
+    "order_type": "",
+    "side": "",
+    "account_vault": {
+        "third_identity_id": "918d7125916c13191f3674e",
+        "api_key": "***",
+        "signature": "***",
+        "note": ""
+    }
+}
+
+```
+
+响应数据 接口报错 待定:
+
+
+
+| Parameter     | required | data type | describe       | Value range |
+|---------------|----------|-----------|----------------|-------------|
+| id            | true     | string    | Transaction ID |             |
+| account_vault | true     | json      |  accountVault  |             |
+
+
+
+响应例子:
+
+```
+
+{
+	"order_list": [
+		{
+			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
+			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+			"datatime": "2023-07-31 02:12:23",
+			"timestamp": "1690516007000",
+			"last_trade_timestamp": "1690516007000",
+			"status": "rejected",
+			"symbol": "USDT/AUD",
+			"type": "market",
+			"time_in_force": "FOK",
+			"side": "buy",
+			"price": "1000",
+			"average": "",
+			"amount": "1000",
+			"filled": "",
+			"remaining": "",
+			"cost": "",
+			"transfer_id": "",
+			"fee": "",
+			"trades": []
+		}
+	],
+	"status": "success",
+	"total": 3864,
+	"page": "1"
+}
+
+```
+
+
+
+## <span id='test'>websocket</span>
+
+```
+from zerocap_api_new_test import ZerocapWebsocketClient
+
+# API key and secret required, 联系zerocap进行注册
+apiKey = "***" 
+apiSecret = "***"
+
+signature = hmac.new(apiSecret.encode("utf-8"), apiKey.encode("utf-8"), hashlib.sha256).hexdigest()
+
+```
+
+#### 1. Subscribe to Market data
+
+<!--websocket wss://dma-uat-ws.defi.wiki/v2/ws/GetMarket-->
+
+```
+market_connect = websocket.get_market()
+
+while True:
+    # Get  messages
+    message = websocket.get_message(market_connect)
+
+    print(f"Receiving message from server: \n{message}")
+
+```
+
+请求参数:
+
+| Parameter     | required | data type | describe                | Value range |
+|---------------|----------|-----------|-------------------------|-------------|
+| api_key       | true     | string    | key                     |             |
+| signature     | true     | long      | Cryptographic signature |             |
+| data_type     | true     | string    | Subscribed Channels     | price       |
+
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+wss://dma-uat-ws.defi.wiki/v2/ws/GetMarket?api_key=***&signature=***&data_type=price
+
+```
+
+
+响应数据:
+
+
+| Parameter          | required | data type | describe      | Value range        |
+|--------------------|----------|-----------|---------------|--------------------|
+| type               | true     | long      | type          |                    |
+| channel            | true     | string    | channel       | dma_price_USDT/AUD |
+| data               | true     | jsonstr   | data          |                    |
+| data['sell_price'] | true     | string    | sell price    |                    |
+| data['buy_price']  | true     | string    | buy price     |                    |
+| data['datetime']   | true     | string    | time          |                    |
+| data['timestamp']  | true     | string    | time          |                    |
+| message            | false    | string    | description   | Is price open      |
+
+
+响应例子:
+
+```
+
+{
+    "type": "message",
+    "channel": "dma_price_USDT/AUD",
+    "data": "{
+        \"sell_price\": \"1.322544321902561296\",
+        \"buy_price\": \"1.668209315127094362\",
+        \"datetime\": \"2023-07-28 10:03:40\",
+        \"timestamp\": \"1690538620.1056492\"
+        }"
+}
+
+{
+    "type": "message",
+    "channel": "dma_price_USDT/AUD",
+    "data": "{
+        \"message\":\"Price stream unavailable.\"
+        }"
+}
+
+# Heartbeat neglect
+{"type":"message","channel":"","data":"{\"ok\": \"ok\"}"}
+
+```
+
+#### 2.  Subscribe Order updates or transaction records
+
+
+<!--websocket url:   wss://dma-uat-ws.defi.wiki/v2/ws/GetOrdersInfo-->
+
+```
+orders_connect = websocket.get_orders()
+
+while True:
+    # Get  messages
+    message = websocket.get_message(orders_connect)
+
+    print(f"Receiving message from server: \n{message}")
+
+```
+
+
+请求参数:
+
+
+| Parameter     | required | data type | describe                | Value range |
+|---------------|----------|-----------|-------------------------|-------------|
+| api_key       | true     | string    | key                     |             |
+| signature     | true     | long      | Cryptographic signature |             |
+| data_type     | true     | string    | Subscribed Channels     | order,trade |
+
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+wss://dma-uat-ws.defi.wiki/v2/ws/GetOrdersInfo?api_key=***&signature=***&data_type=order,trade
+
+```
+
+
+channel: dma_order_info 响应数据:
+
+
+| Parameter             | required   | data type | describe      | Value range                    |
+|-----------------------|------------|-----------|---------------|--------------------------------|
+| type                  | true       | long      | type          |                                |
+| channel               | true       | string    | channel       | dma_order_info、dma_trader_info |
+| data                  | true       | jsonstr   | data          |                                |
+| data['OrderId']       | true       | str       | OrderId       |                                |
+| data['ClientOrderId'] | true       | str       | ClientOrderId |                                |
+| data['TxnAlias']      | true       | str       | TxnAlias      |                                |
+| data['TransferId']    | true       | str       | TransferId    |                                |
+| data['Symbol']        | true       | str       | Symbol        |                                |
+| data['Type']          | true       | str       | Type          |                                |
+| data['TimeInForce']   | true       | str       | TimeInForce   |                                |
+| data['Side']          | true       | str       | Side          |                                |
+| data['OrderId']       | true       | str       | OrderId       |                                |
+| data['Price']         | true       | str       | Price         |                                |
+| data['AveragePrice']  | true       | str       | AveragePrice  |                                |
+| data['Amount']        | true       | str       | Amount        |                                |
+| data['CreatedAt']     | true       | str       | CreatedAt     |                                |
+| data['UpdatedAt']     | true       | str       | UpdatedAt     |                                |
+| data['AccountId']     | true       | str       | AccountId     |                                |
+| data['VaultId']       | true       | str       | VaultId       |                                |
+| data['Note']          | true       | str       | Note          |                                |
+| data['Status']        | true       | str       | Status        |                                |
+| data['Average']       | true       | str       | Average       |                                |
+| data['Filled']        | true       | str       | Filled        |                                |
+| data['Remaining']     | true       | str       | Remaining     |                                |
+| data['Cost']          | true       | str       | Cost          |                                |
+| data['ExecPrice']     | true       | str       | ExecPrice     |                                |
+| data['OrderFrom']     | true       | str       | OrderFrom     |                                |
+
+
+响应例子:
+
+```
+
+{
+    "type":"message",
+    "channel":"dma_order_info",
+    "data":"{
+        \"OrderId\":\"d8be1f41-9e8e-4af0-899b-c1334916aa0e\",
+        \"ClientOrderId\":\"e7f80d34-0d80-4256-9de3-cd37310a55da\",
+        \"TxnAlias\":\"\",
+        \"TransferId\":\"\",
+        \"Symbol\":\"USDT/AUD\",
+        \"Type\":\"market\",
+        \"TimeInForce\":\"FOK\",
+        \"Side\":\"sell\",
+        \"Price\":\"1000\",
+        \"AveragePrice\":\"\",
+        \"Amount\":\"1000\",
+        \"CreatedAt\":1690538950000,
+        \"UpdatedAt\":1690538950000,
+        \"AccountId\":\"1ca36d2b-2103-45c7-a2e3-3b90825ba1b2\",
+        \"VaultId\":\"5175\",
+        \"Note\":\"yyy_test_create_order\",
+        \"Status\":\"open\",
+        \"Average\":\"0\",
+        \"Filled\":\"0\",
+        \"Remaining\":\"1000\",
+        \"Cost\":\"1000000\",
+        \"ExecPrice\":\"\",
+        \"OrderFrom\":\"coinroutes\"
+    }"
+}
+
+```
+
+channel: dma_trader_info 响应数据:
+
+
+| Parameter            | required   | data type | describe     | Value range                    |
+|----------------------|------------|-----------|--------------|--------------------------------|
+| type                 | true       | long      | type         |                                |
+| channel              | true       | string    | channel      | dma_order_info、dma_trader_info |
+| data                 | true       | jsonstr   | data         |                                |
+| data['id']           | true       | str       | id           |                                |
+| data['timestamp']    | true       | str       | timestamp    |                                |
+| data['datetime']     | true       | str       | datetime     |                                |
+| data['symbol']       | true       | str       | symbol       |                                |
+| data['order']        | true       | str       | order        |                                |
+| data['type']         | true       | str       | type         |                                |
+| data['side']         | true       | str       | side         |                                |
+| data['takerOrMaker'] | true       | str       | takerOrMaker |                                |
+| data['price']        | true       | str       | price        |                                |
+| data['amount']       | true       | str       | amount       |                                |
+| data['cost']         | true       | str       | cost         |                                |
+| data['orderFrom']    | true       | str       | orderFrom    |                                |
+
+
+响应例子:
+
+```
+
+{
+    "type":"message",
+    "pattern":null,
+    "channel":"dma_trade_info",
+    "data":"{
+        \"id\":\"60e2e941-070c-40e3-b2ef-4a8f6ad9f316\",
+        \"timestamp\":\"1690767892000\",
+        \"datetime\":\"2023-07-31 01:44:52\",
+        \"symbol\":\"USDT/AUD\",
+        \"order\":\"41969863-1f32-4eaa-b679-a5b0e6fb5542\",
+        \"type\":\"market\",
+        \"side\":\"sell\",
+        \"takerOrMaker\":\"taker\",
+        \"price\":\"1.662902412\",
+        \"amount\":\"101\",
+        \"cost\":\"167.9531436\",
+        \"orderFrom\":\"coinroutes\"
+    }"
+}
+
+```
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.9 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
@@ -98,22 +98,23 @@
 messages message = websocket.get_message(market_connect) print(f"Receiving
 message from server: \n{message}") ``` è¯·æ±åæ°: | Parameter | required |
 data type | describe | Value range | |---------------|----------|-----------|--
 -----------------------|-------------| | api_key | true | string | key | | |
 signature | true | long | Cryptographic signature | | | data_type | true |
 string | Subscribed Channels | price |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
-wss://dma-api.defi.wiki/ws/GetMarket?api_key=***&signature=***&data_type=price
-``` ååºæ°æ®: | Parameter | required | data type | describe | Value range |
-|--------------------|----------|-----------|---------------|------------------
---| | type | true | long | type | | | channel | true | string | channel |
-dma_price_USDT/AUD | | data | true | jsonstr | data | | | data['sell_price'] |
-true | string | sell price | | | data['buy_price'] | true | string | buy price
-| | | data['datetime'] | true | string | time | | | data['timestamp'] | true |
-string | time | | | message | false | string | description | Is price open |
+wss://dma-uat-ws.defi.wiki/v2/ws/
+GetMarket?api_key=***&signature=***&data_type=price ``` ååºæ°æ®: |
+Parameter | required | data type | describe | Value range | |------------------
+--|----------|-----------|---------------|--------------------| | type | true |
+long | type | | | channel | true | string | channel | dma_price_USDT/AUD | |
+data | true | jsonstr | data | | | data['sell_price'] | true | string | sell
+price | | | data['buy_price'] | true | string | buy price | | | data
+['datetime'] | true | string | time | | | data['timestamp'] | true | string |
+time | | | message | false | string | description | Is price open |
 ååºä¾å­: ``` { "type": "message", "channel": "dma_price_USDT/AUD", "data":
 "{ \"sell_price\": \"1.322544321902561296\", \"buy_price\":
 \"1.668209315127094362\", \"datetime\": \"2023-07-28 10:03:40\", \"timestamp\":
 \"1690538620.1056492\" }" } { "type": "message", "channel": "dma_price_USDT/
 AUD", "data": "{ \"message\":\"Price stream unavailable.\" }" } # Heartbeat
 neglect {"type":"message","channel":"","data":"{\"ok\": \"ok\"}"} ``` #### 2.
 Subscribe Order updates or transaction records  ``` orders_connect =
@@ -121,15 +122,15 @@
 websocket.get_message(orders_connect) print(f"Receiving message from server: \n
 {message}") ``` è¯·æ±åæ°: | Parameter | required | data type | describe |
 Value range | |---------------|----------|-----------|-------------------------
 |-------------| | api_key | true | string | key | | | signature | true | long |
 Cryptographic signature | | | data_type | true | string | Subscribed Channels |
 order,trade |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
-wss://dma-api.defi.wiki/ws/
+wss://dma-uat-ws.defi.wiki/v2/ws/
 GetOrdersInfo?api_key=***&signature=***&data_type=order,trade ``` channel:
 dma_order_info ååºæ°æ®: | Parameter | required | data type | describe |
 Value range | |-----------------------|------------|-----------|---------------
 |--------------------------------| | type | true | long | type | | | channel |
 true | string | channel | dma_order_infoãdma_trader_info | | data | true |
 jsonstr | data | | | data['OrderId'] | true | str | OrderId | | | data
 ['ClientOrderId'] | true | str | ClientOrderId | | | data['TxnAlias'] | true |
```

### Comparing `zerocap_api_new_test-0.1.8/README.rst` & `zerocap_api_new_test-0.1.9/README.rst`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,464 +1,464 @@
-# zerocap-api-test 
-
-# <a href="#testapi">Jump restapi</a>
-# <a href="#test">Jump websocket</a>
-
-
-
-```
-
-描述介绍
-
-sdk install
-pip install zerocap-api-test
-。
-。
-。
-
-```
-
-
-
-# <a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi </a>
-get https://dma-api.defi.wiki/redoc
-
-
-
-#### 1. Create an order
-post https://dma-api.defi.wiki/orders/create_order
-
-
-
-请求参数:
-
-| Parameter       | required  | data type | describe        | Value range  |
-|-----------------|-----------|-----------|-----------------|--------------|
-| symbol          | true      | string    | Instrument      | USDT/AUD     |
-| side            | true      | string    | Side            | buy sell     |
-| type            | true      | string    | Type            | market limit |
-| amount          | true      | string    | Quantity        |              |
-| price           | true      | string    | Price           |              |
-| client_order_id | true      | string    | Client order id |              |
-| account_vault   | true      | json      | accountVault    |              |
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-{
-    "symbol": "USDT/AUD",
-    "side": "buy",
-    "type": "market",
-    "amount": "1000",
-    "price": "1000",
-    "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
-    "account_vault": {
-        "third_identity_id": "918d7125916c13191f3674e",
-        "api_key": "***",
-        "signature": "***",
-        "note": ""
-    }
-}
-
-```
-
-响应数据:
-
-| Parameter          | required | data type | describe        | Value range |
-|--------------------|----------|-----------|-----------------|-------------|
-| id                 | true     | long      | Transaction ID  |             |
-| clientOrderId      | true     | string    | Client order id |             |
-| datatime           | true     | string    | Time            |             |
-| timestamp          | true     | string    | Time            |             |
-| lastTradeTimestamp | true     | long      | Time            |             |
-| status             | true     | string    | Status          |             |
-| type               | true     | string    | Type            |             |
-| timeInForce        | true     | string    | timeInForce     |             |
-| side               | true     | string    | Side            |             |
-| price              | true     | string    | Price           |             |
-| average            | true     | string    | average         |             |
-| amount             | true     | string    | Quantity        |             |
-| filled             | true     | string    | filled          |             |
-| remaining          | true     | string    | remaining       |             |
-| cost               | true     | string    | cost            |             |
-| transferId         | true     | string    | transferId      |             |
-| trades             | true     | string    | trades          |             |
-
-
-响应例子:
-
-```
-
- {
-    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
-    "clientOrderId": "e7f80d34-0d80-4256-9de3-cd37310a55dabe",
-    "datatime": "2023-07-28 09:19:45",
-    "timestamp": "1690535984000",
-    "lastTradeTimestamp": "1690535984000",
-    "status": "closed",
-    "symbol": "USDT/AUD",
-    "type": "Market",
-    "timeInForce": "FOK",
-    "side": "buy",
-    "price": "21.1",
-    "average": "1.685133171",
-    "amount": "9",
-    "filled": "9",
-    "remaining": "0",
-    "cost": "15.16619854",
-    "transferId": "12424971-f51d-4144-a205-9e306eb6351c",
-    "trades": [
-        {
-            "id": "12424971-f51d-4144-a205-9e306eb6351c",
-            "timestamp": "1690535984000",
-            "datetime": "2023-07-28 09:19:45",
-            "symbol": "USDT/AUD",
-            "order": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
-            "type": "market",
-            "side": "buy",
-            "takerOrMaker": "taker",
-            "price": "1.685133171",
-            "amount": "9",
-            "cost": "15.16619854",
-            "orderFrom": "coinroutes"
-        }
-    ]
-}
-
-```
-
-
-
-
-#### 2. Fetch specific orders
-post https://dma-api.defi.wiki/orders/fetch_order
-
-
-请求参数:
-
-
-| Parameter       | required | data type | describe       | Value range  |
-|-----------------|----------|-----------|----------------|--------------|
-| id              | true     | string    | Transaction ID |              |
-| account_vault   | true     | json      | accountVault   |              |
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-{
-    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
-    "account_vault": {
-        "third_identity_id": "918d7125916c13191f3674e",
-        "api_key": "***",
-        "signature": "***",
-        "note": ""
-    }
-}
-
-```
-
-响应数据 接口报错 待定:
-
-
-| Parameter     | required | data type | describe       | Value range |
-|---------------|----------|-----------|----------------|-------------|
-| id            | true     | string    | Transaction ID |             |
-| account_vault | true     | json      | accountVault   |             |
-
-
-响应例子:
-
-```
-
-{
-	"id": "5e24b0e6-c5c9-42fa-b998-91eff88cb599",
-	"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310234",
-	"datatime": "2023-07-31 02:10:45",
-	"timestamp": "1690769444000",
-	"last_trade_timestamp": "1690769444000",
-	"status": "closed",
-	"symbol": "USDT/AUD",
-	"type": "Market",
-	"time_in_force": "FOK",
-	"side": "sell",
-	"price": "1",
-	"average": "1.319611568",
-	"amount": "500",
-	"filled": "500",
-	"remaining": "0",
-	"cost": "659.8057838",
-	"transfer_id": "cd8f809d-19bb-4014-8814-ec59cdf54136",
-	"fee": "",
-	"trades": [
-		{
-			"id": "cd8f809d-19bb-4014-8814-ec59cdf54136",
-			"timestamp": "1690769444000",
-			"datetime": "2023-07-31 02:10:45",
-			"symbol": "USDT/AUD",
-			"order": "5e24b0e6-c5c9-42fa-b998-91eff88cb599",
-			"type": "market",
-			"side": "sell",
-			"taker_or_maker": "taker",
-			"price": "1.319611568",
-			"amount": "500",
-			"cost": "659.8057838",
-			"order_from": "coinroutes",
-			"fee": "",
-			"fees": ""
-		}
-	]
-}
-
-```
-
-
-#### 3. Batch fetch order
-post https://dma-api.defi.wiki/orders/fetch_orders
-
-
-
-请求参数:
-
-| Parameter      | required | data type | describe        | Value range |
-|----------------|----------|-----------|-----------------|-------------|
-| symbol         | true     | string    | symbol          |             |
-| start_datetime | true     | string    | start_datetime  |             |
-| end_datetime   | true     | string    | end_datetime    |             |
-| page           | true     | string    | page            |             |
-| limit          | true     | string    | limit           |             |
-| ids            | true     | string    | Transaction ids |             |
-| status         | true     | string    | status          |             |
-| sort_order     | true     | string    | sort_order      |             |
-| order_type     | true     | string    | order_type      |             |
-| side           | true     | string    | side            |             |
-| account_vau lt | true     | j son     | accountVault    |             |
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-{
-    "symbol": "",
-    "start_datetime": 0,
-    "end_datetime": 0,
-    "page": 0,
-    "limit": 0,
-    "ids": "",
-    "status": "",
-    "sort_order": "",
-    "order_type": "",
-    "side": "",
-    "account_vault": {
-        "third_identity_id": "918d7125916c13191f3674e",
-        "api_key": "***",
-        "signature": "***",
-        "note": ""
-    }
-}
-
-```
-
-响应数据 接口报错 待定:
-
-
-
-| Parameter     | required | data type | describe       | Value range |
-|---------------|----------|-----------|----------------|-------------|
-| id            | true     | string    | Transaction ID |             |
-| account_vault | true     | json      |  accountVault  |             |
-
-
-
-响应例子:
-
-```
-
-{
-	"order_list": [
-		{
-			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
-			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
-			"datatime": "2023-07-31 02:12:23",
-			"timestamp": "1690516007000",
-			"last_trade_timestamp": "1690516007000",
-			"status": "rejected",
-			"symbol": "USDT/AUD",
-			"type": "market",
-			"time_in_force": "FOK",
-			"side": "buy",
-			"price": "1000",
-			"average": "",
-			"amount": "1000",
-			"filled": "",
-			"remaining": "",
-			"cost": "",
-			"transfer_id": "",
-			"fee": "",
-			"trades": []
-		}
-	],
-	"status": "success",
-	"total": 3864,
-	"page": "1"
-}
-
-```
-
-
-
-## <span id='test'>websocket</span>
-
-#### 1. Subscribe to Market data
-
-
-websocket wss://dma-api.defi.wiki/ws/GetMarket
-
-
-
-请求参数:
-
-| Parameter     | required | data type | describe                | Value range |
-|---------------|----------|-----------|-------------------------|-------------|
-| api_key       | true     | string    | key                     |             |
-| signature     | true     | long      | Cryptographic signature |             |
-| data_type     | true     | string    | Subscribed Channels     | price       |
-
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-wss://dma-api.defi.wiki/ws/GetMarket?api_key=coinroutes&signature=2585311b823982b325b266e132cd8cdf88d190ca61706dda5a67d421b23005df&data_type=price
-
-```
-
-
-响应数据:
-
-
-| Parameter            | required | data type | describe | Value range        |
-|----------------------|----------|-----------|----------|--------------------|
-| type                 | true     | long      | type     |                    |
-| channel              | true     | string    | channel  | dma_price_USDT/AUD |
-| data                 | true     | jsonstr   | data     |                    |
-| data['sell_price']   | true     | string    | data     | sell price         |
-| data['buy_price']    | true     | string    | data     | buy price          |
-| data['datetime']     | true     | string    | data     | time               |
-| data['timestamp']    | true     | string    | data     | time               |
-
-
-响应例子:
-
-```
-
-{
-    "type": "message",
-    "channel": "dma_price_USDT/AUD",
-    "data": "{
-        \"sell_price\": \"1.322544321902561296\",
-        \"buy_price\": \"1.668209315127094362\",
-        \"datetime\": \"2023-07-28 10:03:40\",
-        \"timestamp\": \"1690538620.1056492\"
-        }"
-}
-
-```
-
-#### 2.  Subscribe Order updates or transaction records
-
-
-websocket wss://dma-api.defi.wiki/ws/GetOrdersInfo
-
-
-
-请求参数:
-
-
-| Parameter     | required | data type | describe                | Value range |
-|---------------|----------|-----------|-------------------------|-------------|
-| api_key       | true     | string    | key                     |             |
-| signature     | true     | long      | Cryptographic signature |             |
-| data_type     | true     | string    | Subscribed Channels     | order,trade |
-
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-wss://dma-api.defi.wiki/ws/GetOrdersInfo?api_key=coinroutes&signature=2585311b823982b325b266e132cd8cdf88d190ca61706dda5a67d421b23005df&data_type=order,trade
-
-```
-
-
-dma_order_info 响应数据:
-
-
-| Parameter             | required   | data type | describe      | Value range                    |
-|-----------------------|------------|-----------|---------------|--------------------------------|
-| type                  | true       | long      | type          |                                |
-| channel               | true       | string    | channel       | dma_order_info dma_trader_info |
-| data                  | true       | jsonstr   | data          |                                |
-| data['OrderId']       | true       | str       | OrderId       |                                |
-| data['ClientOrderId'] | true       | str       | ClientOrderId |                                |
-| data['TxnAlias']      | true       | str       | TxnAlias      |                                |
-| data['TransferId']    | true       | str       | TransferId    |                                |
-| data['Symbol']        | true       | str       | Symbol        |                                |
-| data['Type']          | true       | str       | Type          |                                |
-| data['TimeInForce']   | true       | str       | TimeInForce   |                                |
-| data['Side']          | true       | str       | Side          |                                |
-| data['OrderId']       | true       | str       | OrderId       |                                |
-| data['Price']         | true       | str       | Price         |                                |
-| data['AveragePrice']  | true       | str       | AveragePrice  |                                |
-| data['Amount']        | true       | str       | Amount        |                                |
-| data['CreatedAt']     | true       | str       | CreatedAt     |                                |
-| data['UpdatedAt']     | true       | str       | UpdatedAt     |                                |
-| data['AccountId']     | true       | str       | AccountId     |                                |
-| data['VaultId']       | true       | str       | VaultId       |                                |
-| data['Note']          | true       | str       | Note          |                                |
-| data['Status']        | true       | str       | Status        |                                |
-| data['Average']       | true       | str       | Average       |                                |
-| data['Filled']        | true       | str       | Filled        |                                |
-| data['Remaining']     | true       | str       | Remaining     |                                |
-| data['Cost']          | true       | str       | Cost          |                                |
-| data['ExecPrice']     | true       | str       | ExecPrice     |                                |
-| data['OrderFrom']     | true       | str       | OrderFrom     |                                |
-
-
-响应例子:
-
-```
-
-{
-    "type":"message",
-    "channel":"dma_order_info",
-    "data":"{
-        \"OrderId\":\"d8be1f41-9e8e-4af0-899b-c1334916aa0e\",
-        \"ClientOrderId\":\"e7f80d34-0d80-4256-9de3-cd37310a55da\",
-        \"TxnAlias\":\"\",
-        \"TransferId\":\"\",
-        \"Symbol\":\"USDT/AUD\",
-        \"Type\":\"market\",
-        \"TimeInForce\":\"FOK\",
-        \"Side\":\"sell\",
-        \"Price\":\"1000\",
-        \"AveragePrice\":\"\",
-        \"Amount\":\"1000\",
-        \"CreatedAt\":1690538950000,
-        \"UpdatedAt\":1690538950000,
-        \"AccountId\":\"1ca36d2b-2103-45c7-a2e3-3b90825ba1b2\",
-        \"VaultId\":\"5175\",
-        \"Note\":\"yyy_test_create_order\",
-        \"Status\":\"open\",
-        \"Average\":\"0\",
-        \"Filled\":\"0\",
-        \"Remaining\":\"1000\",
-        \"Cost\":\"1000000\",
-        \"ExecPrice\":\"\",
-        \"OrderFrom\":\"coinroutes\
-    "}"
-}
-
-```
-
-
+# zerocap-api-test 
+
+# <a href="#testapi">Jump restapi</a>
+# <a href="#test">Jump websocket</a>
+
+
+
+```
+
+描述介绍
+
+sdk install
+pip install zerocap-api-test
+。
+。
+。
+
+```
+
+
+
+# <a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi </a>
+get https://dma-api.defi.wiki/redoc
+
+
+
+#### 1. Create an order
+post https://dma-api.defi.wiki/orders/create_order
+
+
+
+请求参数:
+
+| Parameter       | required  | data type | describe        | Value range  |
+|-----------------|-----------|-----------|-----------------|--------------|
+| symbol          | true      | string    | Instrument      | USDT/AUD     |
+| side            | true      | string    | Side            | buy sell     |
+| type            | true      | string    | Type            | market limit |
+| amount          | true      | string    | Quantity        |              |
+| price           | true      | string    | Price           |              |
+| client_order_id | true      | string    | Client order id |              |
+| account_vault   | true      | json      | accountVault    |              |
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+{
+    "symbol": "USDT/AUD",
+    "side": "buy",
+    "type": "market",
+    "amount": "1000",
+    "price": "1000",
+    "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+    "account_vault": {
+        "third_identity_id": "918d7125916c13191f3674e",
+        "api_key": "***",
+        "signature": "***",
+        "note": ""
+    }
+}
+
+```
+
+响应数据:
+
+| Parameter          | required | data type | describe        | Value range |
+|--------------------|----------|-----------|-----------------|-------------|
+| id                 | true     | long      | Transaction ID  |             |
+| clientOrderId      | true     | string    | Client order id |             |
+| datatime           | true     | string    | Time            |             |
+| timestamp          | true     | string    | Time            |             |
+| lastTradeTimestamp | true     | long      | Time            |             |
+| status             | true     | string    | Status          |             |
+| type               | true     | string    | Type            |             |
+| timeInForce        | true     | string    | timeInForce     |             |
+| side               | true     | string    | Side            |             |
+| price              | true     | string    | Price           |             |
+| average            | true     | string    | average         |             |
+| amount             | true     | string    | Quantity        |             |
+| filled             | true     | string    | filled          |             |
+| remaining          | true     | string    | remaining       |             |
+| cost               | true     | string    | cost            |             |
+| transferId         | true     | string    | transferId      |             |
+| trades             | true     | string    | trades          |             |
+
+
+响应例子:
+
+```
+
+ {
+    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
+    "clientOrderId": "e7f80d34-0d80-4256-9de3-cd37310a55dabe",
+    "datatime": "2023-07-28 09:19:45",
+    "timestamp": "1690535984000",
+    "lastTradeTimestamp": "1690535984000",
+    "status": "closed",
+    "symbol": "USDT/AUD",
+    "type": "Market",
+    "timeInForce": "FOK",
+    "side": "buy",
+    "price": "21.1",
+    "average": "1.685133171",
+    "amount": "9",
+    "filled": "9",
+    "remaining": "0",
+    "cost": "15.16619854",
+    "transferId": "12424971-f51d-4144-a205-9e306eb6351c",
+    "trades": [
+        {
+            "id": "12424971-f51d-4144-a205-9e306eb6351c",
+            "timestamp": "1690535984000",
+            "datetime": "2023-07-28 09:19:45",
+            "symbol": "USDT/AUD",
+            "order": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
+            "type": "market",
+            "side": "buy",
+            "takerOrMaker": "taker",
+            "price": "1.685133171",
+            "amount": "9",
+            "cost": "15.16619854",
+            "orderFrom": "coinroutes"
+        }
+    ]
+}
+
+```
+
+
+
+
+#### 2. Fetch specific orders
+post https://dma-api.defi.wiki/orders/fetch_order
+
+
+请求参数:
+
+
+| Parameter       | required | data type | describe       | Value range  |
+|-----------------|----------|-----------|----------------|--------------|
+| id              | true     | string    | Transaction ID |              |
+| account_vault   | true     | json      | accountVault   |              |
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+{
+    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
+    "account_vault": {
+        "third_identity_id": "918d7125916c13191f3674e",
+        "api_key": "***",
+        "signature": "***",
+        "note": ""
+    }
+}
+
+```
+
+响应数据 接口报错 待定:
+
+
+| Parameter     | required | data type | describe       | Value range |
+|---------------|----------|-----------|----------------|-------------|
+| id            | true     | string    | Transaction ID |             |
+| account_vault | true     | json      | accountVault   |             |
+
+
+响应例子:
+
+```
+
+{
+	"id": "5e24b0e6-c5c9-42fa-b998-91eff88cb599",
+	"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310234",
+	"datatime": "2023-07-31 02:10:45",
+	"timestamp": "1690769444000",
+	"last_trade_timestamp": "1690769444000",
+	"status": "closed",
+	"symbol": "USDT/AUD",
+	"type": "Market",
+	"time_in_force": "FOK",
+	"side": "sell",
+	"price": "1",
+	"average": "1.319611568",
+	"amount": "500",
+	"filled": "500",
+	"remaining": "0",
+	"cost": "659.8057838",
+	"transfer_id": "cd8f809d-19bb-4014-8814-ec59cdf54136",
+	"fee": "",
+	"trades": [
+		{
+			"id": "cd8f809d-19bb-4014-8814-ec59cdf54136",
+			"timestamp": "1690769444000",
+			"datetime": "2023-07-31 02:10:45",
+			"symbol": "USDT/AUD",
+			"order": "5e24b0e6-c5c9-42fa-b998-91eff88cb599",
+			"type": "market",
+			"side": "sell",
+			"taker_or_maker": "taker",
+			"price": "1.319611568",
+			"amount": "500",
+			"cost": "659.8057838",
+			"order_from": "coinroutes",
+			"fee": "",
+			"fees": ""
+		}
+	]
+}
+
+```
+
+
+#### 3. Batch fetch order
+post https://dma-api.defi.wiki/orders/fetch_orders
+
+
+
+请求参数:
+
+| Parameter      | required | data type | describe        | Value range |
+|----------------|----------|-----------|-----------------|-------------|
+| symbol         | true     | string    | symbol          |             |
+| start_datetime | true     | string    | start_datetime  |             |
+| end_datetime   | true     | string    | end_datetime    |             |
+| page           | true     | string    | page            |             |
+| limit          | true     | string    | limit           |             |
+| ids            | true     | string    | Transaction ids |             |
+| status         | true     | string    | status          |             |
+| sort_order     | true     | string    | sort_order      |             |
+| order_type     | true     | string    | order_type      |             |
+| side           | true     | string    | side            |             |
+| account_vau lt | true     | j son     | accountVault    |             |
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+{
+    "symbol": "",
+    "start_datetime": 0,
+    "end_datetime": 0,
+    "page": 0,
+    "limit": 0,
+    "ids": "",
+    "status": "",
+    "sort_order": "",
+    "order_type": "",
+    "side": "",
+    "account_vault": {
+        "third_identity_id": "918d7125916c13191f3674e",
+        "api_key": "***",
+        "signature": "***",
+        "note": ""
+    }
+}
+
+```
+
+响应数据 接口报错 待定:
+
+
+
+| Parameter     | required | data type | describe       | Value range |
+|---------------|----------|-----------|----------------|-------------|
+| id            | true     | string    | Transaction ID |             |
+| account_vault | true     | json      |  accountVault  |             |
+
+
+
+响应例子:
+
+```
+
+{
+	"order_list": [
+		{
+			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
+			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+			"datatime": "2023-07-31 02:12:23",
+			"timestamp": "1690516007000",
+			"last_trade_timestamp": "1690516007000",
+			"status": "rejected",
+			"symbol": "USDT/AUD",
+			"type": "market",
+			"time_in_force": "FOK",
+			"side": "buy",
+			"price": "1000",
+			"average": "",
+			"amount": "1000",
+			"filled": "",
+			"remaining": "",
+			"cost": "",
+			"transfer_id": "",
+			"fee": "",
+			"trades": []
+		}
+	],
+	"status": "success",
+	"total": 3864,
+	"page": "1"
+}
+
+```
+
+
+
+## <span id='test'>websocket</span>
+
+#### 1. Subscribe to Market data
+
+
+websocket wss://dma-api.defi.wiki/ws/GetMarket
+
+
+
+请求参数:
+
+| Parameter     | required | data type | describe                | Value range |
+|---------------|----------|-----------|-------------------------|-------------|
+| api_key       | true     | string    | key                     |             |
+| signature     | true     | long      | Cryptographic signature |             |
+| data_type     | true     | string    | Subscribed Channels     | price       |
+
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+wss://dma-api.defi.wiki/ws/GetMarket?api_key=coinroutes&signature=2585311b823982b325b266e132cd8cdf88d190ca61706dda5a67d421b23005df&data_type=price
+
+```
+
+
+响应数据:
+
+
+| Parameter            | required | data type | describe | Value range        |
+|----------------------|----------|-----------|----------|--------------------|
+| type                 | true     | long      | type     |                    |
+| channel              | true     | string    | channel  | dma_price_USDT/AUD |
+| data                 | true     | jsonstr   | data     |                    |
+| data['sell_price']   | true     | string    | data     | sell price         |
+| data['buy_price']    | true     | string    | data     | buy price          |
+| data['datetime']     | true     | string    | data     | time               |
+| data['timestamp']    | true     | string    | data     | time               |
+
+
+响应例子:
+
+```
+
+{
+    "type": "message",
+    "channel": "dma_price_USDT/AUD",
+    "data": "{
+        \"sell_price\": \"1.322544321902561296\",
+        \"buy_price\": \"1.668209315127094362\",
+        \"datetime\": \"2023-07-28 10:03:40\",
+        \"timestamp\": \"1690538620.1056492\"
+        }"
+}
+
+```
+
+#### 2.  Subscribe Order updates or transaction records
+
+
+websocket wss://dma-api.defi.wiki/ws/GetOrdersInfo
+
+
+
+请求参数:
+
+
+| Parameter     | required | data type | describe                | Value range |
+|---------------|----------|-----------|-------------------------|-------------|
+| api_key       | true     | string    | key                     |             |
+| signature     | true     | long      | Cryptographic signature |             |
+| data_type     | true     | string    | Subscribed Channels     | order,trade |
+
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+wss://dma-api.defi.wiki/ws/GetOrdersInfo?api_key=coinroutes&signature=2585311b823982b325b266e132cd8cdf88d190ca61706dda5a67d421b23005df&data_type=order,trade
+
+```
+
+
+dma_order_info 响应数据:
+
+
+| Parameter             | required   | data type | describe      | Value range                    |
+|-----------------------|------------|-----------|---------------|--------------------------------|
+| type                  | true       | long      | type          |                                |
+| channel               | true       | string    | channel       | dma_order_info dma_trader_info |
+| data                  | true       | jsonstr   | data          |                                |
+| data['OrderId']       | true       | str       | OrderId       |                                |
+| data['ClientOrderId'] | true       | str       | ClientOrderId |                                |
+| data['TxnAlias']      | true       | str       | TxnAlias      |                                |
+| data['TransferId']    | true       | str       | TransferId    |                                |
+| data['Symbol']        | true       | str       | Symbol        |                                |
+| data['Type']          | true       | str       | Type          |                                |
+| data['TimeInForce']   | true       | str       | TimeInForce   |                                |
+| data['Side']          | true       | str       | Side          |                                |
+| data['OrderId']       | true       | str       | OrderId       |                                |
+| data['Price']         | true       | str       | Price         |                                |
+| data['AveragePrice']  | true       | str       | AveragePrice  |                                |
+| data['Amount']        | true       | str       | Amount        |                                |
+| data['CreatedAt']     | true       | str       | CreatedAt     |                                |
+| data['UpdatedAt']     | true       | str       | UpdatedAt     |                                |
+| data['AccountId']     | true       | str       | AccountId     |                                |
+| data['VaultId']       | true       | str       | VaultId       |                                |
+| data['Note']          | true       | str       | Note          |                                |
+| data['Status']        | true       | str       | Status        |                                |
+| data['Average']       | true       | str       | Average       |                                |
+| data['Filled']        | true       | str       | Filled        |                                |
+| data['Remaining']     | true       | str       | Remaining     |                                |
+| data['Cost']          | true       | str       | Cost          |                                |
+| data['ExecPrice']     | true       | str       | ExecPrice     |                                |
+| data['OrderFrom']     | true       | str       | OrderFrom     |                                |
+
+
+响应例子:
+
+```
+
+{
+    "type":"message",
+    "channel":"dma_order_info",
+    "data":"{
+        \"OrderId\":\"d8be1f41-9e8e-4af0-899b-c1334916aa0e\",
+        \"ClientOrderId\":\"e7f80d34-0d80-4256-9de3-cd37310a55da\",
+        \"TxnAlias\":\"\",
+        \"TransferId\":\"\",
+        \"Symbol\":\"USDT/AUD\",
+        \"Type\":\"market\",
+        \"TimeInForce\":\"FOK\",
+        \"Side\":\"sell\",
+        \"Price\":\"1000\",
+        \"AveragePrice\":\"\",
+        \"Amount\":\"1000\",
+        \"CreatedAt\":1690538950000,
+        \"UpdatedAt\":1690538950000,
+        \"AccountId\":\"1ca36d2b-2103-45c7-a2e3-3b90825ba1b2\",
+        \"VaultId\":\"5175\",
+        \"Note\":\"yyy_test_create_order\",
+        \"Status\":\"open\",
+        \"Average\":\"0\",
+        \"Filled\":\"0\",
+        \"Remaining\":\"1000\",
+        \"Cost\":\"1000000\",
+        \"ExecPrice\":\"\",
+        \"OrderFrom\":\"coinroutes\
+    "}"
+}
+
+```
+
+
```

### Comparing `zerocap_api_new_test-0.1.8/setup.py` & `zerocap_api_new_test-0.1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from distutils.core import setup
-from setuptools import find_packages, setup, Command
-import io
-import os
-import sys
-from shutil import rmtree
-
-DESCRIPTION = '****'
-here = os.path.abspath(os.path.dirname(__file__))
-  
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-REQUIRED = [
-    'requests',
-    'websocket'
-]
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-
-        sys.exit()
-
-setup(
-    name='zerocap_api_new_test',  # 包名
-    version='0.1.8',  # 版本号
-    description='zerocap_api',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='zerocap',
-    author_email='jiayu.gao@eigen.capital',
-    url='https://zerocap.com/',
-    install_requires=REQUIRED,
-    license='MIT',
-    packages=find_packages(),
-    platforms=["all"],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',  # 对python的最低版本要求
-)
+from distutils.core import setup
+from setuptools import find_packages, setup, Command
+import io
+import os
+import sys
+from shutil import rmtree
+
+DESCRIPTION = '****'
+here = os.path.abspath(os.path.dirname(__file__))
+  
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+REQUIRED = [
+    'requests',
+    'websocket'
+]
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+
+        sys.exit()
+
+setup(
+    name='zerocap_api_new_test',  # 包名
+    version='0.1.9',  # 版本号
+    description='zerocap_api',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author='zerocap',
+    author_email='jiayu.gao@eigen.capital',
+    url='https://zerocap.com/',
+    install_requires=REQUIRED,
+    license='MIT',
+    packages=find_packages(),
+    platforms=["all"],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.6',  # 对python的最低版本要求
+)
```

### Comparing `zerocap_api_new_test-0.1.8/zerocap_api_new_test/main.py` & `zerocap_api_new_test-0.1.9/zerocap_api_new_test/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-import hmac
-import json
-import hashlib
-import requests
-from websocket import create_connection
-
-
-class ZerocapWebsocketClient:
-    def __init__(self, api_key: str, api_secret: str, envion: str = 'development'):
-        self.api_key = api_key
-        self.api_secret = api_secret
-        self.market_websocket = None
-        self.order_websocket = None
-        if envion == 'development':
-            self.base_url = "wss://dma-api.defi.wiki/ws"
-            self.http_url = "https://dma-api.defi.wiki/orders"
-        else:
-            self.base_url = "*"
-            self.http_url = "*"
-        self.signature = self.hashing()
-        self.verify_identity()
-        
-    def verify_identity(self):
-        headers = {'Content-Type': 'application/json'}
-        data = {"api_key": self.api_key, "signature": self.signature}
-        url = f"{self.http_url}/api_key_signature_valid"
-        response = requests.post(url, data=json.dumps(data), headers=headers)
-        if response.status_code != 200 or response.json().get('status_code') != 200:
-            raise Exception("Authentication failed")
-        
-    def hashing(self):
-        return hmac.new(
-            self.api_secret.encode("utf-8"), self.api_key.encode("utf-8"), hashlib.sha256
-        ).hexdigest()
-
-    def get_params(self, channel: str):
-        data_type = ""
-        if channel == "orders":
-            data_type = "order,trader"
-        elif channel == "market":
-            data_type = "price"
-            
-        return {
-            "api_key": self.api_key,
-            "signature": self.signature,
-            "data_type": data_type,
-        }
-
-    def close(self, channel=None):
-        try:
-            if channel == "orders" and self.order_websocket:
-                self.order_websocket.close()
-            elif channel == "market" and self.market_websocket:
-                self.market_websocket.close()
-            else:
-                if self.order_websocket:
-                    self.order_websocket.close()
-                if self.market_websocket:
-                    self.market_websocket.close()
-        except:
-            pass
-        return
-
-    def get_message(self, ws_recv):
-        return ws_recv.__next__()
-    
-    def get_orders(self):
-        try:
-            params = self.get_params(channel="orders")
-            wss_url = f'{self.base_url}/GetOrdersInfo?api_key={params["api_key"]}&signature={params["signature"]}&data_type={params["data_type"]}'
-            self.order_websocket = create_connection(wss_url)
-            while True:
-                message = self.order_websocket.recv()
-                yield message
-        except Exception as e:
-            self.close(channel="orders")
-            raise Exception(e)
-
-    def get_market(self):
-        try:
-            params = self.get_params(channel="market")
-            wss_url = f'{self.base_url}/GetMarket?api_key={params["api_key"]}&signature={params["signature"]}&data_type={params["data_type"]}'
-            self.market_websocket = create_connection(wss_url)
-            while True:
-                message = self.market_websocket.recv()
-                yield message
-        except Exception as e:
-            self.close(channel="market")
-            raise Exception(e)
-
-
-class ZerocapRestClient:
-    def __init__(self, api_key: str, api_secret: str, envion: str = 'development'):
-        self.api_key = api_key
-        self.api_secret = api_secret
-        signature = self.encryption_api_key()
-        if envion == 'development':
-            self.base_url = "https://dma-api.defi.wiki/orders"
-        else:
-            self.base_url = ''
-        url = f"{self.base_url}/api_key_signature_valid"
-        headers = {
-            'Content-Type': 'application/json',
-        }
-        data = {
-            "api_key": self.api_key,
-            "signature": signature,
-        }
-        response = requests.post(url, data=json.dumps(data), headers=headers)
-        check_pass = False
-
-        if response.status_code == 200:
-            result = response.json()
-            if result["status_code"] ==200:
-                check_pass = True
-
-        if not check_pass:
-            raise Exception("ZerocapRestClient init fail")
-        
-    def hashing(self):
-        return hmac.new(
-            self.api_secret.encode("utf-8"), self.api_key.encode("utf-8"), hashlib.sha256
-        ).hexdigest()
-
-    def encryption_api_key(self):
-        signature = self.hashing()
-        return signature
-
-    def create_order(
-        self,
-        symbol: str, 
-        side: str, 
-        type: str, 
-        amount: str, 
-        price: str, 
-        client_order_id: str,  
-        third_identity_id: str, 
-        note: str = ''
-    ):
-        signature = self.encryption_api_key()
-        if signature == "fail":
-            raise Exception("Create Order Api Key error")
-
-        url = f"{self.base_url}/create_order"
-        headers = {
-            'Content-Type': 'application/json',
-        }
-        data = {
-            "symbol": symbol,
-            "side": side,
-            "type": type,
-            "amount": amount,
-            "price": price,
-            "client_order_id": client_order_id,
-            "account_vault": {
-                "third_identity_id": third_identity_id,
-                "api_key": self.api_key,
-                "signature": signature,
-                "note": note,
-            }
-        }
-        response = requests.post(url, data=json.dumps(data), headers=headers)
-        if response.status_code == 200:
-            res = response.json()
-            return res
-        else:
-            raise Exception(response.text)
-
-    def fetch_order(
-        self, id: str,
-        note: str = '', 
-        third_identity_id: str = ''
-    ):
-        signature = self.encryption_api_key()
-        if signature == "fail":
-            raise Exception("Fetch Order Api Key error")
-
-        url = f"{self.base_url}/fetch_order"
-        headers = {
-            'Content-Type': 'application/json',
-        }
-        data = {
-            "id": id,
-            "account_vault": {
-                "third_identity_id": third_identity_id,
-                "api_key": self.api_key,
-                "signature": signature,
-                "note": note,
-            }
-        }
-        response = requests.post(url, data=json.dumps(data), headers=headers)
-        if response.status_code == 200:
-            res = response.json()
-            return res
-        else:
-            raise Exception(response.text)
-
-    def fetch_orders(
-        self,
-        start_datetime: int,
-        end_datetime: int,
-        symbol: str = '',
-        page: int = 0,
-        limit: int = 500, 
-        ids: str = "", 
-        status: str = "", 
-        sort_order: str = "", 
-        order_type: str = "",
-        side: str = "", 
-        third_identity_id: str = "", 
-        note: str = ""
-    ):
-        signature = self.encryption_api_key()
-        if signature == "fail":
-            return "Fetch Orders Api Key error"
-
-        url = f"{self.base_url}/fetch_orders"
-        headers = {
-            'Content-Type': 'application/json',
-        }
-        data = {
-            "symbol": symbol,
-            "start_datetime": start_datetime,
-            "end_datetime": end_datetime,
-            "page": page,
-            "ids": ids,
-            "status": status,
-            "sort_order": sort_order,
-            "order_type": order_type,
-            "side": side,
-            "limit": limit,
-            "account_vault": {
-                "third_identity_id": third_identity_id,
-                "api_key": self.api_key,
-                "signature": signature,
-                "note": note,
-            }
-        }
-        response = requests.post(url, data=json.dumps(data), headers=headers)
-        if response.status_code == 200:
-            res = response.json()
-            return res
-        else:
-            raise Exception(response.text)
+import hmac
+import json
+import hashlib
+import requests
+from websocket import create_connection
+
+
+class ZerocapWebsocketClient:
+    def __init__(self, api_key: str, api_secret: str, envion: str = 'development'):
+        self.api_key = api_key
+        self.api_secret = api_secret
+        self.market_websocket = None
+        self.order_websocket = None
+        if envion == 'development':
+            self.base_url = "wss://dma-uat-ws.defi.wiki/v2/ws"
+            self.http_url = "https://dma-uat-api.defi.wiki/v2/orders"
+        else:
+            self.base_url = "*"
+            self.http_url = "*"
+        self.signature = self.hashing()
+        self.verify_identity()
+        
+    def verify_identity(self):
+        headers = {'Content-Type': 'application/json'}
+        data = {"api_key": self.api_key, "signature": self.signature}
+        url = f"{self.http_url}/api_key_signature_valid"
+        response = requests.post(url, data=json.dumps(data), headers=headers)
+        if response.status_code != 200 or response.json().get('status_code') != 200:
+            raise Exception("Authentication failed")
+        
+    def hashing(self):
+        return hmac.new(
+            self.api_secret.encode("utf-8"), self.api_key.encode("utf-8"), hashlib.sha256
+        ).hexdigest()
+
+    def get_params(self, channel: str):
+        data_type = ""
+        if channel == "orders":
+            data_type = "order,trader"
+        elif channel == "market":
+            data_type = "price"
+            
+        return {
+            "api_key": self.api_key,
+            "signature": self.signature,
+            "data_type": data_type,
+        }
+
+    def close(self, channel=None):
+        try:
+            if channel == "orders" and self.order_websocket:
+                self.order_websocket.close()
+            elif channel == "market" and self.market_websocket:
+                self.market_websocket.close()
+            else:
+                if self.order_websocket:
+                    self.order_websocket.close()
+                if self.market_websocket:
+                    self.market_websocket.close()
+        except:
+            pass
+        return
+
+    def get_message(self, ws_recv):
+        return ws_recv.__next__()
+    
+    def get_orders(self):
+        try:
+            params = self.get_params(channel="orders")
+            wss_url = f'{self.base_url}/GetOrdersInfo?api_key={params["api_key"]}&signature={params["signature"]}&data_type={params["data_type"]}'
+            self.order_websocket = create_connection(wss_url)
+            while True:
+                message = self.order_websocket.recv()
+                yield message
+        except Exception as e:
+            self.close(channel="orders")
+            raise Exception(e)
+
+    def get_market(self):
+        try:
+            params = self.get_params(channel="market")
+            wss_url = f'{self.base_url}/GetMarket?api_key={params["api_key"]}&signature={params["signature"]}&data_type={params["data_type"]}'
+            self.market_websocket = create_connection(wss_url)
+            while True:
+                message = self.market_websocket.recv()
+                yield message
+        except Exception as e:
+            self.close(channel="market")
+            raise Exception(e)
+
+
+class ZerocapRestClient:
+    def __init__(self, api_key: str, api_secret: str, envion: str = 'development'):
+        self.api_key = api_key
+        self.api_secret = api_secret
+        signature = self.encryption_api_key()
+        if envion == 'development':
+            self.base_url = "https://dma-uat-api.defi.wiki/v2/orders"
+        else:
+            self.base_url = ''
+        url = f"{self.base_url}/api_key_signature_valid"
+        headers = {
+            'Content-Type': 'application/json',
+        }
+        data = {
+            "api_key": self.api_key,
+            "signature": signature,
+        }
+        response = requests.post(url, data=json.dumps(data), headers=headers)
+        check_pass = False
+
+        if response.status_code == 200:
+            result = response.json()
+            if result["status_code"] ==200:
+                check_pass = True
+
+        if not check_pass:
+            raise Exception("ZerocapRestClient init fail")
+        
+    def hashing(self):
+        return hmac.new(
+            self.api_secret.encode("utf-8"), self.api_key.encode("utf-8"), hashlib.sha256
+        ).hexdigest()
+
+    def encryption_api_key(self):
+        signature = self.hashing()
+        return signature
+
+    def create_order(
+        self,
+        symbol: str, 
+        side: str, 
+        type: str, 
+        amount: str, 
+        price: str, 
+        client_order_id: str,  
+        third_identity_id: str, 
+        note: str = ''
+    ):
+        signature = self.encryption_api_key()
+        if signature == "fail":
+            raise Exception("Create Order Api Key error")
+
+        url = f"{self.base_url}/create_order"
+        headers = {
+            'Content-Type': 'application/json',
+        }
+        data = {
+            "symbol": symbol,
+            "side": side,
+            "type": type,
+            "amount": amount,
+            "price": price,
+            "client_order_id": client_order_id,
+            "account_vault": {
+                "third_identity_id": third_identity_id,
+                "api_key": self.api_key,
+                "signature": signature,
+                "note": note,
+            }
+        }
+        response = requests.post(url, data=json.dumps(data), headers=headers)
+        if response.status_code == 200:
+            res = response.json()
+            return res
+        else:
+            raise Exception(response.text)
+
+    def fetch_order(
+        self, id: str,
+        note: str = '', 
+        third_identity_id: str = ''
+    ):
+        signature = self.encryption_api_key()
+        if signature == "fail":
+            raise Exception("Fetch Order Api Key error")
+
+        url = f"{self.base_url}/fetch_order"
+        headers = {
+            'Content-Type': 'application/json',
+        }
+        data = {
+            "id": id,
+            "account_vault": {
+                "third_identity_id": third_identity_id,
+                "api_key": self.api_key,
+                "signature": signature,
+                "note": note,
+            }
+        }
+        response = requests.post(url, data=json.dumps(data), headers=headers)
+        if response.status_code == 200:
+            res = response.json()
+            return res
+        else:
+            raise Exception(response.text)
+
+    def fetch_orders(
+        self,
+        start_datetime: int,
+        end_datetime: int,
+        symbol: str = '',
+        page: int = 0,
+        limit: int = 500, 
+        ids: str = "", 
+        status: str = "", 
+        sort_order: str = "", 
+        order_type: str = "",
+        side: str = "", 
+        third_identity_id: str = "", 
+        note: str = ""
+    ):
+        signature = self.encryption_api_key()
+        if signature == "fail":
+            return "Fetch Orders Api Key error"
+
+        url = f"{self.base_url}/fetch_orders"
+        headers = {
+            'Content-Type': 'application/json',
+        }
+        data = {
+            "symbol": symbol,
+            "start_datetime": start_datetime,
+            "end_datetime": end_datetime,
+            "page": page,
+            "ids": ids,
+            "status": status,
+            "sort_order": sort_order,
+            "order_type": order_type,
+            "side": side,
+            "limit": limit,
+            "account_vault": {
+                "third_identity_id": third_identity_id,
+                "api_key": self.api_key,
+                "signature": signature,
+                "note": note,
+            }
+        }
+        response = requests.post(url, data=json.dumps(data), headers=headers)
+        if response.status_code == 200:
+            res = response.json()
+            return res
+        else:
+            raise Exception(response.text)
```

### Comparing `zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/PKG-INFO` & `zerocap_api_new_test-0.1.9/zerocap_api_new_test.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,589 +1,590 @@
-Metadata-Version: 2.1
-Name: zerocap-api-new-test
-Version: 0.1.8
-Summary: zerocap_api
-Home-page: https://zerocap.com/
-Author: zerocap
-Author-email: jiayu.gao@eigen.capital
-License: MIT
-Platform: all
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
-# zerocap-api-new-test 
-
-# <a href="#testapi">Jump restapi</a>
-# <a href="#test">Jump websocket</a>
-
-
-
-```
-
-描述介绍
-
-sdk install
-pip install zerocap-api-new-test 
-。
-。
-。
-
-```
-
-
-
-# <a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi </a>
-#### <a href="https://dma-api.defi.wiki/redoc" target="_blank">接口文档</a> 
-
-```
-from zerocap_api_new_test import ZerocapRestClient
-import uuid
-import time
-
-# API key and secret required, 联系zerocap进行注册
-apiKey = "coinroutes" 
-apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
-```
-
-#### 1. Create an order
-<!--post https://dma-api.defi.wiki/orders/create_order-->
-
-```
-
-client = ZerocapRestClient(apiKey, apiSecret)
-client_order_id = str(uuid.uuid4())
-
-result = client.create_order(
-                    symbol='USDT/AUD', 
-                    side='buy', 
-                    type='market', 
-                    amount='100', 
-                    price='1000', 
-                    client_order_id=client_order_id, 
-                    note='this is test', 
-                    third_identity_id='ZCStreamingLiquidity1')
-
-```
-
-
-请求参数:
-
-| Parameter       | required  | data type | describe        | Value range  |
-|-----------------|-----------|-----------|-----------------|--------------|
-| symbol          | true      | string    | Instrument      | USDT/AUD     |
-| side            | true      | string    | Side            | buy sell     |
-| type            | true      | string    | Type            | market limit |
-| amount          | true      | string    | Quantity        |              |
-| price           | true      | string    | Price           |              |
-| client_order_id | true      | string    | Client order id |              |
-| note | true      | string    | note  |              |
-| third_identity_id | true      | string    | third_identity_id |              |
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-{
-    "symbol": "USDT/AUD",
-    "side": "buy",
-    "type": "market",
-    "amount": "1000",
-    "price": "1000",
-    "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
-    "account_vault": {
-        "third_identity_id": "918d7125916c13191f3674e",
-        "api_key": "***",
-        "signature": "***",
-        "note": ""
-    }
-}
-
-```
-
-响应数据:
-
-| Parameter          | required | data type | describe        | Value range |
-|--------------------|----------|-----------|-----------------|-------------|
-| id                 | true     | long      | Transaction ID  |             |
-| clientOrderId      | true     | string    | Client order id |             |
-| datatime           | true     | string    | Time            |             |
-| timestamp          | true     | string    | Time            |             |
-| lastTradeTimestamp | true     | long      | Time            |             |
-| status             | true     | string    | Status          |             |
-| type               | true     | string    | Type            |             |
-| timeInForce        | true     | string    | timeInForce     |             |
-| side               | true     | string    | Side            |             |
-| price              | true     | string    | Price           |             |
-| average            | true     | string    | average         |             |
-| amount             | true     | string    | Quantity        |             |
-| filled             | true     | string    | filled          |             |
-| remaining          | true     | string    | remaining       |             |
-| cost               | true     | string    | cost            |             |
-| transferId         | true     | string    | transferId      |             |
-| trades             | true     | string    | trades          |             |
-
-
-响应例子:
-
-```
-
- {
-    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
-    "clientOrderId": "e7f80d34-0d80-4256-9de3-cd37310a55dabe",
-    "datatime": "2023-07-28 09:19:45",
-    "timestamp": "1690535984000",
-    "lastTradeTimestamp": "1690535984000",
-    "status": "closed",
-    "symbol": "USDT/AUD",
-    "type": "Market",
-    "timeInForce": "FOK",
-    "side": "buy",
-    "price": "21.1",
-    "average": "1.685133171",
-    "amount": "9",
-    "filled": "9",
-    "remaining": "0",
-    "cost": "15.16619854",
-    "transferId": "12424971-f51d-4144-a205-9e306eb6351c",
-    "trades": [
-        {
-            "id": "12424971-f51d-4144-a205-9e306eb6351c",
-            "timestamp": "1690535984000",
-            "datetime": "2023-07-28 09:19:45",
-            "symbol": "USDT/AUD",
-            "order": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
-            "type": "market",
-            "side": "buy",
-            "takerOrMaker": "taker",
-            "price": "1.685133171",
-            "amount": "9",
-            "cost": "15.16619854",
-            "orderFrom": "coinroutes"
-        }
-    ]
-}
-
-```
-
-
-
-
-#### 2. Fetch specific orders
-<!--post https://dma-api.defi.wiki/orders/fetch_order-->
-```
-result = client.fetch_order(id='')
-```
-
-请求参数:
-
-
-| Parameter       | required | data type | describe       | Value range  |
-|-----------------|----------|-----------|----------------|--------------|
-| id              | true     | string    | Transaction ID |              |
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-{
-    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
-    "account_vault": {
-        "third_identity_id": "918d7125916c13191f3674e",
-        "api_key": "***",
-        "signature": "***",
-        "note": ""
-    }
-}
-
-```
-
-响应数据 接口报错 待定:
-
-
-| Parameter     | required | data type | describe       | Value range |
-|---------------|----------|-----------|----------------|-------------|
-| id            | true     | string    | Transaction ID |             |
-
-
-响应例子:
-
-```
-
-{
-	"order_list": [
-		{
-			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
-			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
-			"datatime": "2023-07-31 02:12:23",
-			"timestamp": "1690516007000",
-			"last_trade_timestamp": "1690516007000",
-			"status": "rejected",
-			"symbol": "USDT/AUD",
-			"type": "market",
-			"time_in_force": "FOK",
-			"side": "buy",
-			"price": "1000",
-			"average": "",
-			"amount": "1000",
-			"filled": "",
-			"remaining": "",
-			"cost": "",
-			"transfer_id": "",
-			"fee": "",
-			"trades": []
-		}
-	],
-	"status": "success",
-	"total": 3864,
-	"page": "1"
-}
-
-```
-
-
-#### 3. Batch fetch order
-<!--post https://dma-api.defi.wiki/orders/fetch_orders-->
-
-```
-result = client.fetch_orders(symbol='USDT/AUD', end_datetime=int(time.time() * 1000),
-                             start_datetime=int(time.time() * 1000 - 10*86400*1000),
-                             limit=10)
-```
-
-
-
-请求参数:
-
-| Parameter      | required | data type | describe        | Value range |
-|----------------|----------|-----------|-----------------|-------------|
-| symbol         | true     | string    | symbol          |             |
-| start_datetime | true     | string    | start_datetime  |             |
-| end_datetime   | true     | string    | end_datetime    |             |
-| page           | true     | string    | page            |             |
-| limit          | true     | string    | limit           |             |
-| ids            | true     | string    | Transaction ids(null character string or id1,id2...) |   |
-| status         | true     | string    | status          |             |
-| sort_order     | true     | string    | sort_order      |             |
-| order_type     | true     | string    | order_type      |             |
-| side           | true     | string    | side            |             |
-
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-{
-    "symbol": "",
-    "start_datetime": 0,
-    "end_datetime": 0,
-    "page": 0,
-    "limit": 0,
-    "ids": "",
-    "status": "",
-    "sort_order": "",
-    "order_type": "",
-    "side": "",
-    "account_vault": {
-        "third_identity_id": "918d7125916c13191f3674e",
-        "api_key": "***",
-        "signature": "***",
-        "note": ""
-    }
-}
-
-```
-
-响应数据 接口报错 待定:
-
-
-
-| Parameter     | required | data type | describe       | Value range |
-|---------------|----------|-----------|----------------|-------------|
-| id            | true     | string    | Transaction ID |             |
-| account_vault | true     | json      |  accountVault  |             |
-
-
-
-响应例子:
-
-```
-
-{
-	"order_list": [
-		{
-			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
-			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
-			"datatime": "2023-07-31 02:12:23",
-			"timestamp": "1690516007000",
-			"last_trade_timestamp": "1690516007000",
-			"status": "rejected",
-			"symbol": "USDT/AUD",
-			"type": "market",
-			"time_in_force": "FOK",
-			"side": "buy",
-			"price": "1000",
-			"average": "",
-			"amount": "1000",
-			"filled": "",
-			"remaining": "",
-			"cost": "",
-			"transfer_id": "",
-			"fee": "",
-			"trades": []
-		}
-	],
-	"status": "success",
-	"total": 3864,
-	"page": "1"
-}
-
-```
-
-
-
-## <span id='test'>websocket</span>
-
-```
-from zerocap_api_new_test import ZerocapWebsocketClient
-
-# API key and secret required, 联系zerocap进行注册
-apiKey = "***" 
-apiSecret = "***"
-
-signature = hmac.new(apiSecret.encode("utf-8"), apiKey.encode("utf-8"), hashlib.sha256).hexdigest()
-
-```
-
-#### 1. Subscribe to Market data
-
-<!--websocket wss://dma-api.defi.wiki/ws/GetMarket-->
-
-```
-market_connect = websocket.get_market()
-
-while True:
-    # Get  messages
-    message = websocket.get_message(market_connect)
-
-    print(f"Receiving message from server: \n{message}")
-
-```
-
-请求参数:
-
-| Parameter     | required | data type | describe                | Value range |
-|---------------|----------|-----------|-------------------------|-------------|
-| api_key       | true     | string    | key                     |             |
-| signature     | true     | long      | Cryptographic signature |             |
-| data_type     | true     | string    | Subscribed Channels     | price       |
-
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-wss://dma-api.defi.wiki/ws/GetMarket?api_key=***&signature=***&data_type=price
-
-```
-
-
-响应数据:
-
-
-| Parameter          | required | data type | describe      | Value range        |
-|--------------------|----------|-----------|---------------|--------------------|
-| type               | true     | long      | type          |                    |
-| channel            | true     | string    | channel       | dma_price_USDT/AUD |
-| data               | true     | jsonstr   | data          |                    |
-| data['sell_price'] | true     | string    | sell price    |                    |
-| data['buy_price']  | true     | string    | buy price     |                    |
-| data['datetime']   | true     | string    | time          |                    |
-| data['timestamp']  | true     | string    | time          |                    |
-| message            | false    | string    | description   | Is price open      |
-
-
-响应例子:
-
-```
-
-{
-    "type": "message",
-    "channel": "dma_price_USDT/AUD",
-    "data": "{
-        \"sell_price\": \"1.322544321902561296\",
-        \"buy_price\": \"1.668209315127094362\",
-        \"datetime\": \"2023-07-28 10:03:40\",
-        \"timestamp\": \"1690538620.1056492\"
-        }"
-}
-
-{
-    "type": "message",
-    "channel": "dma_price_USDT/AUD",
-    "data": "{
-        \"message\":\"Price stream unavailable.\"
-        }"
-}
-
-# Heartbeat neglect
-{"type":"message","channel":"","data":"{\"ok\": \"ok\"}"}
-
-```
-
-#### 2.  Subscribe Order updates or transaction records
-
-
-<!--websocket url:   wss://dma-api.defi.wiki/ws/GetOrdersInfo-->
-
-```
-orders_connect = websocket.get_orders()
-
-while True:
-    # Get  messages
-    message = websocket.get_message(orders_connect)
-
-    print(f"Receiving message from server: \n{message}")
-
-```
-
-
-请求参数:
-
-
-| Parameter     | required | data type | describe                | Value range |
-|---------------|----------|-----------|-------------------------|-------------|
-| api_key       | true     | string    | key                     |             |
-| signature     | true     | long      | Cryptographic signature |             |
-| data_type     | true     | string    | Subscribed Channels     | order,trade |
-
-
-请求参数：示例（不能直接使用,需要替换自己的参数）
-
-```
-
-wss://dma-api.defi.wiki/ws/GetOrdersInfo?api_key=***&signature=***&data_type=order,trade
-
-```
-
-
-channel: dma_order_info 响应数据:
-
-
-| Parameter             | required   | data type | describe      | Value range                    |
-|-----------------------|------------|-----------|---------------|--------------------------------|
-| type                  | true       | long      | type          |                                |
-| channel               | true       | string    | channel       | dma_order_info、dma_trader_info |
-| data                  | true       | jsonstr   | data          |                                |
-| data['OrderId']       | true       | str       | OrderId       |                                |
-| data['ClientOrderId'] | true       | str       | ClientOrderId |                                |
-| data['TxnAlias']      | true       | str       | TxnAlias      |                                |
-| data['TransferId']    | true       | str       | TransferId    |                                |
-| data['Symbol']        | true       | str       | Symbol        |                                |
-| data['Type']          | true       | str       | Type          |                                |
-| data['TimeInForce']   | true       | str       | TimeInForce   |                                |
-| data['Side']          | true       | str       | Side          |                                |
-| data['OrderId']       | true       | str       | OrderId       |                                |
-| data['Price']         | true       | str       | Price         |                                |
-| data['AveragePrice']  | true       | str       | AveragePrice  |                                |
-| data['Amount']        | true       | str       | Amount        |                                |
-| data['CreatedAt']     | true       | str       | CreatedAt     |                                |
-| data['UpdatedAt']     | true       | str       | UpdatedAt     |                                |
-| data['AccountId']     | true       | str       | AccountId     |                                |
-| data['VaultId']       | true       | str       | VaultId       |                                |
-| data['Note']          | true       | str       | Note          |                                |
-| data['Status']        | true       | str       | Status        |                                |
-| data['Average']       | true       | str       | Average       |                                |
-| data['Filled']        | true       | str       | Filled        |                                |
-| data['Remaining']     | true       | str       | Remaining     |                                |
-| data['Cost']          | true       | str       | Cost          |                                |
-| data['ExecPrice']     | true       | str       | ExecPrice     |                                |
-| data['OrderFrom']     | true       | str       | OrderFrom     |                                |
-
-
-响应例子:
-
-```
-
-{
-    "type":"message",
-    "channel":"dma_order_info",
-    "data":"{
-        \"OrderId\":\"d8be1f41-9e8e-4af0-899b-c1334916aa0e\",
-        \"ClientOrderId\":\"e7f80d34-0d80-4256-9de3-cd37310a55da\",
-        \"TxnAlias\":\"\",
-        \"TransferId\":\"\",
-        \"Symbol\":\"USDT/AUD\",
-        \"Type\":\"market\",
-        \"TimeInForce\":\"FOK\",
-        \"Side\":\"sell\",
-        \"Price\":\"1000\",
-        \"AveragePrice\":\"\",
-        \"Amount\":\"1000\",
-        \"CreatedAt\":1690538950000,
-        \"UpdatedAt\":1690538950000,
-        \"AccountId\":\"1ca36d2b-2103-45c7-a2e3-3b90825ba1b2\",
-        \"VaultId\":\"5175\",
-        \"Note\":\"yyy_test_create_order\",
-        \"Status\":\"open\",
-        \"Average\":\"0\",
-        \"Filled\":\"0\",
-        \"Remaining\":\"1000\",
-        \"Cost\":\"1000000\",
-        \"ExecPrice\":\"\",
-        \"OrderFrom\":\"coinroutes\"
-    }"
-}
-
-```
-
-channel: dma_trader_info 响应数据:
-
-
-| Parameter            | required   | data type | describe     | Value range                    |
-|----------------------|------------|-----------|--------------|--------------------------------|
-| type                 | true       | long      | type         |                                |
-| channel              | true       | string    | channel      | dma_order_info、dma_trader_info |
-| data                 | true       | jsonstr   | data         |                                |
-| data['id']           | true       | str       | id           |                                |
-| data['timestamp']    | true       | str       | timestamp    |                                |
-| data['datetime']     | true       | str       | datetime     |                                |
-| data['symbol']       | true       | str       | symbol       |                                |
-| data['order']        | true       | str       | order        |                                |
-| data['type']         | true       | str       | type         |                                |
-| data['side']         | true       | str       | side         |                                |
-| data['takerOrMaker'] | true       | str       | takerOrMaker |                                |
-| data['price']        | true       | str       | price        |                                |
-| data['amount']       | true       | str       | amount       |                                |
-| data['cost']         | true       | str       | cost         |                                |
-| data['orderFrom']    | true       | str       | orderFrom    |                                |
-
-
-响应例子:
-
-```
-
-{
-    "type":"message",
-    "pattern":null,
-    "channel":"dma_trade_info",
-    "data":"{
-        \"id\":\"60e2e941-070c-40e3-b2ef-4a8f6ad9f316\",
-        \"timestamp\":\"1690767892000\",
-        \"datetime\":\"2023-07-31 01:44:52\",
-        \"symbol\":\"USDT/AUD\",
-        \"order\":\"41969863-1f32-4eaa-b679-a5b0e6fb5542\",
-        \"type\":\"market\",
-        \"side\":\"sell\",
-        \"takerOrMaker\":\"taker\",
-        \"price\":\"1.662902412\",
-        \"amount\":\"101\",
-        \"cost\":\"167.9531436\",
-        \"orderFrom\":\"coinroutes\"
-    }"
-}
-
-```
+Metadata-Version: 2.1
+Name: zerocap-api-new-test
+Version: 0.1.9
+Summary: zerocap_api
+Home-page: https://zerocap.com/
+Author: zerocap
+Author-email: jiayu.gao@eigen.capital
+License: MIT
+Platform: all
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# zerocap-api-new-test 
+
+# <a href="#testapi">Jump restapi</a>
+# <a href="#test">Jump websocket</a>
+
+
+
+```
+
+描述介绍
+
+sdk install
+pip install zerocap-api-new-test 
+。
+。
+。
+
+```
+
+
+
+# <a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi </a>
+#### <a href="https://dma-api.defi.wiki/redoc" target="_blank">接口文档</a> 
+
+```
+from zerocap_api_new_test import ZerocapRestClient
+import uuid
+import time
+
+# API key and secret required, 联系zerocap进行注册
+apiKey = "coinroutes" 
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
+```
+
+#### 1. Create an order
+<!--post https://dma-uat-api.defi.wiki/v2/orders/create_order-->
+
+```
+
+client = ZerocapRestClient(apiKey, apiSecret)
+client_order_id = str(uuid.uuid4())
+
+result = client.create_order(
+                    symbol='USDT/AUD', 
+                    side='buy', 
+                    type='market', 
+                    amount='100', 
+                    price='1000', 
+                    client_order_id=client_order_id, 
+                    note='this is test', 
+                    third_identity_id='ZCStreamingLiquidity1')
+
+```
+
+
+请求参数:
+
+| Parameter       | required  | data type | describe        | Value range  |
+|-----------------|-----------|-----------|-----------------|--------------|
+| symbol          | true      | string    | Instrument      | USDT/AUD     |
+| side            | true      | string    | Side            | buy sell     |
+| type            | true      | string    | Type            | market limit |
+| amount          | true      | string    | Quantity        |              |
+| price           | true      | string    | Price           |              |
+| client_order_id | true      | string    | Client order id |              |
+| note | true      | string    | note  |              |
+| third_identity_id | true      | string    | third_identity_id |              |
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+{
+    "symbol": "USDT/AUD",
+    "side": "buy",
+    "type": "market",
+    "amount": "1000",
+    "price": "1000",
+    "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+    "account_vault": {
+        "third_identity_id": "918d7125916c13191f3674e",
+        "api_key": "***",
+        "signature": "***",
+        "note": ""
+    }
+}
+
+```
+
+响应数据:
+
+| Parameter          | required | data type | describe        | Value range |
+|--------------------|----------|-----------|-----------------|-------------|
+| id                 | true     | long      | Transaction ID  |             |
+| clientOrderId      | true     | string    | Client order id |             |
+| datatime           | true     | string    | Time            |             |
+| timestamp          | true     | string    | Time            |             |
+| lastTradeTimestamp | true     | long      | Time            |             |
+| status             | true     | string    | Status          |             |
+| type               | true     | string    | Type            |             |
+| timeInForce        | true     | string    | timeInForce     |             |
+| side               | true     | string    | Side            |             |
+| price              | true     | string    | Price           |             |
+| average            | true     | string    | average         |             |
+| amount             | true     | string    | Quantity        |             |
+| filled             | true     | string    | filled          |             |
+| remaining          | true     | string    | remaining       |             |
+| cost               | true     | string    | cost            |             |
+| transferId         | true     | string    | transferId      |             |
+| trades             | true     | string    | trades          |             |
+
+
+响应例子:
+
+```
+
+ {
+    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
+    "clientOrderId": "e7f80d34-0d80-4256-9de3-cd37310a55dabe",
+    "datatime": "2023-07-28 09:19:45",
+    "timestamp": "1690535984000",
+    "lastTradeTimestamp": "1690535984000",
+    "status": "closed",
+    "symbol": "USDT/AUD",
+    "type": "Market",
+    "timeInForce": "FOK",
+    "side": "buy",
+    "price": "21.1",
+    "average": "1.685133171",
+    "amount": "9",
+    "filled": "9",
+    "remaining": "0",
+    "cost": "15.16619854",
+    "transferId": "12424971-f51d-4144-a205-9e306eb6351c",
+    "trades": [
+        {
+            "id": "12424971-f51d-4144-a205-9e306eb6351c",
+            "timestamp": "1690535984000",
+            "datetime": "2023-07-28 09:19:45",
+            "symbol": "USDT/AUD",
+            "order": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
+            "type": "market",
+            "side": "buy",
+            "takerOrMaker": "taker",
+            "price": "1.685133171",
+            "amount": "9",
+            "cost": "15.16619854",
+            "orderFrom": "coinroutes"
+        }
+    ]
+}
+
+```
+
+
+
+
+#### 2. Fetch specific orders
+<!--post https://dma-uat-api.defi.wiki/v2/orders/fetch_order-->
+```
+result = client.fetch_order(id='')
+```
+
+请求参数:
+
+
+| Parameter       | required | data type | describe       | Value range  |
+|-----------------|----------|-----------|----------------|--------------|
+| id              | true     | string    | Transaction ID |              |
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+{
+    "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
+    "account_vault": {
+        "third_identity_id": "918d7125916c13191f3674e",
+        "api_key": "***",
+        "signature": "***",
+        "note": ""
+    }
+}
+
+```
+
+响应数据 接口报错 待定:
+
+
+| Parameter     | required | data type | describe       | Value range |
+|---------------|----------|-----------|----------------|-------------|
+| id            | true     | string    | Transaction ID |             |
+
+
+响应例子:
+
+```
+
+{
+	"order_list": [
+		{
+			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
+			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+			"datatime": "2023-07-31 02:12:23",
+			"timestamp": "1690516007000",
+			"last_trade_timestamp": "1690516007000",
+			"status": "rejected",
+			"symbol": "USDT/AUD",
+			"type": "market",
+			"time_in_force": "FOK",
+			"side": "buy",
+			"price": "1000",
+			"average": "",
+			"amount": "1000",
+			"filled": "",
+			"remaining": "",
+			"cost": "",
+			"transfer_id": "",
+			"fee": "",
+			"trades": []
+		}
+	],
+	"status": "success",
+	"total": 3864,
+	"page": "1"
+}
+
+```
+
+
+#### 3. Batch fetch order
+<!--post https://dma-uat-api.defi.wiki/v2/orders/fetch_orders-->
+
+```
+result = client.fetch_orders(symbol='USDT/AUD', end_datetime=int(time.time() * 1000),
+                             start_datetime=int(time.time() * 1000 - 10*86400*1000),
+                             limit=10)
+```
+
+
+
+请求参数:
+
+| Parameter      | required | data type | describe        | Value range |
+|----------------|----------|-----------|-----------------|-------------|
+| symbol         | true     | string    | symbol          |             |
+| start_datetime | true     | string    | start_datetime  |             |
+| end_datetime   | true     | string    | end_datetime    |             |
+| page           | true     | string    | page            |             |
+| limit          | true     | string    | limit           |             |
+| ids            | true     | string    | Transaction ids(null character string or id1,id2...) |   |
+| status         | true     | string    | status          |             |
+| sort_order     | true     | string    | sort_order      |             |
+| order_type     | true     | string    | order_type      |             |
+| side           | true     | string    | side            |             |
+
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+{
+    "symbol": "",
+    "start_datetime": 0,
+    "end_datetime": 0,
+    "page": 0,
+    "limit": 0,
+    "ids": "",
+    "status": "",
+    "sort_order": "",
+    "order_type": "",
+    "side": "",
+    "account_vault": {
+        "third_identity_id": "918d7125916c13191f3674e",
+        "api_key": "***",
+        "signature": "***",
+        "note": ""
+    }
+}
+
+```
+
+响应数据 接口报错 待定:
+
+
+
+| Parameter     | required | data type | describe       | Value range |
+|---------------|----------|-----------|----------------|-------------|
+| id            | true     | string    | Transaction ID |             |
+| account_vault | true     | json      |  accountVault  |             |
+
+
+
+响应例子:
+
+```
+
+{
+	"order_list": [
+		{
+			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
+			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+			"datatime": "2023-07-31 02:12:23",
+			"timestamp": "1690516007000",
+			"last_trade_timestamp": "1690516007000",
+			"status": "rejected",
+			"symbol": "USDT/AUD",
+			"type": "market",
+			"time_in_force": "FOK",
+			"side": "buy",
+			"price": "1000",
+			"average": "",
+			"amount": "1000",
+			"filled": "",
+			"remaining": "",
+			"cost": "",
+			"transfer_id": "",
+			"fee": "",
+			"trades": []
+		}
+	],
+	"status": "success",
+	"total": 3864,
+	"page": "1"
+}
+
+```
+
+
+
+## <span id='test'>websocket</span>
+
+```
+from zerocap_api_new_test import ZerocapWebsocketClient
+
+# API key and secret required, 联系zerocap进行注册
+apiKey = "***" 
+apiSecret = "***"
+
+signature = hmac.new(apiSecret.encode("utf-8"), apiKey.encode("utf-8"), hashlib.sha256).hexdigest()
+
+```
+
+#### 1. Subscribe to Market data
+
+<!--websocket wss://dma-uat-ws.defi.wiki/v2/ws/GetMarket-->
+
+```
+market_connect = websocket.get_market()
+
+while True:
+    # Get  messages
+    message = websocket.get_message(market_connect)
+
+    print(f"Receiving message from server: \n{message}")
+
+```
+
+请求参数:
+
+| Parameter     | required | data type | describe                | Value range |
+|---------------|----------|-----------|-------------------------|-------------|
+| api_key       | true     | string    | key                     |             |
+| signature     | true     | long      | Cryptographic signature |             |
+| data_type     | true     | string    | Subscribed Channels     | price       |
+
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+wss://dma-uat-ws.defi.wiki/v2/ws/GetMarket?api_key=***&signature=***&data_type=price
+
+```
+
+
+响应数据:
+
+
+| Parameter          | required | data type | describe      | Value range        |
+|--------------------|----------|-----------|---------------|--------------------|
+| type               | true     | long      | type          |                    |
+| channel            | true     | string    | channel       | dma_price_USDT/AUD |
+| data               | true     | jsonstr   | data          |                    |
+| data['sell_price'] | true     | string    | sell price    |                    |
+| data['buy_price']  | true     | string    | buy price     |                    |
+| data['datetime']   | true     | string    | time          |                    |
+| data['timestamp']  | true     | string    | time          |                    |
+| message            | false    | string    | description   | Is price open      |
+
+
+响应例子:
+
+```
+
+{
+    "type": "message",
+    "channel": "dma_price_USDT/AUD",
+    "data": "{
+        \"sell_price\": \"1.322544321902561296\",
+        \"buy_price\": \"1.668209315127094362\",
+        \"datetime\": \"2023-07-28 10:03:40\",
+        \"timestamp\": \"1690538620.1056492\"
+        }"
+}
+
+{
+    "type": "message",
+    "channel": "dma_price_USDT/AUD",
+    "data": "{
+        \"message\":\"Price stream unavailable.\"
+        }"
+}
+
+# Heartbeat neglect
+{"type":"message","channel":"","data":"{\"ok\": \"ok\"}"}
+
+```
+
+#### 2.  Subscribe Order updates or transaction records
+
+
+<!--websocket url:   wss://dma-uat-ws.defi.wiki/v2/ws/GetOrdersInfo-->
+
+```
+orders_connect = websocket.get_orders()
+
+while True:
+    # Get  messages
+    message = websocket.get_message(orders_connect)
+
+    print(f"Receiving message from server: \n{message}")
+
+```
+
+
+请求参数:
+
+
+| Parameter     | required | data type | describe                | Value range |
+|---------------|----------|-----------|-------------------------|-------------|
+| api_key       | true     | string    | key                     |             |
+| signature     | true     | long      | Cryptographic signature |             |
+| data_type     | true     | string    | Subscribed Channels     | order,trade |
+
+
+请求参数：示例（不能直接使用,需要替换自己的参数）
+
+```
+
+wss://dma-uat-ws.defi.wiki/v2/ws/GetOrdersInfo?api_key=***&signature=***&data_type=order,trade
+
+```
+
+
+channel: dma_order_info 响应数据:
+
+
+| Parameter             | required   | data type | describe      | Value range                    |
+|-----------------------|------------|-----------|---------------|--------------------------------|
+| type                  | true       | long      | type          |                                |
+| channel               | true       | string    | channel       | dma_order_info、dma_trader_info |
+| data                  | true       | jsonstr   | data          |                                |
+| data['OrderId']       | true       | str       | OrderId       |                                |
+| data['ClientOrderId'] | true       | str       | ClientOrderId |                                |
+| data['TxnAlias']      | true       | str       | TxnAlias      |                                |
+| data['TransferId']    | true       | str       | TransferId    |                                |
+| data['Symbol']        | true       | str       | Symbol        |                                |
+| data['Type']          | true       | str       | Type          |                                |
+| data['TimeInForce']   | true       | str       | TimeInForce   |                                |
+| data['Side']          | true       | str       | Side          |                                |
+| data['OrderId']       | true       | str       | OrderId       |                                |
+| data['Price']         | true       | str       | Price         |                                |
+| data['AveragePrice']  | true       | str       | AveragePrice  |                                |
+| data['Amount']        | true       | str       | Amount        |                                |
+| data['CreatedAt']     | true       | str       | CreatedAt     |                                |
+| data['UpdatedAt']     | true       | str       | UpdatedAt     |                                |
+| data['AccountId']     | true       | str       | AccountId     |                                |
+| data['VaultId']       | true       | str       | VaultId       |                                |
+| data['Note']          | true       | str       | Note          |                                |
+| data['Status']        | true       | str       | Status        |                                |
+| data['Average']       | true       | str       | Average       |                                |
+| data['Filled']        | true       | str       | Filled        |                                |
+| data['Remaining']     | true       | str       | Remaining     |                                |
+| data['Cost']          | true       | str       | Cost          |                                |
+| data['ExecPrice']     | true       | str       | ExecPrice     |                                |
+| data['OrderFrom']     | true       | str       | OrderFrom     |                                |
+
+
+响应例子:
+
+```
+
+{
+    "type":"message",
+    "channel":"dma_order_info",
+    "data":"{
+        \"OrderId\":\"d8be1f41-9e8e-4af0-899b-c1334916aa0e\",
+        \"ClientOrderId\":\"e7f80d34-0d80-4256-9de3-cd37310a55da\",
+        \"TxnAlias\":\"\",
+        \"TransferId\":\"\",
+        \"Symbol\":\"USDT/AUD\",
+        \"Type\":\"market\",
+        \"TimeInForce\":\"FOK\",
+        \"Side\":\"sell\",
+        \"Price\":\"1000\",
+        \"AveragePrice\":\"\",
+        \"Amount\":\"1000\",
+        \"CreatedAt\":1690538950000,
+        \"UpdatedAt\":1690538950000,
+        \"AccountId\":\"1ca36d2b-2103-45c7-a2e3-3b90825ba1b2\",
+        \"VaultId\":\"5175\",
+        \"Note\":\"yyy_test_create_order\",
+        \"Status\":\"open\",
+        \"Average\":\"0\",
+        \"Filled\":\"0\",
+        \"Remaining\":\"1000\",
+        \"Cost\":\"1000000\",
+        \"ExecPrice\":\"\",
+        \"OrderFrom\":\"coinroutes\"
+    }"
+}
+
+```
+
+channel: dma_trader_info 响应数据:
+
+
+| Parameter            | required   | data type | describe     | Value range                    |
+|----------------------|------------|-----------|--------------|--------------------------------|
+| type                 | true       | long      | type         |                                |
+| channel              | true       | string    | channel      | dma_order_info、dma_trader_info |
+| data                 | true       | jsonstr   | data         |                                |
+| data['id']           | true       | str       | id           |                                |
+| data['timestamp']    | true       | str       | timestamp    |                                |
+| data['datetime']     | true       | str       | datetime     |                                |
+| data['symbol']       | true       | str       | symbol       |                                |
+| data['order']        | true       | str       | order        |                                |
+| data['type']         | true       | str       | type         |                                |
+| data['side']         | true       | str       | side         |                                |
+| data['takerOrMaker'] | true       | str       | takerOrMaker |                                |
+| data['price']        | true       | str       | price        |                                |
+| data['amount']       | true       | str       | amount       |                                |
+| data['cost']         | true       | str       | cost         |                                |
+| data['orderFrom']    | true       | str       | orderFrom    |                                |
+
+
+响应例子:
+
+```
+
+{
+    "type":"message",
+    "pattern":null,
+    "channel":"dma_trade_info",
+    "data":"{
+        \"id\":\"60e2e941-070c-40e3-b2ef-4a8f6ad9f316\",
+        \"timestamp\":\"1690767892000\",
+        \"datetime\":\"2023-07-31 01:44:52\",
+        \"symbol\":\"USDT/AUD\",
+        \"order\":\"41969863-1f32-4eaa-b679-a5b0e6fb5542\",
+        \"type\":\"market\",
+        \"side\":\"sell\",
+        \"takerOrMaker\":\"taker\",
+        \"price\":\"1.662902412\",
+        \"amount\":\"101\",
+        \"cost\":\"167.9531436\",
+        \"orderFrom\":\"coinroutes\"
+    }"
+}
+
+```
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.9 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
@@ -98,22 +98,23 @@
 messages message = websocket.get_message(market_connect) print(f"Receiving
 message from server: \n{message}") ``` è¯·æ±åæ°: | Parameter | required |
 data type | describe | Value range | |---------------|----------|-----------|--
 -----------------------|-------------| | api_key | true | string | key | | |
 signature | true | long | Cryptographic signature | | | data_type | true |
 string | Subscribed Channels | price |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
-wss://dma-api.defi.wiki/ws/GetMarket?api_key=***&signature=***&data_type=price
-``` ååºæ°æ®: | Parameter | required | data type | describe | Value range |
-|--------------------|----------|-----------|---------------|------------------
---| | type | true | long | type | | | channel | true | string | channel |
-dma_price_USDT/AUD | | data | true | jsonstr | data | | | data['sell_price'] |
-true | string | sell price | | | data['buy_price'] | true | string | buy price
-| | | data['datetime'] | true | string | time | | | data['timestamp'] | true |
-string | time | | | message | false | string | description | Is price open |
+wss://dma-uat-ws.defi.wiki/v2/ws/
+GetMarket?api_key=***&signature=***&data_type=price ``` ååºæ°æ®: |
+Parameter | required | data type | describe | Value range | |------------------
+--|----------|-----------|---------------|--------------------| | type | true |
+long | type | | | channel | true | string | channel | dma_price_USDT/AUD | |
+data | true | jsonstr | data | | | data['sell_price'] | true | string | sell
+price | | | data['buy_price'] | true | string | buy price | | | data
+['datetime'] | true | string | time | | | data['timestamp'] | true | string |
+time | | | message | false | string | description | Is price open |
 ååºä¾å­: ``` { "type": "message", "channel": "dma_price_USDT/AUD", "data":
 "{ \"sell_price\": \"1.322544321902561296\", \"buy_price\":
 \"1.668209315127094362\", \"datetime\": \"2023-07-28 10:03:40\", \"timestamp\":
 \"1690538620.1056492\" }" } { "type": "message", "channel": "dma_price_USDT/
 AUD", "data": "{ \"message\":\"Price stream unavailable.\" }" } # Heartbeat
 neglect {"type":"message","channel":"","data":"{\"ok\": \"ok\"}"} ``` #### 2.
 Subscribe Order updates or transaction records  ``` orders_connect =
@@ -121,15 +122,15 @@
 websocket.get_message(orders_connect) print(f"Receiving message from server: \n
 {message}") ``` è¯·æ±åæ°: | Parameter | required | data type | describe |
 Value range | |---------------|----------|-----------|-------------------------
 |-------------| | api_key | true | string | key | | | signature | true | long |
 Cryptographic signature | | | data_type | true | string | Subscribed Channels |
 order,trade |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
-wss://dma-api.defi.wiki/ws/
+wss://dma-uat-ws.defi.wiki/v2/ws/
 GetOrdersInfo?api_key=***&signature=***&data_type=order,trade ``` channel:
 dma_order_info ååºæ°æ®: | Parameter | required | data type | describe |
 Value range | |-----------------------|------------|-----------|---------------
 |--------------------------------| | type | true | long | type | | | channel |
 true | string | channel | dma_order_infoãdma_trader_info | | data | true |
 jsonstr | data | | | data['OrderId'] | true | str | OrderId | | | data
 ['ClientOrderId'] | true | str | ClientOrderId | | | data['TxnAlias'] | true |
```

