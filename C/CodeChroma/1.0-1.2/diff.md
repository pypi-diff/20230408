# Comparing `tmp/CodeChroma-1.0.tar.gz` & `tmp/CodeChroma-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CodeChroma-1.0.tar", last modified: Thu Apr  6 08:48:38 2023, max compression
+gzip compressed data, was "dist\CodeChroma-1.2.tar", last modified: Sat Apr  8 18:13:06 2023, max compression
```

## Comparing `CodeChroma-1.0.tar` & `CodeChroma-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 08:48:38.000000 CodeChroma-1.0/
-drwxrwxrwx   0        0        0        0 2023-04-06 08:48:38.000000 CodeChroma-1.0/CodeChroma/
--rw-rw-rw-   0        0        0       90 2023-04-06 07:32:22.000000 CodeChroma-1.0/CodeChroma/__init__.py
--rw-rw-rw-   0        0        0     9951 2023-04-06 08:23:15.000000 CodeChroma-1.0/CodeChroma/colors.py
--rw-rw-rw-   0        0        0     9458 2023-04-06 08:24:01.000000 CodeChroma-1.0/CodeChroma/terminalColors.py
-drwxrwxrwx   0        0        0        0 2023-04-06 08:48:38.000000 CodeChroma-1.0/CodeChroma.egg-info/
--rw-rw-rw-   0        0        0     5210 2023-04-06 08:48:37.000000 CodeChroma-1.0/CodeChroma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-04-06 08:48:38.000000 CodeChroma-1.0/CodeChroma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 08:48:37.000000 CodeChroma-1.0/CodeChroma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-06 08:48:37.000000 CodeChroma-1.0/CodeChroma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-06 08:48:37.000000 CodeChroma-1.0/CodeChroma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5210 2023-04-06 08:48:38.000000 CodeChroma-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4024 2023-04-06 08:41:54.000000 CodeChroma-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-06 08:48:38.000000 CodeChroma-1.0/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-04-06 08:48:32.000000 CodeChroma-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:06.000000 CodeChroma-1.2/
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:06.000000 CodeChroma-1.2/CodeChroma/
+-rw-rw-rw-   0        0        0       90 2023-04-06 07:32:22.000000 CodeChroma-1.2/CodeChroma/__init__.py
+-rw-rw-rw-   0        0        0     9951 2023-04-06 08:23:15.000000 CodeChroma-1.2/CodeChroma/colors.py
+-rw-rw-rw-   0        0        0    13547 2023-04-08 08:21:17.000000 CodeChroma-1.2/CodeChroma/terminalColors.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:06.000000 CodeChroma-1.2/CodeChroma.egg-info/
+-rw-rw-rw-   0        0        0     8893 2023-04-08 18:13:03.000000 CodeChroma-1.2/CodeChroma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-04-08 18:13:05.000000 CodeChroma-1.2/CodeChroma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 18:13:03.000000 CodeChroma-1.2/CodeChroma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-08 18:13:03.000000 CodeChroma-1.2/CodeChroma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-08 18:13:03.000000 CodeChroma-1.2/CodeChroma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8893 2023-04-08 18:13:06.000000 CodeChroma-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7171 2023-04-08 18:12:33.000000 CodeChroma-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 18:13:06.000000 CodeChroma-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-04-08 08:45:34.000000 CodeChroma-1.2/setup.py
```

### Comparing `CodeChroma-1.0/CodeChroma/colors.py` & `CodeChroma-1.2/CodeChroma/colors.py`

 * *Files identical despite different names*

### Comparing `CodeChroma-1.0/CodeChroma/terminalColors.py` & `CodeChroma-1.2/CodeChroma/terminalColors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,172 @@
 from pygments import highlight
 from pygments.lexers import get_lexer_by_name, guess_lexer
