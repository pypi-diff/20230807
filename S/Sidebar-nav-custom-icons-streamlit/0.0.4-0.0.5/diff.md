# Comparing `tmp/Sidebar-nav-custom-icons-streamlit-0.0.4.tar.gz` & `tmp/Sidebar-nav-custom-icons-streamlit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sidebar-nav-custom-icons-streamlit-0.0.4.tar", last modified: Sat Aug  5 17:59:19 2023, max compression
+gzip compressed data, was "Sidebar-nav-custom-icons-streamlit-0.0.5.tar", last modified: Mon Aug  7 09:36:17 2023, max compression
```

## Comparing `Sidebar-nav-custom-icons-streamlit-0.0.4.tar` & `Sidebar-nav-custom-icons-streamlit-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 17:59:19.261475 Sidebar-nav-custom-icons-streamlit-0.0.4/
--rw-rw-rw-   0        0        0     1082 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       57 2023-08-05 14:33:15.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      617 2023-08-05 17:59:19.258481 Sidebar-nav-custom-icons-streamlit-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 17:59:19.221165 Sidebar-nav-custom-icons-streamlit-0.0.4/Sidebar_nav_custom_icons_streamlit.egg-info/
--rw-rw-rw-   0        0        0      617 2023-08-05 17:59:18.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-08-05 17:59:18.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/Sidebar_nav_custom_icons_streamlit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 17:59:18.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/Sidebar_nav_custom_icons_streamlit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-05 17:59:18.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/Sidebar_nav_custom_icons_streamlit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-08-05 17:59:18.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/Sidebar_nav_custom_icons_streamlit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 17:59:19.248431 Sidebar-nav-custom-icons-streamlit-0.0.4/custom_sidebar_icons/
--rw-rw-rw-   0        0        0    14579 2023-08-05 17:57:51.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/custom_sidebar_icons/__init__.py
--rw-rw-rw-   0        0        0       42 2023-08-05 17:59:19.262476 Sidebar-nav-custom-icons-streamlit-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-08-05 17:58:29.000000 Sidebar-nav-custom-icons-streamlit-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:36:17.270253 Sidebar-nav-custom-icons-streamlit-0.0.5/
+-rw-rw-rw-   0        0        0     1082 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-08-05 14:33:15.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1600 2023-08-07 09:36:17.266257 Sidebar-nav-custom-icons-streamlit-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-08-07 09:35:31.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 09:36:17.245565 Sidebar-nav-custom-icons-streamlit-0.0.5/Sidebar_nav_custom_icons_streamlit.egg-info/
+-rw-rw-rw-   0        0        0     1600 2023-08-07 09:36:16.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-08-07 09:36:16.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/Sidebar_nav_custom_icons_streamlit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:36:16.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/Sidebar_nav_custom_icons_streamlit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-07 09:36:16.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/Sidebar_nav_custom_icons_streamlit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-07 09:36:16.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/Sidebar_nav_custom_icons_streamlit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 09:36:17.251565 Sidebar-nav-custom-icons-streamlit-0.0.5/custom_sidebar_icons/
+-rw-rw-rw-   0        0        0    20094 2023-08-07 09:27:57.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/custom_sidebar_icons/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:36:17.271781 Sidebar-nav-custom-icons-streamlit-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-08-07 09:17:32.000000 Sidebar-nav-custom-icons-streamlit-0.0.5/setup.py
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.4/LICENSE` & `Sidebar-nav-custom-icons-streamlit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.4/custom_sidebar_icons/__init__.py` & `Sidebar-nav-custom-icons-streamlit-0.0.5/custom_sidebar_icons/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import os
 import streamlit as st
 import time
   
 class Set_Nav_Emojis:
 
-    def __init__(self, emojisToRender, uniform_icon_ID="page-title-icon"):
+    def __init__(self, emojisToRender, uniform_icon_ID="page-title-icon", streamlit_cloud_app=False, my_custom_head_CDN_selector=False, append_CDN_to=""):
         """
         Load in the emojis to show - list of dictionaries. Also the uniform id for all icon ids
         """
         self.emojisToRender = emojisToRender
         self.uniform_icon_ID = uniform_icon_ID
+        self.streamlit_cloud_app = streamlit_cloud_app
+        self.my_custom_head_CDN_selector = my_custom_head_CDN_selector
+        self.append_CDN_to = append_CDN_to
 
     def create_important_session_state(self):
         """
         Create session variables to highlight that function has run. This will help to remove the iframe created from st.components.v1.html so that space is created in the app.
         """
         if "sideNav" not in st.session_state:
             st.session_state['sideNav'] = False
