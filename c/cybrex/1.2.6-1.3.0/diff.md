# Comparing `tmp/cybrex-1.2.6.tar.gz` & `tmp/cybrex-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.2.6.tar", last modified: Fri Aug  4 09:11:32 2023, max compression
+gzip compressed data, was "cybrex-1.3.0.tar", last modified: Mon Aug  7 13:44:11 2023, max compression
```

## Comparing `cybrex-1.2.6.tar` & `cybrex-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 09:11:32.530575 cybrex-1.2.6/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.2.6/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-04 09:11:32.529975 cybrex-1.2.6/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.2.6/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 09:11:32.525836 cybrex-1.2.6/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.2.6/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5649 2023-08-04 07:30:23.000000 cybrex-1.2.6/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    13562 2023-08-04 08:15:13.000000 cybrex-1.2.6/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13933 2023-08-04 09:11:04.000000 cybrex-1.2.6/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 09:11:32.529130 cybrex-1.2.6/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-04 09:11:12.000000 cybrex-1.2.6/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.2.6/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-04 09:11:32.530800 cybrex-1.2.6/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.015717 cybrex-1.3.0/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.3.0/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 13:44:11.015448 cybrex-1.3.0/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.3.0/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.011270 cybrex-1.3.0/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.3.0/cybrex/__init__.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.013787 cybrex-1.3.0/cybrex/chains/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.0/cybrex/chains/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.3.0/cybrex/chains/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2381 2023-08-07 13:01:11.000000 cybrex-1.3.0/cybrex/chains/map_reduce.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5550 2023-08-07 10:16:43.000000 cybrex-1.3.0/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    10794 2023-08-07 13:42:48.000000 cybrex-1.3.0/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1676 2023-08-05 19:44:06.000000 cybrex-1.3.0/cybrex/document_chunker.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4830 2023-08-07 11:07:40.000000 cybrex-1.3.0/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.014262 cybrex-1.3.0/cybrex/prompts/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.0/cybrex/prompts/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     9756 2023-08-07 13:43:38.000000 cybrex-1.3.0/cybrex/prompts/base.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.015014 cybrex-1.3.0/cybrex/vector_storage/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.0/cybrex/vector_storage/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      206 2023-08-07 13:42:48.000000 cybrex-1.3.0/cybrex/vector_storage/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2987 2023-08-07 12:50:10.000000 cybrex-1.3.0/cybrex/vector_storage/chroma.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.013079 cybrex-1.3.0/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 13:44:10.000000 cybrex-1.3.0/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      554 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-07 13:43:56.000000 cybrex-1.3.0/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.3.0/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-07 13:44:11.015817 cybrex-1.3.0/setup.cfg
```

### Comparing `cybrex-1.2.6/PKG-INFO` & `cybrex-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.2.6
+Version: 1.3.0
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.2.6/README.md` & `cybrex-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.2.6/cybrex/cli.py` & `cybrex-1.3.0/cybrex/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,75 +20,75 @@
 
     async def add_all_documents(self):
         async with self.cybrex as cybrex:
             async for document in cybrex.geck.get_summa_client().documents('nexus_science'):
                 document = json.loads(document)
                 await self.cybrex.add_full_documents([document])
 
-    async def dump_texts(self, query: str, output_path: str, n_summa_documents: int = 100):
+    async def dump_texts(self, query: str, output_path: str, n_documents: int = 100):
         """
         Store STC text chunks in ZIP archive
 
         :param query: query to STC
         :param output_path: where to store result
-        :param n_summa_documents: the number of documents to extract
+        :param n_documents: the number of chunks to extract
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Q', 'green')}: {query}")
-            await cybrex.dump_texts(
+            await cybrex.export_texts(
                 query=query,
                 output_path=output_path,
-                n_summa_documents=n_summa_documents
+                n_documents=n_documents
             )
 
     async def import_texts(self, input_path: str):
         """
         Import binary file with embeddings
 
         :param input_path:
         """
         await self.cybrex.import_texts(input_path=input_path)
 
-    async def chat_doc(self, field: str, value: str, question: str, n_results: int = 4):
+    async def chat_doc(self, field: str, value: str, question: str, n_chunks: int = 4):
         """
         Ask a question about content of document identified by DOI.
 
         :param field: name of the field in document used for selection
         :param value: value of the field in document used for selection
         :param question: Text question to the document
-        :param n_results: the number of documents to extract from Chroma
+        :param n_chunks: the number of chunks to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Document', 'green')}: {field}:{value}")
             print(f"{colored('Q', 'green')}: {question}")