+from pygments.lexers.special import TextLexer
 from pygments.formatters import TerminalFormatter
 from CodeChroma.colors import Colors
 import re
 
 class TerminalColors:
     """
-       This object has all the methods for coloring text in the terminal.
-       For this function it is necessary to use the class colors that helps to color the code easier.
-        - Color the code syntax
-        - Colorize urls
-        - Colorize text between quotation marks
-        - Colorize text between brackets
-        - Match titles
-        - Search for text blocks
-        
-        Example
-            ```python
-            from CodeChroma import TerminalColors
-            termcolor = TerminalColors()
-            text = '''# Sintaxis de Java 
-                    ## Variables'''
-            colored_text = termcolor.coloring_text(text)
-            print(colored_text)
-            ```
+        Class that colors different parts of the text.
+    
+        This object has all the methods for coloring text in the terminal.
+        For this function it is necessary to use the class colors that helps to color the code easier.
+        
+        Colors:
+            - yellow
+            - light_yellow
+            - red
+            - light_red
+            - blue
+            - light_blue
+            - green
+            - light_green
+            - cyan
+            - light_cyan
+            - magenta
+            - light_magenta
+        
+        Features:
+            - Color the code syntax
+            - Colorize urls
+            - Colorize text between quotation marks
+            - Colorize text between brackets
+            - Match titles
+            - Search for text blocks
+        
+        ```python
+        from CodeChroma import TerminalColors
+        termcolor = TerminalColors()
+        text = '''# Sintaxis de Java 
+                ## Variables'''
+        colored_text = termcolor.coloring_text(text)
+        print(colored_text)
+        ```
+    
+        This class defines a dictionary with different labels and their corresponding colors, which can be modified according to the user's needs.
+        according to the user's needs. The dictionary is used to apply different colors to different parts of the text.
+        of the text. The pattern used to find the different parts of the text is defined in the `pattern` property.
+    
+        Attributes:
+            elements (dict): dictionary with different labels and their corresponding colors.
+                ```
+                    from CodeChroma import Colors
+                    color = Colors()
+                    termcolor.elements = {
+                            "title" : colors.light_blue,
+                            "block" : colors.light_green,
+                            "list-item": colors.light_yellow,
+                            "url" : colors.light_blue,
+                            "parentheses" : colors.blue,
+                            "string" : colors.magenta,
+                            "code" : colors.light_cyan
+                            }
+                ```
     """
     
-    def __init__(self):
-        # Crea la instancia que colorea el texto
-        self.colors = Colors()
+    def __init__(self, title='light_blue', block='light_green', list_item='light_yellow', url='light_blue', parentheses='blue', string='magenta', code='light_cyan', lang='green'):
+        # Creates the instance that colors the text
+        # Define a dictionary with different labels and their corresponding colors.
+        # This dictionary will be used to apply different colors to different parts of the text.
+        self._colors = Colors()
+        self.elements = {
+            "title": getattr(self._colors, title),
+            "block": getattr(self._colors, block),
+            "list-item": getattr(self._colors, list_item),
+            "url": getattr(self._colors, url),
+            "parentheses": getattr(self._colors, parentheses),
+            "string": getattr(self._colors, string),
+            "code": getattr(self._colors, code),
+            "lang": getattr(self._colors, lang)
+        }
+
+        # Search pattern to be used by the class to obtain the elements to be colorized.
+        self._pattern = r'(```.*?```|\'\'\'.*?\'\'\'|\'[^\n]*?\'|"[^\n]*?"|\'.*?\'|\`[^\n]*?\`|\(.*?\)|https?://\S+|- [^\n]*\n|#+[^\n]*\n|>.*?\n(?: {4}.*?\n)*)'
+        # This property indicates whether the identified language is to be displayed or not.
+        self.view_lang:bool = True
+        self.format_code = True
 
-        # Combinar los patrones utilizando el operador | (OR)
-        self.pattern = r'(```.*?```|\'\'\'.*?\'\'\'|\'[^\n]*?\'|"[^\n]*?"|\'.*?\'|\`[^\n]*?\`|\(.*?\)|https?://\S+|- [^\n]*\n|#+[^\n]*\n|>.*?\n(?: {4}.*?\n)*)'
 
 
     def coloring_text(self, text: str) -> str:
-        """
-            Esta funcion es la principal que colorea el texto pasado por parametro
-        """
-        return re.sub(self.pattern, self._replacement, text, flags=re.DOTALL)
+        """ This is the main function that colors the text passed by parameter. """
+        return re.sub(self._pattern, self._replacement, text, flags=re.DOTALL)
 
     def _replacement(self, match):
-        """
-            Esta función busca y valida el texto que tipo de texto es y lo colorea.
-            Retorna el el texto coloreado si cumple la condicion.
-        """
+        # This function looks for and validates the text what type of text it is and colors it.
+        # It returns the colored text if it meets the condition.
         text = match.group(1)
         