@@ -67,14 +70,104 @@
                 icon8_line_awesome2.rel = "stylesheet";
                 window.top.document.head.appendChild(icon8_line_awesome2);
 
             </script>
         """
         st.components.v1.html(linkJS, height=0, width=0)
 
+    def Load_All_CDNs_to_streamlit_cloud(self):
+        query = "iframe[title='streamlitApp']"
+
+        linkJS = f"""
+            <script>
+                headToAppendIframe = window.top.document.querySelectorAll("{query}")[0].contentDocument.head
+
+                const GoogleEmoji = document.createElement("link");
+                GoogleEmoji.href = "https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@48,400,0,0";
+                GoogleEmoji.rel = "stylesheet";
+                headToAppendIframe.appendChild(GoogleEmoji);
+
+                const remixIcon = document.createElement("link");
+                remixIcon.href = "https://cdn.jsdelivr.net/npm/remixicon@3.5.0/fonts/remixicon.css";
+                remixIcon.rel = "stylesheet";
+                headToAppendIframe.appendChild(remixIcon);
+
+                const tablerIcons = document.createElement("link");
+                tablerIcons.href = "https://cdn.jsdelivr.net/npm/@tabler/icons@latest/iconfont/tabler-icons.min.css";
+                tablerIcons.rel = "stylesheet";
+                headToAppendIframe.appendChild(tablerIcons); 
+
+                const tablerIcons_2 = document.createElement("link");
+                tablerIcons_2.href ="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@latest/tabler-icons.min.css";      
+                tablerIcons_2.rel = "stylesheet";
+                headToAppendIframe.appendChild(tablerIcons_2);   
+
+                const tablerIcons_3 = document.createElement("script")
+                tablerIcons_3.src = "https://cdn.jsdelivr.net/npm/@tabler/icons@latest/icons-react/dist/index.umd.min.js"
+                headToAppendIframe.appendChild(tablerIcons_3) 
+
+                const icon8_line_awesome = document.createElement("link");
+                icon8_line_awesome.href = "https://maxst.icons8.com/vue-static/landings/line-awesome/font-awesome-line-awesome/css/all.min.css";
+                icon8_line_awesome.rel = "stylesheet";
+                headToAppendIframe.appendChild(icon8_line_awesome);
+
+                const icon8_line_awesome2 = document.createElement("link");
+                icon8_line_awesome2.href = "https://maxst.icons8.com/vue-static/landings/line-awesome/line-awesome/1.3.0/css/line-awesome.min.css";
+                icon8_line_awesome2.rel = "stylesheet";
+                headToAppendIframe.appendChild(icon8_line_awesome2);
+
+            </script>
+        """
+        st.components.v1.html(linkJS, height=0, width=0)
+
+    def custom_query_for_my_app_head_tag_CDN(self):
+
+        linkJS = f"""
+            <script>
+                headToAppendIframe = {self.append_CDN_to}
+
+                const GoogleEmoji = document.createElement("link");
+                GoogleEmoji.href = "https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@48,400,0,0";
+                GoogleEmoji.rel = "stylesheet";
+                headToAppendIframe.appendChild(GoogleEmoji);
+
+                const remixIcon = document.createElement("link");
+                remixIcon.href = "https://cdn.jsdelivr.net/npm/remixicon@3.5.0/fonts/remixicon.css";
+                remixIcon.rel = "stylesheet";
+                headToAppendIframe.appendChild(remixIcon);
+
+                const tablerIcons = document.createElement("link");
+                tablerIcons.href = "https://cdn.jsdelivr.net/npm/@tabler/icons@latest/iconfont/tabler-icons.min.css";
+                tablerIcons.rel = "stylesheet";
+                headToAppendIframe.appendChild(tablerIcons); 
+
+                const tablerIcons_2 = document.createElement("link");
+                tablerIcons_2.href ="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@latest/tabler-icons.min.css";      
+                tablerIcons_2.rel = "stylesheet";
+                headToAppendIframe.appendChild(tablerIcons_2);   
+
+                const tablerIcons_3 = document.createElement("script")
+                tablerIcons_3.src = "https://cdn.jsdelivr.net/npm/@tabler/icons@latest/icons-react/dist/index.umd.min.js"
+                headToAppendIframe.appendChild(tablerIcons_3) 
+
+                const icon8_line_awesome = document.createElement("link");
+                icon8_line_awesome.href = "https://maxst.icons8.com/vue-static/landings/line-awesome/font-awesome-line-awesome/css/all.min.css";
+                icon8_line_awesome.rel = "stylesheet";
+                headToAppendIframe.appendChild(icon8_line_awesome);
+
+                const icon8_line_awesome2 = document.createElement("link");
+                icon8_line_awesome2.href = "https://maxst.icons8.com/vue-static/landings/line-awesome/line-awesome/1.3.0/css/line-awesome.min.css";
+                icon8_line_awesome2.rel = "stylesheet";
+                headToAppendIframe.appendChild(icon8_line_awesome2);
+
+            </script>
+        """
+        st.components.v1.html(linkJS, height=0, width=0)
+        
+
     def create_unique_class_for_streamlitTabs(self):
         """
             Need to create a unique identified for the <span></span> tag that contains the navigation title. This is especially important because 
             when using multiple icon libraries together, we need to position the icons next to the title. Without this unique identifier, icons will be added to the same page title.
             For example using the google-material-symbols uses <span> tag to render its icons (can also use <i> too). If we were to combine google-material-symbols and line-awesome icon library,
             when running the loop for these two libraries, javascript will continue to append icons to the first page title instead of going to the next page as it found
             google-material-sybmols icon's <span> first and thus appends the icon to its left instead of the next page title's left. A unique identified prevents this behaviour. 
