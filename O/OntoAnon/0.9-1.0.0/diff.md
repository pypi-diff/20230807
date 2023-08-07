# Comparing `tmp/ontoanon-0.9.tar.gz` & `tmp/OntoAnon-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "OntoAnon-1.0.0.tar", last modified: Mon Aug  7 10:24:17 2023, max compression
```

## Comparing `ontoanon-0.9.tar` & `OntoAnon-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,18 @@
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 ontoanon-0.9/Pipfile
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 ontoanon-0.9/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontoanon-0.9/__init__.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 ontoanon-0.9/src/anonymization.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 ontoanon-0.9/src/main.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ontoanon-0.9/.gitignore
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 ontoanon-0.9/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 ontoanon-0.9/pyproject.toml
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 ontoanon-0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 10:24:17.161721 OntoAnon-1.0.0/
+-rw-rw-rw-   0        0        0     1120 2023-08-06 15:03:57.000000 OntoAnon-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2848 2023-08-07 10:24:17.160719 OntoAnon-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2303 2023-08-07 10:22:05.000000 OntoAnon-1.0.0/README.md
+-rw-rw-rw-   0        0        0      704 2023-08-07 08:04:00.000000 OntoAnon-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 10:24:17.162721 OntoAnon-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 10:24:17.061183 OntoAnon-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 10:24:17.100183 OntoAnon-1.0.0/src/OntoAnon/
+-rw-rw-rw-   0        0        0       59 2023-08-07 07:27:02.000000 OntoAnon-1.0.0/src/OntoAnon/__init__.py
+-rw-rw-rw-   0        0        0     8446 2023-08-07 10:20:30.000000 OntoAnon-1.0.0/src/OntoAnon/__main__.py
+-rw-rw-rw-   0        0        0    16068 2023-08-07 09:11:22.000000 OntoAnon-1.0.0/src/OntoAnon/anonymization.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:24:17.156729 OntoAnon-1.0.0/src/OntoAnon.egg-info/
+-rw-rw-rw-   0        0        0     2848 2023-08-07 10:24:17.000000 OntoAnon-1.0.0/src/OntoAnon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-08-07 10:24:17.000000 OntoAnon-1.0.0/src/OntoAnon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 10:24:17.000000 OntoAnon-1.0.0/src/OntoAnon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-07 10:24:17.000000 OntoAnon-1.0.0/src/OntoAnon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 10:24:17.000000 OntoAnon-1.0.0/src/OntoAnon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 10:24:17.000000 OntoAnon-1.0.0/src/OntoAnon.egg-info/top_level.txt
```

### Comparing `ontoanon-0.9/src/anonymization.py` & `OntoAnon-1.0.0/src/OntoAnon/anonymization.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,24 @@
 import rdflib, time
 from rdflib import Graph, Literal, URIRef, BNode
 from rdflib.namespace import Namespace
 
 predefined_ns = [ns for ns in rdflib.namespace._NAMESPACE_PREFIXES_RDFLIB.values()] + [ns for ns in rdflib.namespace._NAMESPACE_PREFIXES_CORE.values()]
 predefined_ns.append(rdflib.Namespace("http://www.w3.org/2003/11/swrl#")) # This one was missing
 
-def anonymize(filename, fileformat, anony_path, dict_path, all_ns):
+def anonymize(filename: str, fileformat: str, anony_path: str, dict_path: str, all_ns: list):
+    """Starts the anonymization for a file
+
+    Args:
+        filename (str): _description_
+        fileformat (str): _description_
+        anony_path (str): _description_
+        dict_path (str): _description_
+        all_ns (list): _description_
+    """
     # Create a Graph
     start_time = time.time()
     g = Graph(store="SimpleMemory")
     
 
 
 
@@ -67,15 +76,23 @@
     end_time = time.time()
     execution_time = int(end_time - start_time)
     
     # Showing a message that the process is finished.
     messagebox.showinfo("System-Message", f"Anonymization is finished.\nExecution time: {execution_time} seconds")
 
 # identifying the elements of a ontology graph
-def identify_elements(g):
+def identify_elements(g:rdflib.Graph):
+    """Fills the global variables for the elements in a graph
+
+    Args:
+        g (rdflib.Graph): The loaded Graph
+
+    Returns:
+        lists: Namespaces, Objects, Predicates, Subjects
+    """
     # init lists
     namespaces = []
     subjects = []
     predicates = []
     objects = []
 
     # get the namespaces
