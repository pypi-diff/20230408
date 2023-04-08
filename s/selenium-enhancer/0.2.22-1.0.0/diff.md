# Comparing `tmp/selenium_enhancer-0.2.22.tar.gz` & `tmp/selenium_enhancer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_enhancer-0.2.22.tar", last modified: Mon Oct 11 14:21:42 2021, max compression
+gzip compressed data, was "selenium_enhancer-1.0.0.tar", last modified: Sat Apr  8 18:47:03 2023, max compression
```

## Comparing `selenium_enhancer-0.2.22.tar` & `selenium_enhancer-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2021-10-11 14:21:42.000000 selenium_enhancer-0.2.22/
--rw-rw-rw-   0        0        0     2184 2021-10-11 14:21:42.000000 selenium_enhancer-0.2.22/PKG-INFO
--rw-rw-rw-   0        0        0     1307 2021-08-20 21:09:39.000000 selenium_enhancer-0.2.22/README.md
-drwxrwxrwx   0        0        0        0 2021-10-11 14:21:42.000000 selenium_enhancer-0.2.22/selenium_enhancer.egg-info/
--rw-rw-rw-   0        0        0     2184 2021-10-11 14:21:42.000000 selenium_enhancer-0.2.22/selenium_enhancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2021-10-11 14:21:42.000000 selenium_enhancer-0.2.22/selenium_enhancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-11 14:21:42.000000 selenium_enhancer-0.2.22/selenium_enhancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2021-10-11 14:21:42.000000 selenium_enhancer-0.2.22/selenium_enhancer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15712 2021-10-11 13:36:11.000000 selenium_enhancer-0.2.22/selenium_enhancer.py
--rw-rw-rw-   0        0        0       42 2021-10-11 14:21:42.000000 selenium_enhancer-0.2.22/setup.cfg
--rw-rw-rw-   0        0        0      867 2021-10-11 14:20:59.000000 selenium_enhancer-0.2.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:47:03.605860 selenium_enhancer-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-08 18:46:56.000000 selenium_enhancer-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-08 18:47:03.605860 selenium_enhancer-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:47:03.605860 selenium_enhancer-1.0.0/selenium_enhancer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-08 18:47:03.000000 selenium_enhancer-1.0.0/selenium_enhancer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-08 18:47:03.000000 selenium_enhancer-1.0.0/selenium_enhancer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:47:03.000000 selenium_enhancer-1.0.0/selenium_enhancer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:47:03.000000 selenium_enhancer-1.0.0/selenium_enhancer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 18:47:03.000000 selenium_enhancer-1.0.0/selenium_enhancer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:47:03.000000 selenium_enhancer-1.0.0/selenium_enhancer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-08 18:47:03.605860 selenium_enhancer-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:46:56.000000 selenium_enhancer-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `selenium_enhancer-0.2.22/PKG-INFO` & `selenium_enhancer-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,76 @@
-Metadata-Version: 2.1
-Name: selenium_enhancer
-Version: 0.2.22
-Summary: A package to enhance your Selenium WebDriver experience
-Home-page: https://github.com/dannybrown37/SeleniumEnhancer
-Author: Danny Brown
-Author-email: dannybrown37@gmail.com
-License: UNKNOWN
-Description: # Installation
-        
-        ```
-        pip install selenium-enhancer
-        ```
-        
-        # Getting Started
-        
-        ```python
-        from selenium_enhancer import SeleniumEnhancer
-        
-        class ClassName(SeleniumEnhancer):
-        
-            def complete_web_form(self):
-                self.start_chrome_driver()
-                self.driver.get("full-url-of-page-with-form.com")
-                self.set_input_elements({
-                    "id or CSS selector or XPath" : "value I want to set",
-                    "second id or CSS selector or XPath" : "second value"
-                })
-                self.set_select_elements({
-                    "name or id of select element" : "partial/complete text of option"
-                })
-                self.click_button("submitButtonId")
-        
-        
-        driver = ClassName()
-        driver.complete_web_form()
-        ```
-        
-        # Setting Up a Driver
-        
-        [ChromeDriver](https://chromedriver.chromium.org/) is recommended as it has more options, but Firefox and IE drivers are compatible as well. Set the path to your chosen driver as a system environment variable named CHROME_DRIVER FIREFOX_DRIVER, or IE_DRIVER.
-        
-        # Examples
-        
-        See/run `examples.py` for usage examples.
-        
-        # Miscellaneous
-        
-        [PyPi](https://pypi.org/project/selenium-enhancer/)
-        
-        
-        # Updating PyPi (notes to self)
-        
-        1. Update version number in setup.py
-        2. Commit to Git
-        3. `python setup.py sdist`
-        4. `twine upload --skip-existing dist/*`
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: selenium_enhancer
+Version: 1.0.0
+Summary: A package to streamline and enhance your Selenium code
+Home-page: https://github.com/dannybrown37/SeleniumEnhancer
+Author: Danny Brown
+Author-email: danny.public.emails@gmail.com
+License: MIT
+Keywords: selenium
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Installation
+
+```
+pip install selenium-enhancer
+```
+
+# Setting Up a Driver
+
+After installing or whenver you need to update to the latest version of
+ChromeDriver, run:
+
+```
+python -m selenium_enhancer.get_latest_chrome_driver
+```
+
+[ChromeDriver](https://chromedriver.chromium.org/) is recommended as it has 
+more options, but Firefox and IE drivers are in theory compatible as well.
+Please feel free to contribute if you need additional functionality.
+
+# Getting Started
+
+```python
+from selenium_enhancer import SeleniumEnhancer
+
+class ClassName(SeleniumEnhancer):
+
+    def complete_web_form(self):
+        self.start_chrome_driver()
+        self.driver.get("full-url-of-page-with-form.com")
+        self.set_input_elements({
+            "id or CSS selector or XPath" : "value I want to set",
+            "second id or CSS selector or XPath" : "second value"
+        })
+        self.set_select_elements({
+            "name or id of select element" : "partial/complete text of option"
+        })
+        self.click_button("submitButtonId")
+
+
+driver = ClassName()
+driver.complete_web_form()
+```
+
+# Examples
+
+If you're cloning the repo to contribute, you can run/view/add to the tests
+with at ``pytest tests -s -vv``.
+
+# Miscellaneous
+
+[PyPi](https://pypi.org/project/selenium-enhancer/)
+
+
+# Updating PyPi (notes to self)
+
+1. Update version number in setup.py
+2. Commit to Git
+3. `python setup.py sdist`
+4. `twine upload --skip-existing dist/*`
+
```

### Comparing `selenium_enhancer-0.2.22/selenium_enhancer.egg-info/PKG-INFO` & `selenium_enhancer-1.0.0/selenium_enhancer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,76 @@
-Metadata-Version: 2.1
-Name: selenium-enhancer
-Version: 0.2.22
-Summary: A package to enhance your Selenium WebDriver experience
-Home-page: https://github.com/dannybrown37/SeleniumEnhancer
-Author: Danny Brown
-Author-email: dannybrown37@gmail.com
-License: UNKNOWN
-Description: # Installation
-        
-        ```
-        pip install selenium-enhancer
-        ```
-        
-        # Getting Started
-        
-        ```python
-        from selenium_enhancer import SeleniumEnhancer
-        
-        class ClassName(SeleniumEnhancer):
-        
-            def complete_web_form(self):
-                self.start_chrome_driver()
-                self.driver.get("full-url-of-page-with-form.com")
-                self.set_input_elements({
-                    "id or CSS selector or XPath" : "value I want to set",
-                    "second id or CSS selector or XPath" : "second value"
-                })
-                self.set_select_elements({
-                    "name or id of select element" : "partial/complete text of option"
-                })
-                self.click_button("submitButtonId")
-        
-        
-        driver = ClassName()
-        driver.complete_web_form()
-        ```
-        
-        # Setting Up a Driver
-        
-        [ChromeDriver](https://chromedriver.chromium.org/) is recommended as it has more options, but Firefox and IE drivers are compatible as well. Set the path to your chosen driver as a system environment variable named CHROME_DRIVER FIREFOX_DRIVER, or IE_DRIVER.
-        
-        # Examples
-        
-        See/run `examples.py` for usage examples.
-        
-        # Miscellaneous
-        
-        [PyPi](https://pypi.org/project/selenium-enhancer/)
-        
-        
-        # Updating PyPi (notes to self)
-        
-        1. Update version number in setup.py
-        2. Commit to Git
-        3. `python setup.py sdist`
-        4. `twine upload --skip-existing dist/*`
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: selenium-enhancer
+Version: 1.0.0
+Summary: A package to streamline and enhance your Selenium code
+Home-page: https://github.com/dannybrown37/SeleniumEnhancer
+Author: Danny Brown
+Author-email: danny.public.emails@gmail.com
+License: MIT
+Keywords: selenium
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Installation
+
+```
+pip install selenium-enhancer
+```
+
+# Setting Up a Driver
+
+After installing or whenver you need to update to the latest version of
+ChromeDriver, run:
+
+```
+python -m selenium_enhancer.get_latest_chrome_driver
+```
+
+[ChromeDriver](https://chromedriver.chromium.org/) is recommended as it has 
+more options, but Firefox and IE drivers are in theory compatible as well.
+Please feel free to contribute if you need additional functionality.
+
+# Getting Started
+
+```python
+from selenium_enhancer import SeleniumEnhancer
+
+class ClassName(SeleniumEnhancer):
+
+    def complete_web_form(self):
+        self.start_chrome_driver()
+        self.driver.get("full-url-of-page-with-form.com")
+        self.set_input_elements({
+            "id or CSS selector or XPath" : "value I want to set",
+            "second id or CSS selector or XPath" : "second value"
+        })
+        self.set_select_elements({
+            "name or id of select element" : "partial/complete text of option"
+        })
+        self.click_button("submitButtonId")
+
+
+driver = ClassName()
+driver.complete_web_form()
+```
+
+# Examples
+
+If you're cloning the repo to contribute, you can run/view/add to the tests
+with at ``pytest tests -s -vv``.
+
+# Miscellaneous
+
+[PyPi](https://pypi.org/project/selenium-enhancer/)
+
+
+# Updating PyPi (notes to self)
+
+1. Update version number in setup.py
+2. Commit to Git
+3. `python setup.py sdist`
+4. `twine upload --skip-existing dist/*`
+
```