-            response = await cybrex.chat_document(field, value, question, n_results)
+            response = await cybrex.chat_document(field, value, question, n_chunks)
             print(f"{colored('A', 'green')}: {response}")
 
     async def chat_sci(
         self,
         query: str,
-        n_results: int = 4,
-        n_summa_documents: int = 10,
+        n_chunks: int = 4,
+        n_documents: int = 10,
     ):
         """
         Ask a question about content of document identified by DOI.
 
         :param query: Text question to the document
-        :param n_results: the number of documents to extract from Chroma
+        :param n_chunks: the number of chunks to extract from Chroma
             more means more tokens to use and more precision in answer
-        :param n_summa_documents: the number of documents to extract from Chroma
+        :param n_documents: the number of chunks to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Q', 'green')}: {query}")
             answer, documents, summa_documents = await cybrex.chat_science(
                 query=query,
-                n_results=n_results,
-                n_summa_documents=n_summa_documents,
+                n_chunks=n_chunks,
+                n_documents=n_documents,
             )
             answer = re.sub(r'\(DOI: ([^)]+)\)', r'(https://doi.org/\g<1>)', answer)
             summa_documents = [f'{summa_document["doi"]}: {summa_document["title"]}' for summa_document in summa_documents]
             sources = '\n'.join(summa_documents)
             print(f"{colored('A', 'green')}: {answer}")
             print(f"{colored('References', 'green')}:\n{textwrap.indent(sources, ' - ')}")
 
@@ -100,29 +100,29 @@
         :param value: value of the field in document used for selection
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Document', 'green')}: {field}:{value}")
             response = await cybrex.summarize_document(field, value)
             print(f"{colored('Summarization', 'green')}: {response}")
 
-    async def semantic_search(self, query: str, n_results: int = 10, n_summa_documents: int = 30):
+    async def semantic_search(self, query: str, n_chunks: int = 10, n_documents: int = 30):
         """
         Ask a question about content of document identified by DOI.
 
         :param query: query to STC
-        :param n_results: number of pieces to return
-        :param n_summa_documents: the number of documents to extract from Chroma
+        :param n_chunks: number of pieces to return
+        :param n_documents: the number of chunks to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Q', 'green')}: {query}")
             documents = await cybrex.semantic_search(
                 query=query,
-                n_results=n_results,
-                n_summa_documents=n_summa_documents
+                n_chunks=n_chunks,
+                n_documents=n_documents
             )
             snippets = [
                 ' - ' + create_snippet(document)
                 for document in documents
             ]
             sources = '\n'.join(snippets)
             print(f"{colored('Sources', 'green')}:\n{sources}")
@@ -132,15 +132,15 @@
     """
     :param debug: add debugging output
     :return:
     """
     logging.basicConfig(stream=sys.stdout, level=logging.INFO if debug else logging.ERROR)
     cybrex_ai = CybrexCli()
     return {
-        'add-all-documents': cybrex_ai.add_all_documents,
+        'add-all-chunks': cybrex_ai.add_all_documents,
         'chat-doc': cybrex_ai.chat_doc,
         'chat-sci': cybrex_ai.chat_sci,
         'dump-texts': cybrex_ai.dump_texts,
         'import-texts': cybrex_ai.import_texts,
         'semantic-search': cybrex_ai.semantic_search,
         'sum-doc': cybrex_ai.sum_doc,
     }
```

### Comparing `cybrex-1.2.6/cybrex/models.py` & `cybrex-1.3.0/cybrex/prompts/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,112 @@
-import logging
 from collections import OrderedDict
 from typing import List
 
-from ctransformers import AutoModelForCausalLM
-from keybert import KeyBERT
-from langchain import OpenAI
-from langchain.embeddings import HuggingFaceInstructEmbeddings, OpenAIEmbeddings
-from langchain.text_splitter import RecursiveCharacterTextSplitter
-from lazy import lazy
-
 
 class BasePrompter:
     @staticmethod
     def prompter_from_type(type_):
         return {
             'default': BasePrompter(),
             'llama2-7b': Llama27bPrompter(),
             'openai': OpenAIPrompter()
         }[type_]
 
-    def qa_prompt(self, question, documents: List[dict]):
-        if len(documents) >= 1:
+    def qa_prompt(self, question, chunks: List[dict]):
+        if len(chunks) >= 1:
             return '''
-USER: You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
-ALWAYS add references to extracted parts using template "DOI: 10.1038/s41576-022-00477-6" near corresponding statements. 
+You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
+ALWAYS add references using DOIs near corresponding statements in your answer.
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
+
+USER:
 Extracted parts:
 {summary}
 
 Question:
 {question}
-ASSISTANT:'''.format(question=question, summary=self.generate_summary(documents))
+ASSISTANT:'''.format(question=question, summary=self.generate_summary(chunks))
         else:
             return '''