@@ -92,16 +109,22 @@
     # delete doubles
     namespaces = list(dict.fromkeys(namespaces))
     subjects = list(dict.fromkeys(subjects))
     predicates = list(dict.fromkeys(predicates))
     objects = list(dict.fromkeys(objects))
     return namespaces, objects, predicates, subjects
 
-# translates the namespaces to generic namespaces
-def namespace_to_generic_namespace(namespaces, translator, all_ns):
+def namespace_to_generic_namespace(namespaces: list, translator: list, all_ns: list)->None:
+    """Translates the namespaces to anynomized versions
+
+    Args:
+        namespaces (list): List with all namespaces
+        translator (list): list containing the translation (empty and initialized at time of calling)
+        all_ns (list): The namespaces that shall be translated
+    """
     name_counter = 0
     standard_ns = False
 
     for name_element in namespaces:
         # check if namespace standard namespace
         for ns in all_ns:
             if (URIRef(name_element[1]) in Namespace(ns)) :
@@ -125,15 +148,15 @@
 # translates the subjects to generic subjects
 def subject_to_generic_subject(subjects:list, namespace_translator:list, all_ns:list):
     """Translates a list of subjects
 
     Args:
         subjects (list): The subjects (list of URIRefs) to be translated
         namespace_translator (list): The already translated namespaces
-        all_ns (list): The list of standard-Namespaces
+        all_ns (list): The list of standard-Namespaces that shall not be translated
 
     Returns:
         dict: key value pair for original and translated values
     """
     subject_translator = {}
     subj_counter = 0
     standard_ns = False
@@ -174,14 +197,25 @@
                 subject_translator.update({subj_element: Literal("Subject" + str(subj_counter), datatype=subj_element.datatype, lang=subj_element.language)})
         subj_counter = subj_counter + 1
         standard_ns = False
     return subject_translator
 
 # translates the predicates to generic predicates
 def predicate_to_generic_predicat(predicates: list, namespace_translator: list, subject_translator: dict, all_ns:list)-> dict:
+    """Translates all predicates, regarding the already translated terms (in this case: subjects)
+
+    Args:
+        predicates (list): The predicates (list of URIRefs) to be translated
+        namespace_translator (list): The already translated namespaces
+        all_ns (list): The list of standard-Namespaces that shall not be translated
+        subject_translator (dict): The already translated Subjects
+
+    Returns:
+        dict: Translation of the predicates
+    """
     predicate_translator = {}
     predicat_counter = 0
     standard_ns = False
     for pred_element in predicates:
         # check if namespace standard namespace
         for ns in all_ns:
             if (URIRef(pred_element) in Namespace(ns)) :
@@ -222,15 +256,27 @@
         elif not standard_ns:
             predicate_translator.update({pred_element: Literal("Predicate" + str(predicat_counter))})
         predicat_counter = predicat_counter + 1
 
         standard_ns = False
     return predicate_translator
 # translates the objects to generic objects
-def object_to_generic_object(objects, namespace_translator, subject_translator, predicat_translator, all_ns):
+def object_to_generic_object(objects, namespace_translator: list, subject_translator: dict, predicat_translator: dict, all_ns: list)->dict:
+    """Tranlsates the objects to generic ones (anonymized). Regards the already translated terms (subjects & predicates)
+
+    Args:
+        objects (list): The objects (list of URIRefs) to be translated
+        namespace_translator (list): The already translated namespaces
+        all_ns (list): The list of standard-Namespaces that shall not be translated
+        subject_translator (dict): The already translated Subjects
+        predicat_translator (dict): The already translated predicates
+
+    Returns:
+        dict: translated objects
+    """
     object_counter = 0
     object_translator = {}
     for obj_element in objects:
         # check if namespace standard namespace
         standard_ns = False
         for ns in all_ns:
             if (URIRef(obj_element) in Namespace(ns)) :
```

### Comparing `ontoanon-0.9/src/main.py` & `OntoAnon-1.0.0/src/OntoAnon/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,137 +5,145 @@
 from tkinter.filedialog import askopenfilename, asksaveasfile
 from rdflib.util import guess_format
 import rdflib
 
 import anonymization
 
 