-        if self._is_code(text): return self._color_code(text)
+        if self._is_code(text): return self.color_code(text)
         elif self._is_title(text): return self._color_title(text)
         elif self._is_string(text): return self._color_string(text)
         elif self._is_parentheses(text): return self._color_parentheses(text)
         elif self._is_block(text): return self._color_block(text)
         elif self._is_url(text): return self._color_url(text)
         elif self._is_list_item(text): return self._color_list_item(text)
         else: return text
 
-    # * Aqui se guarda los metodos que colorean el string encontrado segun se defina
+    # Here are stored the methods that color the string found as defined
     
-    def _color_code(self, code: str) -> str:
-        # Primero valida el lenguaje del codigo extraido como string
-        # Primero revisa si el mismo bloque de codigo ya tiene el lenguaje especificado
-        # Si no entonces pasalo a una segunda función quebuscara patrones para detectar el lenguaje
-        # Si no entonces pasalo a una funcion dentro de la libreria pygments que detecte el lenguaje en automatico
-        # Y si al final no detecta nada entonces colorea el codigo de cyan
-        code_extract = self._extract_lang_in_string(code)
-        lang = self._detect_code_language(code) if code_extract is None else code_extract
-        code = code[3: -3] if code_extract is None else code[3 + len(lang):-3]
-        lexer = get_lexer_by_name(lang) if lang else guess_lexer(code)
+    def color_code(self, code: str) -> str:
+        """This function colors the syntax of a code passed as a string.
+
+        Args:
+            code (str): Code to color syntax.
+
+        Returns:
+            str: Returns the code already colored correctly.Returns the string with the code already colored correctly and if desired with its language identified at the top of the code.
+        """
+        
+        # First identify the language of the code passed as a string.
+        # Once with the language get the lexer that will be used to color the code.
+        try:
+            lang = self.detect_code_language(code=code)
+            lexer = get_lexer_by_name(lang)
+        except:
+            lexer = TextLexer()
+        
+        # Extracts only the part of the code you are interested in having
+        if self.format_code:
+            code_extract = self._extract_lang_in_string_markdown(text=code)
+            if re.search(r'```|~~~', code):
+                if code_extract is None:
+                    code = code[code.index('```') + 3:code.rindex('```')]
+                    code = code.replace('`', '')
+                else:
+                    code = code[code.index('```') + 3:code.rindex('```')]
+                    code = code.replace('`', '')
+                    code = code.replace(code_extract, '', 1)
+        
+        # Finally, color the text according to the language identified.
         result = highlight(code, lexer, TerminalFormatter())
-        return f"\n{self.colors.light_green(lexer.name)}\n\n{self.colors.light_cyan(result)}\n"
+        result = self.elements["code"](result)
+        result_lang = self.elements["lang"](lexer.name)
+        return f"\n{result_lang}\n\n{result}" if self.view_lang else f"\n{result}"
 
     def _color_string(self, string: str) -> str:
-        return self.colors.light_magenta(string)
-    
+        return self.elements["string"](string)
 
     def _color_parentheses(self, parentheses: str) -> str:
-        return self.colors.light_blue(parentheses)
+        return self.elements["parentheses"](parentheses)
 
     def _color_url(self, url: str) -> str:
-        return self.colors.bold(self.colors.light_blue(url))
-
+        return self._colors.bold(self.elements["url"](url))
     
     def _color_list_item(self, item: str) -> str:
-        return self.colors.bold(self.colors.light_yellow(item))
+        return self._colors.bold(self.elements["list-item"](item))
     
     def _color_title(self, title:str) -> str:
-        return self.colors.light_blue(title)
+        return self.elements["title"](title)
     
     def _color_block(self, text:str) -> str:
-        return self.colors.light_green(text)
+        return self.elements["block"](text)
         
-    # * En estos metodos se almacena la funcionalidad de validación si se encuentra cierto elemento en el texto
+    # In these methods, the validation functionality is stored if a certain element is found in the text.
     
     def _is_code(self, text: str) -> bool:
         return (text.startswith('```') and text.endswith('```')) or (text.startswith("'''\n") and text.endswith("'''\n"))
     
     def _is_string(self, text: str) -> bool:
         return (text.startswith('"') and text.endswith('"')) or (text.startswith("'") and text.endswith("'")) or (text.startswith("`") and text.endswith("`"))
     
@@ -111,27 +182,51 @@
     def _is_block(self, text: str) -> bool:
         return text.startswith('>')
     
     def _is_title(self, text: str) -> bool:
         return text.startswith('#')
 
     
