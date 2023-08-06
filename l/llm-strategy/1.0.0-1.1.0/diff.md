# Comparing `tmp/llm_strategy-1.0.0.tar.gz` & `tmp/llm_strategy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_strategy-1.0.0.tar", max compression
+gzip compressed data, was "llm_strategy-1.1.0.tar", max compression
```

## Comparing `llm_strategy-1.0.0.tar` & `llm_strategy-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1090 2023-08-02 22:30:44.700720 llm_strategy-1.0.0/LICENSE
--rw-r--r--   0        0        0     5216 2023-08-02 22:30:44.700720 llm_strategy-1.0.0/README.md
--rw-r--r--   0        0        0      185 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/__init__.py
--rw-r--r--   0        0        0     2220 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/adapters.py
--rw-r--r--   0        0        0     2120 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/chat_chain.py
--rw-r--r--   0        0        0    36554 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/llm_function.py
--rw-r--r--   0        0        0     4562 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/llm_strategy.py
--rw-r--r--   0        0        0        0 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/__init__.py
--rw-r--r--   0        0        0     5974 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/fake_chat_model.py
--rw-r--r--   0        0        0     3217 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/fake_llm.py
--rw-r--r--   0        0        0     1999 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/tests/test_fake_chat_model.py
--rw-r--r--   0        0        0      685 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/testing/tests/test_fake_llm.py
--rw-r--r--   0        0        0      776 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/tests/test_adapters.py
--rw-r--r--   0        0        0    15025 2023-08-02 22:30:44.704720 llm_strategy-1.0.0/llm_strategy/tests/test_llm_function.py
--rw-r--r--   0        0        0    23624 2023-08-02 22:30:44.708720 llm_strategy-1.0.0/llm_strategy/tests/test_llm_strategy.py
--rw-r--r--   0        0        0     1847 2023-08-02 22:31:14.316805 llm_strategy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5941 1970-01-01 00:00:00.000000 llm_strategy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-08-06 23:12:14.100914 llm_strategy-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5216 2023-08-06 23:12:14.100914 llm_strategy-1.1.0/README.md
+-rw-r--r--   0        0        0      695 2023-08-06 23:25:55.489254 llm_strategy-1.1.0/llm_strategy/__init__.py
+-rw-r--r--   0        0        0     2730 2023-08-06 23:25:55.465253 llm_strategy-1.1.0/llm_strategy/adapters.py
+-rw-r--r--   0        0        0     2630 2023-08-06 23:25:55.493254 llm_strategy-1.1.0/llm_strategy/chat_chain.py
+-rw-r--r--   0        0        0    37064 2023-08-06 23:25:55.469253 llm_strategy-1.1.0/llm_strategy/llm_function.py
+-rw-r--r--   0        0        0     5072 2023-08-06 23:25:55.485254 llm_strategy-1.1.0/llm_strategy/llm_strategy.py
+-rw-r--r--   0        0        0     1999 2023-08-06 23:25:55.481253 llm_strategy-1.1.0/llm_strategy/structured_query.py
+-rw-r--r--   0        0        0      509 2023-08-06 23:25:55.737264 llm_strategy-1.1.0/llm_strategy/testing/__init__.py
+-rw-r--r--   0        0        0     6381 2023-08-06 23:25:55.481253 llm_strategy-1.1.0/llm_strategy/testing/fake_chat_model.py
+-rw-r--r--   0        0        0     3727 2023-08-06 23:25:55.485254 llm_strategy-1.1.0/llm_strategy/testing/fake_llm.py
+-rw-r--r--   0        0        0     2406 2023-08-06 23:25:55.473253 llm_strategy-1.1.0/llm_strategy/testing/tests/test_fake_chat_model.py
+-rw-r--r--   0        0        0     1195 2023-08-06 23:25:55.465253 llm_strategy-1.1.0/llm_strategy/testing/tests/test_fake_llm.py
+-rw-r--r--   0        0        0     1286 2023-08-06 23:25:55.461253 llm_strategy-1.1.0/llm_strategy/tests/test_adapters.py
+-rw-r--r--   0        0        0    15535 2023-08-06 23:25:55.477253 llm_strategy-1.1.0/llm_strategy/tests/test_llm_function.py
+-rw-r--r--   0        0        0    24134 2023-08-06 23:25:55.469253 llm_strategy-1.1.0/llm_strategy/tests/test_llm_strategy.py
+-rw-r--r--   0        0        0     3948 2023-08-06 23:25:55.457252 llm_strategy-1.1.0/llm_strategy/tests/test_structured_query.py
+-rw-r--r--   0        0        0     1847 2023-08-06 23:27:39.677656 llm_strategy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5941 1970-01-01 00:00:00.000000 llm_strategy-1.1.0/PKG-INFO
```

### Comparing `llm_strategy-1.0.0/LICENSE` & `llm_strategy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_strategy-1.0.0/README.md` & `llm_strategy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `llm_strategy-1.0.0/llm_strategy/adapters.py` & `llm_strategy-1.1.0/llm_strategy/adapters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+#  Copyright (c) 2023, Andreas Kirsch, Daedalus Lab Ltd
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
+
 from typing import List, Optional
 
 from langchain.chat_models.base import BaseChatModel
 from langchain.llms import BaseLLM
 from langchain.schema import AIMessage, BaseMessage, ChatMessage, ChatResult, LLMResult
```