-# choosing the ontology file
-def choose_open_file():
-    filename = askopenfilename(title="Ontology File")
-    onto_text.delete(0, END)
-    onto_text.insert(0, filename)
-
-# choosing where to store the anonymized ontology
-def choose_anon_file():
-        path = asksaveasfile(title="Anonymized File")
-        anon_text.delete(0, END)
-        anon_text.insert(0, path)
-        start = "<_io.TextIOWrapper name='"
-        end = "' mode='w' encoding='cp1252'>"
-        filename = anon_filename.get()[anon_filename.get().find(start)+len(start):anon_filename.get().rfind(end)]
-        anon_text.delete(0, END)
-        anon_text.insert(0, filename)
-
-# choosing where to store the dictionary file
-def choose_dict_file():
-        filename = asksaveasfile(title="Dictionary File")
-        dict_text.delete(0, END)
-        dict_text.insert(0, filename)
-        start = "<_io.TextIOWrapper name='"
-        end = "' mode='w' encoding='cp1252'>"
-        filename = dict_filename.get()[dict_filename.get().find(start)+len(start):dict_filename.get().rfind(end)]
-        dict_text.delete(0, END)
-        dict_text.insert(0, filename)
 
-def choose_namespaces():
-    global SELECTED_NS
-    values = [str(val) for val in anonymization.predefined_ns]
-    values += [str(e) for e in SELECTED_NS if str(e) not in values]
-    def add_value():
-        global SELECTED_NS
-        new_value = new_value_entry.get()
-        if new_value:
-            values.append(new_value)
-            listbox.insert(tk.END, new_value) 
-            listbox.selection_set(tk.END, tk.END)
-            new_value_entry.delete(0, tk.END)
-            SELECTED_NS.append(new_value)
-        else:
-            messagebox.showwarning("Warning", "Please enter a value.")
 
-    def select_all():
-        listbox.select_set(0, tk.END)
 
-    def deselect_all():
-        listbox.selection_clear(0, tk.END)
+def start_gui():
+    """Calls the GUI to be started
+    """
+    # choosing the ontology file
+    def choose_open_file():
+        filename = askopenfilename(title="Ontology File")
+        onto_text.delete(0, END)
+        onto_text.insert(0, filename)
+
+    # choosing where to store the anonymized ontology
+    def choose_anon_file():
+            path = asksaveasfile(title="Anonymized File")
+            anon_text.delete(0, END)
+            anon_text.insert(0, path)
+            start = "<_io.TextIOWrapper name='"
+            end = "' mode='w' encoding='cp1252'>"
+            filename = anon_filename.get()[anon_filename.get().find(start)+len(start):anon_filename.get().rfind(end)]
+            anon_text.delete(0, END)
+            anon_text.insert(0, filename)
+
+    # choosing where to store the dictionary file
+    def choose_dict_file():
+            filename = asksaveasfile(title="Dictionary File")
+            dict_text.delete(0, END)
+            dict_text.insert(0, filename)
+            start = "<_io.TextIOWrapper name='"
+            end = "' mode='w' encoding='cp1252'>"
+            filename = dict_filename.get()[dict_filename.get().find(start)+len(start):dict_filename.get().rfind(end)]
+            dict_text.delete(0, END)
+            dict_text.insert(0, filename)
 
-    def submit_selection():
+    def choose_namespaces():
         global SELECTED_NS