-    # * Otras funcionalidades como identificar el lenguaje de un texto como codigo de programación.
+    # Other functionalities such as identifying the language of a text as programming code.
     
-    def _extract_lang_in_string(self, text:str) -> (str or None):
+    def detect_code_language(self, code:str) -> str:
+        """This function allows you to identify the language of the code passed as a string.
+
+        Args:
+            code (str): Code to identify the language.
+
+        Returns:
+            str: Returns the string with the identified language.
+        """
+        
+        lang = self._extract_lang_in_string_markdown(code)
+        lang = self._detect_language_by_regex(code) if lang is None else lang
+        if lang is None:
+            if re.search(r'```|~~~', code):
+                code = code[code.index('```') + 3:code.rindex('```')]
+                code = code.replace('`', '')
+                lang = guess_lexer(code).name
+            else: 
+                lang = guess_lexer(code).name
+        return lang
+        
+    
+    def _extract_lang_in_string_markdown(self, text:str) -> (str or None):
         """
         Esta función recibe un string y extrae el texto contenido entre los caracteres de comillas simples o dobles.
         Si no se encuentra ningún texto, retorna None.
         """
-        lang = text.split("```")[1].split("\n")[0]
-        if (len(lang) <= 0 or lang is None): return None
-        else: return lang
-        
+        try:
+            lang = text.split("```")[1].split("\n")[0]
+            if (len(lang) <= 0 or lang is None): return None
+            else: return lang
+        except:
+            return None
         