-USER: You are Cybrex AI created by People of Nexus. Answer the question.
+You are Cybrex AI created by People of Nexus. Answer the question.
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 
+USER:
 Question:
 {question}
 ASSISTANT:'''.format(question=question)
 
-    def generate_summary(self, documents: List[dict]):
-        document_summaries = []
-        document_summaries_grouped = OrderedDict()
-        for document in documents:
-            if document["metadata"]["doi"] not in document_summaries_grouped:
-                document_summaries_grouped[document["metadata"]["doi"]] = []
-            document_summaries_grouped[document["metadata"]["doi"]].append(document['text'])
-        for doi, texts in document_summaries_grouped.items():
+    def summarize_prompt(self, chunks: List[dict]):
+        return '''
+You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document, summarize its content.
+
+USER:
+Extracted parts:
+{summary}
+
+ASSISTANT:'''.format(summary=self.generate_summary(chunks))
+
+    def generate_summary(self, chunks: List[dict]):
+        chunk_summaries = []
+        chunk_summaries_grouped = OrderedDict()
+        for chunk in chunks:
+            doi = chunk.get("metadata", {}).get("doi")
+            if doi not in chunk_summaries_grouped:
+                chunk_summaries_grouped[doi] = []
+            chunk_summaries_grouped[doi].append(chunk['text'])
+        for doi, texts in chunk_summaries_grouped.items():
             texts = ' <..> '.join(texts)
-            document_summaries.append(f'DOI: {doi}\nCONTENT: {texts}')
-        return '\n'.join(document_summaries)
+            if doi:
+                chunk_summaries.append(f'DOI: {doi}\nCONTENT: {texts}')
+            else:
+                chunk_summaries.append(f'CONTENT: {texts}')
+        return '\n'.join(chunk_summaries)
 
 
 class Llama27bPrompter(BasePrompter):
-    def qa_prompt(self, question: str, documents: List[dict]):
-        if len(documents) >= 1:
+    def qa_prompt(self, question: str, chunks: List[dict]):
+        if len(chunks) >= 1:
             return '''
 <s><<SYS>>
 You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
-ALWAYS add references to extracted parts using template "DOI: 10.1038/s41576-022-00477-6" near corresponding statements. 
+ALWAYS add references to extracted parts using template "DOI: 10.1038/s41576-022-00477-6" near corresponding statements.
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 <</SYS>>
 [INST]
 Extracted parts:
 {summary}
 
 Question:
 {question}