-        SELECTED_NS = [listbox.get(index) for index in listbox.curselection()]
-        predefinied_NS = [ns for ns in  anonymization.predefined_ns if str(ns) in SELECTED_NS]
-        custom_NS = [rdflib.Namespace(ns) for ns in SELECTED_NS if ns not in predefinied_NS]
-        SELECTED_NS = predefinied_NS + custom_NS
-        root.destroy()
-
-    
-    root = tk.Tk()
-    root.geometry("500x400")
-    root.title("Value Selection")
-
-    # Frame for the listbox and scrollbar
-    frame = ttk.Frame(root)
-    frame.pack(pady=2, padx=2, fill=tk.BOTH)
-
-    # Scrollbar
-    scrollbar = ttk.Scrollbar(frame)
-    scrollbar.pack(side=tk.RIGHT, fill=tk.Y)
-
-    # Listbox
-    listbox = tk.Listbox(frame, width=300, selectmode=tk.MULTIPLE, yscrollcommand=scrollbar.set)
-    i = 0
-    for value in values:
-        listbox.insert(tk.END, value)
-        if value in [str(element) for element in  SELECTED_NS]:
-            listbox.select_set(tk.END, tk.END)
-            # listbox.activate(tk.END)
-            i += 1
-    listbox.pack(side=tk.LEFT, fill=tk.BOTH)
-    scrollbar.config(command=listbox.yview)
-    if len(SELECTED_NS) == 0:
-        select_all()
-    # Entry for adding new values
-    new_value_entry = ttk.Entry(root)
-    new_value_entry.pack(pady=5, fill=tk.X)
-
-    # Buttons
-    add_button = ttk.Button(root, text="Add Value", command=add_value)
-    add_button.pack(fill=tk.X)
-    select_all_button = ttk.Button(root, text="Select All", command=select_all)
-    select_all_button.pack(fill=tk.X, pady=5)
-    deselect_all_button = ttk.Button(root, text="Deselect All", command=deselect_all)
-    deselect_all_button.pack(fill=tk.X)
-    submit_button = ttk.Button(root, text="Submit", command=submit_selection)
-    submit_button.pack(fill=tk.X, pady=10)
-
-    root.mainloop()
-    
-
-# identifing the format of the ontology
-def identify_file_format():
-    try:
-        format = guess_format(onto_filename.get())
-        format_text.delete(0,END)
-        format_text.insert(0,format)
-    except Exception:
-        format_text.delete(0,END)
-        format_text.insert(0,'The file is missing, an url or not supported.')
-
-# calling the anonymization method
-def anonymize():
-    global SELECTED_NS
-    if len(SELECTED_NS) == 0:
-        SELECTED_NS = anonymization.predefined_ns
-    if (onto_filename.get() == "" or onto_format.get() == "" or anon_filename.get() == "" or dict_filename.get() == "" ):
-        messagebox.showerror("Error", "Not all values set!")
-    else:
-        anonymization.anonymize(onto_filename.get(), onto_format.get(), anon_filename.get(), dict_filename.get(), SELECTED_NS)
-
+        values = [str(val) for val in anonymization.predefined_ns]
+        values += [str(e) for e in SELECTED_NS if str(e) not in values]
+        def add_value():
+            global SELECTED_NS
+            new_value = new_value_entry.get()
+            if new_value:
+                values.append(new_value)
+                listbox.insert(tk.END, new_value) 
+                listbox.selection_set(tk.END, tk.END)
+                new_value_entry.delete(0, tk.END)
+                SELECTED_NS.append(new_value)
+            else:
+                messagebox.showwarning("Warning", "Please enter a value.")
+
+        def select_all():
+            listbox.select_set(0, tk.END)
+
+        def deselect_all():
+            listbox.selection_clear(0, tk.END)
+
+        def submit_selection():
+            global SELECTED_NS
+            SELECTED_NS = [listbox.get(index) for index in listbox.curselection()]
+            predefinied_NS = [ns for ns in  anonymization.predefined_ns if str(ns) in SELECTED_NS]
+            custom_NS = [rdflib.Namespace(ns) for ns in SELECTED_NS if ns not in predefinied_NS]
+            SELECTED_NS = predefinied_NS + custom_NS
+            root.destroy()
+
+        
+        root = tk.Tk()
+        root.geometry("500x400")
+        root.title("Value Selection")
+
+        # Frame for the listbox and scrollbar
+        frame = ttk.Frame(root)
+        frame.pack(pady=2, padx=2, fill=tk.BOTH)
+
+        # Scrollbar
+        scrollbar = ttk.Scrollbar(frame)
+        scrollbar.pack(side=tk.RIGHT, fill=tk.Y)
+
+        # Listbox
+        listbox = tk.Listbox(frame, width=300, selectmode=tk.MULTIPLE, yscrollcommand=scrollbar.set)
+        i = 0
+        for value in values:
+            listbox.insert(tk.END, value)
+            if value in [str(element) for element in  SELECTED_NS]:
+                listbox.select_set(tk.END, tk.END)
+                # listbox.activate(tk.END)
+                i += 1
+        listbox.pack(side=tk.LEFT, fill=tk.BOTH)
+        scrollbar.config(command=listbox.yview)
+        if len(SELECTED_NS) == 0:
+            select_all()
+        # Entry for adding new values
+        new_value_entry = ttk.Entry(root)
+        new_value_entry.pack(pady=5, fill=tk.X)
+
+        # Buttons
+        add_button = ttk.Button(root, text="Add Value", command=add_value)
+        add_button.pack(fill=tk.X)
+        select_all_button = ttk.Button(root, text="Select All", command=select_all)
+        select_all_button.pack(fill=tk.X, pady=5)
+        deselect_all_button = ttk.Button(root, text="Deselect All", command=deselect_all)
+        deselect_all_button.pack(fill=tk.X)
+        submit_button = ttk.Button(root, text="Submit", command=submit_selection)
+        submit_button.pack(fill=tk.X, pady=10)
+
+        root.mainloop()
+        
+
+    # identifing the format of the ontology
+    def identify_file_format():
+        """Identifies the file format of the ontology (e.g., turtle, rdf/xml)
+        """
+        try:
+            format = guess_format(onto_filename.get())
+            format_text.delete(0,END)
+            format_text.insert(0,format)
+        except Exception:
+            format_text.delete(0,END)
+            format_text.insert(0,'The file is missing, an url or not supported.')
+
+
+    def anonymize():
+        """calling the anonymization method
+        """
+        global SELECTED_NS
+        if len(SELECTED_NS) == 0:
+            SELECTED_NS = anonymization.predefined_ns
+        if (onto_filename.get() == "" or onto_format.get() == "" or anon_filename.get() == "" or dict_filename.get() == "" ):
+            messagebox.showerror("Error", "Not all values set!")
+        else:
+            anonymization.anonymize(onto_filename.get(), onto_format.get(), anon_filename.get(), dict_filename.get(), SELECTED_NS)
 