-    def _detect_code_language(self, code: str) -> (str or None):
+    def _detect_language_by_regex(self, code: str) -> (str or None):
         """Esta función recibe un texto y detecta si contiene algún código de programación en él y retorna el código encontrado."""
 
         # Definir una lista de expresiones regulares para identificar los lenguajes de programación más comunes
         regex = [
             # Buscar las palabras def, print o elif seguidas de un nombre y paréntesis
             (r"(def|print|elif)\s+\w+\(.*\)", "Python"),
             # Buscar las palabras print import o from seguidas de un nombre y paréntesis
```

### Comparing `CodeChroma-1.0/CodeChroma.egg-info/PKG-INFO` & `CodeChroma-1.2/CodeChroma.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeChroma
-Version: 1.0
+Version: 1.2
 Summary: This project is a simple library to color text in the terminal with python.
 Home-page: https://github.com/EddyBel/CodeChroma
 Author: Eduardo Rangel
 Author-email: dante61918@gmail.com
 License: MIT
 Download-URL: https://github.com/EddyBel/CodeChroma
 Description: <h1 align="center">CodeChroma</h1>
@@ -15,18 +15,26 @@
         <img src="https://img.shields.io/github/languages/top/EddyBel/CodeChroma?color=%23F9E79F&style=for-the-badge" />
         <img src="https://img.shields.io/github/languages/count/EddyBel/CodeChroma?color=%23ABEBC6&style=for-the-badge" />
         <img src="https://img.shields.io/github/languages/code-size/EddyBel/CodeChroma?color=%23F1948A&style=for-the-badge" />
         </p>
         
         <p align="center">Simple python text coloring package</p>
         
-        <p aling="center" >
+        <!-- BY LOCAL -->
+        <!-- <p aling="center" >
         <img src="./assets/Captura1.png" width="100%" />
         <img src="./assets/Captura2.png" width="100%" />
         <img src="./assets/Captura3.png" width="100%" />
+        </p> -->
+        
+        <!-- BY WEB -->
+        <p aling="center" >
+        <img src="https://raw.githubusercontent.com/EddyBel/CodeChroma/main/assets/Captura1.png" width="100%" />
+        <img src="https://raw.githubusercontent.com/EddyBel/CodeChroma/main/assets/Captura2.png" width="100%" />
+        <img src="https://raw.githubusercontent.com/EddyBel/CodeChroma/main/assets/Captura2.png" width="100%" />
         </p>
         
         The "CodeChroma" project is a Python library for highlighting and coloring text in the terminal. With this library, users can highlight code syntax and color specific markdown elements, such as titles, links, parentheses and text in quotation marks.
         
         ## Why the project?
         
         The project was created with the aim of improving the readability and aesthetics of text in projects using the terminal. On many occasions, text in the terminal can be difficult to read due to its flat, uncolored format, which can make work difficult and decrease efficiency. For this reason, a Python library was developed to allow text highlighting and coloring in a simple and easy to implement way.
@@ -44,14 +52,18 @@
         - [x] Allows you to color key elements of the markdown syntax such as code, titles, links, etc.
         - [x] Allows quick and easy implementation of the colors to be used.
         
         ## How to use
         
         The library is simple to use and only requires installation and import.
         
+        ```bash
+        pip install CodeChroma
+        ```
+        
         The library allows you to color the text using only one method of the library for ease of use.
         
         ```python
         from CodeChroma import TerminalColors
         
         # We create an instance of the library
         termcolor = TerminalColors()
@@ -79,14 +91,69 @@
         # We color the text with its method "coloring_text", the text passed by parameter
         # The function returns a new string with the text already colored.
         colored_text = termcolor.coloring_text(text)
         # We can display the new text
         print(colored_text)
         ```
         
+        ## Configuration
+        
+        The library allows for a few extra settings, which allow the user to modify and color their text as needed.
+        
+        ### Colors
+        
+        The colors can be easily modified from the parameters assigned when creating the instance of the TerminalColors class, you can write the available color you need for each colorable element.
+        
+        ```python
+        termcolor = TerminalColors(title="yellow", list_item="magenta", ...)
+        ```
+        
+        Another way to modify the colors of each element is from its elements attribute, for this it is necessary to pass some method either own of the library or personal (But it must be a method), that allows to color the text and to return the colored text.
+        
+        ```python
+        colors = Colors()
+        termcolor = TerminalColors(title="yellow", list_item="magenta")
+        termcolor.elements = {
+                "title": colors.bg_cyan,
+                "block": colors.yellow,
+                "list-item": colors.magenta,
+                "url": colors.cyan,
+                "parentheses": colors.light_red,
+                "string": colors.light_green,
+                "code": colors.yellow,
+                "lang": colors.red
+              }
+        ```
+        
+        ### Format
+        
+        The TerminalColors class has some properties that modify how the string resulting from the coloring is displayed.
+        
+        One of them is the programming language, with the view_lang property (boolean value, by default it is set to True) allows to modify if the identified language will be shown or not.
+        
+        ```python
+        termcolor.view_lang = False
+        ```
+        
+        The following format_code modifies whether the code is returned with or without the markdown code block characters "````", by default it is set to True.
+        
+        ```python
+        termcolor.format_code = False
+        ```
+        
+        ## Methods
+        
+        The TerminalColors class has some coloring methods as needed.
+        
+        | FUNCTION             | PARAMS   | DESCRIPTION                                                                                                                                                 |
+        | -------------------- | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
+        | coloring_text        | text:str | This function receives a text as a parameter and allows coloring the string with markdown formatting and features.                                          |
+        | color_code           | code:str | This function allows you to pass a code as a string, the function will identify the language and color it according to its syntax if it finds the language. |
+        | detect_code_language | code:str | This function also allows you to receive a code as a string and it will return a string with the language you identified in the code.                       |
+        
         ## Licence
         
         <h3 align="center">MIT</h3>
         
         ---
         
         <p align="center">
```

### Comparing `CodeChroma-1.0/PKG-INFO` & `CodeChroma-1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeChroma
-Version: 1.0
+Version: 1.2
 Summary: This project is a simple library to color text in the terminal with python.
 Home-page: https://github.com/EddyBel/CodeChroma
 Author: Eduardo Rangel
 Author-email: dante61918@gmail.com
 License: MIT
 Download-URL: https://github.com/EddyBel/CodeChroma
 Description: <h1 align="center">CodeChroma</h1>
@@ -15,18 +15,26 @@
         <img src="https://img.shields.io/github/languages/top/EddyBel/CodeChroma?color=%23F9E79F&style=for-the-badge" />
         <img src="https://img.shields.io/github/languages/count/EddyBel/CodeChroma?color=%23ABEBC6&style=for-the-badge" />
         <img src="https://img.shields.io/github/languages/code-size/EddyBel/CodeChroma?color=%23F1948A&style=for-the-badge" />
         </p>
         
         <p align="center">Simple python text coloring package</p>
         
-        <p aling="center" >
+        <!-- BY LOCAL -->
+        <!-- <p aling="center" >
         <img src="./assets/Captura1.png" width="100%" />
         <img src="./assets/Captura2.png" width="100%" />
         <img src="./assets/Captura3.png" width="100%" />
+        </p> -->
+        
+        <!-- BY WEB -->
+        <p aling="center" >
+        <img src="https://raw.githubusercontent.com/EddyBel/CodeChroma/main/assets/Captura1.png" width="100%" />
+        <img src="https://raw.githubusercontent.com/EddyBel/CodeChroma/main/assets/Captura2.png" width="100%" />
+        <img src="https://raw.githubusercontent.com/EddyBel/CodeChroma/main/assets/Captura2.png" width="100%" />
         </p>
         
         The "CodeChroma" project is a Python library for highlighting and coloring text in the terminal. With this library, users can highlight code syntax and color specific markdown elements, such as titles, links, parentheses and text in quotation marks.
         
         ## Why the project?
         
         The project was created with the aim of improving the readability and aesthetics of text in projects using the terminal. On many occasions, text in the terminal can be difficult to read due to its flat, uncolored format, which can make work difficult and decrease efficiency. For this reason, a Python library was developed to allow text highlighting and coloring in a simple and easy to implement way.
@@ -44,14 +52,18 @@
         - [x] Allows you to color key elements of the markdown syntax such as code, titles, links, etc.
         - [x] Allows quick and easy implementation of the colors to be used.
         
         ## How to use
         
         The library is simple to use and only requires installation and import.
         
+        ```bash
+        pip install CodeChroma
+        ```
+        
         The library allows you to color the text using only one method of the library for ease of use.
         
         ```python
         from CodeChroma import TerminalColors
         
         # We create an instance of the library
         termcolor = TerminalColors()
@@ -79,14 +91,69 @@
         # We color the text with its method "coloring_text", the text passed by parameter
         # The function returns a new string with the text already colored.
         colored_text = termcolor.coloring_text(text)
         # We can display the new text
         print(colored_text)
         ```
         
+        ## Configuration
+        
+        The library allows for a few extra settings, which allow the user to modify and color their text as needed.
+        
+        ### Colors
+        
+        The colors can be easily modified from the parameters assigned when creating the instance of the TerminalColors class, you can write the available color you need for each colorable element.
+        
+        ```python
+        termcolor = TerminalColors(title="yellow", list_item="magenta", ...)
+        ```
+        
+        Another way to modify the colors of each element is from its elements attribute, for this it is necessary to pass some method either own of the library or personal (But it must be a method), that allows to color the text and to return the colored text.
+        
+        ```python
+        colors = Colors()
+        termcolor = TerminalColors(title="yellow", list_item="magenta")
+        termcolor.elements = {
+                "title": colors.bg_cyan,
+                "block": colors.yellow,
+                "list-item": colors.magenta,
+                "url": colors.cyan,
+                "parentheses": colors.light_red,
+                "string": colors.light_green,
+                "code": colors.yellow,
+                "lang": colors.red
+              }
+        ```
+        
+        ### Format
+        
+        The TerminalColors class has some properties that modify how the string resulting from the coloring is displayed.
+        
+        One of them is the programming language, with the view_lang property (boolean value, by default it is set to True) allows to modify if the identified language will be shown or not.
+        
+        ```python
+        termcolor.view_lang = False
+        ```
+        
+        The following format_code modifies whether the code is returned with or without the markdown code block characters "````", by default it is set to True.
+        
+        ```python
+        termcolor.format_code = False
+        ```
+        
+        ## Methods
+        
+        The TerminalColors class has some coloring methods as needed.
+        
+        | FUNCTION             | PARAMS   | DESCRIPTION                                                                                                                                                 |
+        | -------------------- | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
+        | coloring_text        | text:str | This function receives a text as a parameter and allows coloring the string with markdown formatting and features.                                          |
+        | color_code           | code:str | This function allows you to pass a code as a string, the function will identify the language and color it according to its syntax if it finds the language. |
+        | detect_code_language | code:str | This function also allows you to receive a code as a string and it will return a string with the language you identified in the code.                       |
+        
         ## Licence
         
         <h3 align="center">MIT</h3>
         
         ---
         
         <p align="center">
```

### Comparing `CodeChroma-1.0/setup.py` & `CodeChroma-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 readme = open("./README.md", "r")
 
 setup(
     name="CodeChroma",
     packages=["CodeChroma"],
-    version=1.0,
+    version=1.2,
     description="This project is a simple library to color text in the terminal with python.",
     long_description=readme.read(),
     long_description_content_type="text/markdown",
     author="Eduardo Rangel",
     author_email="dante61918@gmail.com",
     url="https://github.com/EddyBel/CodeChroma",
     download_url="https://github.com/EddyBel/CodeChroma",
```