@@ -241,46 +334,51 @@
         self.create_important_session_state()
 
         if st.session_state['codeHasRun'] == False:
             placeholder = st.empty()
             if st.session_state['sideNav'] == False:
                 with placeholder.container():
 
-                    self.Load_All_CDNs()
+                    if self.streamlit_cloud_app == True:
+                        self.Load_All_CDNs_to_streamlit_cloud() 
+                    elif self.my_custom_head_CDN_selector == True:
+                        self.custom_query_for_my_app_head_tag_CDN()
+                    else:
+                        self.Load_All_CDNs()
                     time.sleep(2)
-                    self.create_unique_class_for_streamlitTabs()
                     
+                    self.create_unique_class_for_streamlitTabs()
 
                     for data_object, index in zip(self.emojisToRender, range(len(self.emojisToRender))):
-                        if data_object['emojiLibrary'] == "Google_material_symbols":
+                        if data_object['iconLibrary'] == "Google_material_symbols":
                             self.Google_material_symbols(data_object, index)
-                        elif data_object['emojiLibrary'] == "line_awesome":
+                        elif data_object['iconLibrary'] == "line_awesome":
                             self.line_awesome(data_object, index)
-                        elif data_object['emojiLibrary'] == "icon_8":
+                        elif data_object['iconLibrary'] == "icon_8":
                             self.icon_8(data_object, index)
-                        elif data_object['emojiLibrary'] == "remix_icon":
+                        elif data_object['iconLibrary'] == "remix_icon":
                             self.remix_icon(data_object, index)
-                        elif data_object['emojiLibrary'] == "tabler_icons":
+                        elif data_object['iconLibrary'] == "tabler_icons":
                             self.tabler_icons(data_object, index) 
                         print(data_object, index)
                     
                     st.session_state['sideNav'] = True 
                     time.sleep(1)
                     st.experimental_rerun()
             else: 
                 placeholder.empty()
                 st.session_state['codeHasRun'] = True
 
 """
  -- Example --
 
 emojis_list = [
-    {"emojiLibrary":"remix_icon", "pageT":"two", "iconName":"ri-verified-badge-fill", "emojiObject":{}, "style":"", "elementID":"",},
-    {"emojiLibrary":"icon_8", "pageT":"init", "iconName":"settings", "emojiObject":{'src':"https://img.icons8.com/fluency/48/smiling.png", 'height':'50', 'width':'50', 'alt':'smiling'}, "style":"", "elementID":"", },
-    {"emojiLibrary":"tabler_icons", "pageT":"one", "iconName":"ti ti-adjustments-pin", "emojiObject":{}, "style":"", "elementID":"",},
+    {"iconLibrary":"remix_icon", "pageT":"two", "iconName":"ri-verified-badge-fill", "emojiObject":{}, "style":"", "elementID":"",},
+    {"iconLibrary":"icon_8", "pageT":"init", "iconName":"settings", "emojiObject":{'src':"https://img.icons8.com/fluency/48/smiling.png", 'height':'50', 'width':'50', 'alt':'smiling'}, "style":"", "elementID":"", },
+    {"iconLibrary":"tabler_icons", "pageT":"one", "iconName":"ti ti-adjustments-pin", "emojiObject":{}, "style":"", "elementID":"",},
 
 ]
 emojisOrender = Set_Nav_Emojis(emojis_list)
 emojisOrender.show_me_the_icons_Render()
 emojisOrender.create_unique_class_for_streamlitTabs()
 
 """
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.4/setup.py` & `Sidebar-nav-custom-icons-streamlit-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="Sidebar-nav-custom-icons-streamlit",
-    version="0.0.4",
+    version="0.0.5",
     author="",
     author_email="",
     description="Streamlit component that allows you to set emojis from 5 prettier icon libraries",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