-if __name__ == '__main__':
     global SELECTED_NS
     if "SELECTED_NS" not in globals():
         SELECTED_NS = []
 # Main window
     # create a window
     main_window = Tk()
     # set window title
@@ -179,8 +187,13 @@
     Button(main_window, text='Anonymized File', command=choose_anon_file).grid(row=2, column=2, padx=5, sticky=EW)
     Button(main_window, text='Dictionary File', command=choose_dict_file).grid(row=2, column=3, padx=5, sticky=EW)
     Button(main_window, text='Namespaces', command=choose_namespaces).grid(row=2, column=4, padx=5, sticky=EW)
 
     Button(main_window, text='Anonymize', command=anonymize).grid(row=11, column=0, padx=5, sticky=EW)
 
     # run window in loop
-    main_window.mainloop()
+    main_window.mainloop()
+
+    
+if __name__ == '__main__':
+    print("start OntoAnon")
+    start_gui()
```

### Comparing `ontoanon-0.9/README.md` & `OntoAnon-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # OntoAnon
 ***An Application For Anonymizing Ontologies.***
 
 OntoAnon iterates through all triples of a graph and anonymizes/removes the data while preserving the ontology structure. Data is preserved by keeping standard vocabulary like the ontology languages *OWL, RDF(S), SHACL*, but also standardized ontologies like *FOAF, DC, SKOS*. A full list of kept namespaces can be found [here](https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.namespace.html#namespace-utilities). OntoAnon runs locally, so no data leaves the computer. It allows sharing the structural data and using online tools like [neontometrics](http://neontometrics.com) or the OntolOlogy Pitfall Scanner ([OOPS](https://oops.linkeddata.es/)), without giving away company secrets.
 
+To use the software, either use the prepackaged .exe file at github, or install the software using `pip install OntoAnon` and call `OntoAnon` from the terminal.
+
 OntoAnon builds on the python GUI TKinter and [rdflib](https://rdflib.readthedocs.io/en/stable/index.html). The former is preinstalled with current python versions, the latter can be acquired using pip or the corresponding pipfile.
 
 The tool is part of a publication currently under review. The development of the tool was part of a bachelor thesis by Robert Schlücker, cf. https://github.com/Junech1/Ontology-Anonymisation for the original repository.
 
 
 ````mermaid
 %%{init: {'theme':'neutral', fontSize: '20px'}}%%
```

### Comparing `ontoanon-0.9/PKG-INFO` & `OntoAnon-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-Metadata-Version: 2.1
-Name: OntoAnon
-Version: 0.9
-Summary: A Structural Anonymizer for Ontologies
-Project-URL: Homepage, https://github.com/Uni-Rostock-Win/OntoAnon
-Project-URL: Bug Tracker, https://github.com/Uni-Rostock-Win/OntoAnon/issues
-Author: Robert Schlücker
-Author-email: Achim Reiz <achim.reiz@uni-rostock.de>
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# OntoAnon
-***An Application For Anonymizing Ontologies.***
-
-OntoAnon iterates through all triples of a graph and anonymizes/removes the data while preserving the ontology structure. Data is preserved by keeping standard vocabulary like the ontology languages *OWL, RDF(S), SHACL*, but also standardized ontologies like *FOAF, DC, SKOS*. A full list of kept namespaces can be found [here](https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.namespace.html#namespace-utilities). OntoAnon runs locally, so no data leaves the computer. It allows sharing the structural data and using online tools like [neontometrics](http://neontometrics.com) or the OntolOlogy Pitfall Scanner ([OOPS](https://oops.linkeddata.es/)), without giving away company secrets.
-
-OntoAnon builds on the python GUI TKinter and [rdflib](https://rdflib.readthedocs.io/en/stable/index.html). The former is preinstalled with current python versions, the latter can be acquired using pip or the corresponding pipfile.
-
-The tool is part of a publication currently under review. The development of the tool was part of a bachelor thesis by Robert Schlücker, cf. https://github.com/Junech1/Ontology-Anonymisation for the original repository.
-
-
-````mermaid
-%%{init: {'theme':'neutral', fontSize: '20px'}}%%
-   graph LR
-    A([Start]) --> D
-    subgraph Iterate over elements
-    C -- True:<br>Go to <br>next element --> D{Check if<br>standard<br> namespace}
-    D -- True --> E[Do not translate]
-    I -- True --> J{Check if<br>object is<br>already<br> translated}
-    J -- True --> K[Use<br>existing<br>translation]
-    K --> F
-    S -- Is blind-node --> 
-    J -- False --> M[Translate with <br>counter variable]
-    M --> F
-    I -- False --> O[Translate<br>namespace]
-    O --> M
-    
-    D -- False --> S{Check<br>element<br>type}
-    S -- Is<br>URI --> I{Check if<br>URI is in<br> a known<br>namespace}
-    S -- Is<bR>literal --> T{Check if element<br> is a number}
-    T -- True --> E
-    T -->  M
-
-    E --> F[counter + 1]
-    F --> C{More<br>Elements <br> available?}
-    end
-    C -- False --> AB([Return<br>translation])
-
-```
+Metadata-Version: 2.1
+Name: OntoAnon
+Version: 1.0.0
+Summary: A Structural Anonymizer for Ontologies
+Author-email: Achim Reiz <achim.reiz@uni-rostock.de>
+Project-URL: Homepage, https://github.com/Uni-Rostock-Win/OntoAnon
+Project-URL: Bug Tracker, https://github.com/Uni-Rostock-Win/OntoAnon/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# OntoAnon
+***An Application For Anonymizing Ontologies.***
+
+OntoAnon iterates through all triples of a graph and anonymizes/removes the data while preserving the ontology structure. Data is preserved by keeping standard vocabulary like the ontology languages *OWL, RDF(S), SHACL*, but also standardized ontologies like *FOAF, DC, SKOS*. A full list of kept namespaces can be found [here](https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.namespace.html#namespace-utilities). OntoAnon runs locally, so no data leaves the computer. It allows sharing the structural data and using online tools like [neontometrics](http://neontometrics.com) or the OntolOlogy Pitfall Scanner ([OOPS](https://oops.linkeddata.es/)), without giving away company secrets.
+
+To use the software, either use the prepackaged .exe file at github, or install the software using `pip install OntoAnon` and call `OntoAnon` from the terminal.
+
+OntoAnon builds on the python GUI TKinter and [rdflib](https://rdflib.readthedocs.io/en/stable/index.html). The former is preinstalled with current python versions, the latter can be acquired using pip or the corresponding pipfile.
+
+The tool is part of a publication currently under review. The development of the tool was part of a bachelor thesis by Robert Schlücker, cf. https://github.com/Junech1/Ontology-Anonymisation for the original repository.
+
+
+````mermaid
+%%{init: {'theme':'neutral', fontSize: '20px'}}%%
+   graph LR
+    A([Start]) --> D
+    subgraph Iterate over elements
+    C -- True:<br>Go to <br>next element --> D{Check if<br>standard<br> namespace}
+    D -- True --> E[Do not translate]
+    I -- True --> J{Check if<br>object is<br>already<br> translated}
+    J -- True --> K[Use<br>existing<br>translation]
+    K --> F
+    S -- Is blind-node --> 
+    J -- False --> M[Translate with <br>counter variable]
+    M --> F
+    I -- False --> O[Translate<br>namespace]
+    O --> M
+    
+    D -- False --> S{Check<br>element<br>type}
+    S -- Is<br>URI --> I{Check if<br>URI is in<br> a known<br>namespace}
+    S -- Is<bR>literal --> T{Check if element<br> is a number}
+    T -- True --> E
+    T -->  M
+
+    E --> F[counter + 1]
+    F --> C{More<br>Elements <br> available?}
+    end
+    C -- False --> AB([Return<br>translation])
+
+```
```