### Comparing `llm_strategy-1.0.0/llm_strategy/chat_chain.py` & `llm_strategy-1.1.0/llm_strategy/chat_chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+#  Copyright (c) 2023, Andreas Kirsch, Daedalus Lab Ltd
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
+
 import dataclasses
 import typing
 from dataclasses import dataclass
 from typing import Tuple
 
 from langchain.chat_models.base import BaseChatModel
 from langchain.output_parsers import PydanticOutputParser
```

### Comparing `llm_strategy-1.0.0/llm_strategy/llm_function.py` & `llm_strategy-1.1.0/llm_strategy/llm_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+#  Copyright (c) 2023, Andreas Kirsch, Daedalus Lab Ltd
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
+
 # type: ignore
 import dis
 import functools
 import inspect
 import json
 import re
 import string
```

### Comparing `llm_strategy-1.0.0/llm_strategy/llm_strategy.py` & `llm_strategy-1.1.0/llm_strategy/llm_strategy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+#  Copyright (c) 2023, Andreas Kirsch, Daedalus Lab Ltd
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
+
 # type: ignore
 import dataclasses
 import functools  # noqa: F401
 import inspect
 import typing
 from dataclasses import dataclass
```

### Comparing `llm_strategy-1.0.0/llm_strategy/testing/fake_chat_model.py` & `llm_strategy-1.1.0/llm_strategy/testing/fake_chat_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,15 @@
-#  Blackboard-PAGI - LLM Proto-AGI using the Blackboard Pattern
-#  Copyright (c) 2023. Andreas Kirsch
+#  Copyright (c) 2023, Andreas Kirsch, Daedalus Lab Ltd
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Affero General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
```

### Comparing `llm_strategy-1.0.0/llm_strategy/testing/fake_llm.py` & `llm_strategy-1.1.0/llm_strategy/testing/fake_llm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+#  Copyright (c) 2023, Andreas Kirsch, Daedalus Lab Ltd
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
+
 from typing import Any, Mapping
 
 from langchain.llms.base import LLM, BaseLLM
 from pydantic import BaseModel, Field
 
 
 class FakeLLM(LLM, BaseModel):
```

### Comparing `llm_strategy-1.0.0/llm_strategy/testing/tests/test_fake_chat_model.py` & `llm_strategy-1.1.0/llm_strategy/testing/tests/test_fake_chat_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,15 @@
-#  Blackboard-PAGI - LLM Proto-AGI using the Blackboard Pattern
-#  Copyright (c) 2023. Andreas Kirsch
+#  Copyright (c) 2023, Andreas Kirsch, Daedalus Lab Ltd
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Affero General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
```

### Comparing `llm_strategy-1.0.0/llm_strategy/tests/test_llm_function.py` & `llm_strategy-1.1.0/llm_strategy/tests/test_llm_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+#  Copyright (c) 2023, Andreas Kirsch, Daedalus Lab Ltd
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
+
 # type: ignore
 import inspect
 import re
 import typing
 
 import pytest
 from langchain.chat_models.base import BaseChatModel
```

### Comparing `llm_strategy-1.0.0/llm_strategy/tests/test_llm_strategy.py` & `llm_strategy-1.1.0/llm_strategy/tests/test_llm_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+#  Copyright (c) 2023, Andreas Kirsch, Daedalus Lab Ltd
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
+
 from dataclasses import dataclass
 
 from llm_strategy import llm_strategy
 from llm_strategy.llm_function import is_not_implemented
 from llm_strategy.testing.fake_llm import FakeLLM
```

### Comparing `llm_strategy-1.0.0/pyproject.toml` & `llm_strategy-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm_strategy"
-version = "1.0.0"
+version = "1.1.0"
 description = "Directly Connecting Python to LLMs - Dataclasses & Interfaces <-> LLMs"
 authors = ["Andreas Kirsch, Daedalus Lab Ltd <blackhc@gmail.com>"]
 repository = "https://github.com/blackhc/llm-strategy"
 documentation = "https://blackhc.github.io/llm-strategy/"
 readme = "README.md"
 packages = [
   {include = "llm_strategy"}
```

### Comparing `llm_strategy-1.0.0/PKG-INFO` & `llm_strategy-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-strategy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Directly Connecting Python to LLMs - Dataclasses & Interfaces <-> LLMs
 Home-page: https://github.com/blackhc/llm-strategy
 Author: Andreas Kirsch, Daedalus Lab Ltd
 Author-email: blackhc@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