-[/INST]'''.format(question=question, summary=self.generate_summary(documents))
+[/INST]'''.format(question=question, summary=self.generate_summary(chunks))
         else:
             return '''
 <s><<SYS>>
 You are Cybrex AI created by People of Nexus. Answer the question.
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 <</SYS>>
 [INST]
 Question:
 {question}
-[/INST]'''.format(question=question, summary=self.generate_summary(documents))
+[/INST]'''.format(question=question)
+
+    def summarize_prompt(self, chunks: List[dict]):
+        return '''
+<s><<SYS>>
+You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document, summarize its content.
+<</SYS>>
+[INST]
+Extracted parts:
+{summary}
+[/INST]'''.format(summary=self.generate_summary(chunks))
 
 
 class OpenAIPrompter(BasePrompter):
-    def qa_prompt(self, question: str, documents: List[dict]):
-        return """Given the following extracted parts of a long document and a question, create a final answer with references ("DOIs"). 
+    def qa_prompt(self, question: str, chunks: List[dict]):
+        return """Given the following extracted parts of a long document and a question, create a final answer with references ("DOIs").
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 ALWAYS return a "DOIs" part in your answer.
 
 QUESTION: Which state/country's law governs the interpretation of the contract?
 =========
 DOI: 28-pl
 CONTENT: This Agreement is governed by English law and the parties submit to the exclusive jurisdiction of the English courts in  relation to any dispute (contractual or non-contractual) concerning this Agreement save that either party may apply to any court for an  injunction or other relief to protect its Intellectual Property Rights.
@@ -112,127 +131,8 @@
 FINAL ANSWER: The president did not mention Michael Jackson.
 DOIs:
 
 QUESTION: {question}
 =========
 {summary}
 =========
-FINAL ANSWER:""".format(question=question, summary=self.generate_summary(documents))
-
-class LLM:
-    def __init__(self, llm, prompter):
-        self.llm = llm
-        self.prompter = prompter
-
-    def ask_documents(self, question, documents):
-        prompt = self.prompter.qa_prompt(question, documents)
-        logging.getLogger('statbox').info({'action': 'ask_documents', 'mode': 'llm', 'prompt': prompt})
-        return self.llm(prompt).strip()
-
-
-def get_embedding_function(model_name):
-    if model_name.startswith('hkunlp/instructor'):
-        return HuggingFaceInstructEmbeddings(
-            model_name=model_name,
-            embed_instruction="Represent science paragraph for retrieval",
-            query_instruction="Represent science question for retrieval",
-        )
-    elif model_name == "text-embedding-ada-002":
-        return OpenAIEmbeddings(model=model_name)
-    else:
-        raise ValueError("Unsupported embedding model")
-
-
-class CybrexModel:
-    def __init__(self, config):
-        self.config = config
-        self.text_splitter = RecursiveCharacterTextSplitter(
-            chunk_size=self.config['text_splitter']['chunk_size'],
-            chunk_overlap=self.config['text_splitter']['chunk_overlap'],
-        )
-
-    @classmethod
-    def standard_llms(cls, name):
-        return {
-            'llama-2-7b': {
-                'config': {
-                    'context_length': 4096,
-                    'max_new_tokens': 512,
-                    'model_path_or_repo_id': 'TheBloke/Llama-2-7B-Chat-GGML',
-                    'model_file': 'llama-2-7b-chat.ggmlv3.q4_K_S.bin',
-                },
-                'model_type': 'llama',
-                'prompter': {
-                    'type': 'llama-7b'
-                }
-            },
-            'llama-2-7b-uncensored': {
-                'config': {
-                    'context_length': 4096,
-                    'max_new_tokens': 512,
-                    'model_path_or_repo_id': 'TheBloke/Luna-AI-Llama2-Uncensored-GGML',
-                    'model_file': 'luna-ai-llama2-uncensored.ggmlv3.q4_K_S.bin',
-                },
-                'model_type': 'llama',
-                'prompter': {
-                    'type': 'default'
-                },
-            },
-            'openai': {
-                'config': {}
-            },
-        }[name]
-
-    @classmethod
-    def default_config(cls):
-        return {
-            'text_splitter': {
-                'chunk_size': 1024,
-                'chunk_overlap': 128,
-                'type': 'rcts',
-            },
-            'embedder': {
-                'model_name': 'hkunlp/instructor-xl',
-                'model_type': 'instructor',
-            },
-            'llm': cls.standard_llms("llama-2-7b-uncensored")
-        }
-
-    @lazy
-    def keyword_extractor(self):
-        return KeyBERT()
-
-    @lazy
-    def embedder(self):
-        if self.config['embedder']['model_type'] == 'instructor':
-            return HuggingFaceInstructEmbeddings(
-                model_name=self.config['embedder']['model_name'],
-                embed_instruction="Represent science paragraph for retrieval",
-                query_instruction="Represent science question for retrieval",
-            )
-        elif self.config['embedder']['model_type'] == 'openai':
-            return OpenAIEmbeddings(model=self.config['embedder']['model_name'])
-        else:
-            raise ValueError("Unsupported embedding model")
-
-    def embed_documents(self, texts: List[str]) -> List[List[float]]:
-        return self.embedder.embed_documents(texts)
-
-    @lazy
-    def llm(self):
-        if self.config['llm']['model_type'] == 'llama':
-            return LLM(
-                llm=AutoModelForCausalLM.from_pretrained(**self.config['llm']['config']),
-                prompter=BasePrompter.prompter_from_type(self.config['llm']['prompter']['type'])
-            )
-        elif self.config['llm']['model_type'] == 'openai':
-            return LLM(
-                llm=OpenAI(**self.config['llm']['config']),
-                prompter=BasePrompter.prompter_from_type(self.config['llm']['prompter']['type']),
-            )
-
-    def get_embeddings_id(self):
-        text_splitter_id = f'{self.config["text_splitter"]["type"]}' \
-                           f'-{self.config["text_splitter"]["chunk_size"]}' \
-                           f'-{self.config["text_splitter"]["chunk_overlap"]}'
-        embedder_id = self.config['embedder']['model_name'].replace('/', '-')
-        return f"{embedder_id}-{text_splitter_id}"
+FINAL ANSWER:""".format(question=question, summary=self.generate_summary(chunks))
```

### Comparing `cybrex-1.2.6/cybrex.egg-info/PKG-INFO` & `cybrex-1.3.0/cybrex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.2.6
+Version: 1.3.0
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.2.6/pyproject.toml` & `cybrex-1.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.2.6"
+version = "1.3.0"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

