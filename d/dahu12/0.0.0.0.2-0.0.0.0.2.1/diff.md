# Comparing `tmp/dahu12-0.0.0.0.2.tar.gz` & `tmp/dahu12-0.0.0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dahu12-0.0.0.0.2.tar", max compression
+gzip compressed data, was "dahu12-0.0.0.0.2.1.tar", max compression
```

## Comparing `dahu12-0.0.0.0.2.tar` & `dahu12-0.0.0.0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      136 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/__init__.py
--rw-r--r--   0        0        0     1243 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/donnees.py
--rw-r--r--   0        0        0      194 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/elec.py
--rw-r--r--   0        0        0     2469 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/erreurs.py
--rw-r--r--   0        0        0     1959 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/graph.py
--rw-r--r--   0        0        0     1466 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/main.py
--rw-r--r--   0        0        0    18393 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/maths.py
--rw-r--r--   0        0        0     1924 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/meca.py
--rw-r--r--   0        0        0     2330 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/papiers.py
--rw-r--r--   0        0        0      200 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/phy.py
--rw-r--r--   0        0        0      923 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/DAHU/test.py
--rw-r--r--   0        0        0     1261 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/LICENSE
--rw-r--r--   0        0        0      699 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/README.md
--rw-r--r--   0        0        0      521 2023-04-04 17:33:57.695870 dahu12-0.0.0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 dahu12-0.0.0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      136 2023-04-08 17:02:11.012331 dahu12-0.0.0.0.2.1/DAHU/__init__.py
+-rw-r--r--   0        0        0     1243 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/donnees.py
+-rw-r--r--   0        0        0      194 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/elec.py
+-rw-r--r--   0        0        0     2469 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/erreurs.py
+-rw-r--r--   0        0        0     1959 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/graph.py
+-rw-r--r--   0        0        0     1466 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/main.py
+-rw-r--r--   0        0        0    18747 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/maths.py
+-rw-r--r--   0        0        0     1963 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/meca.py
+-rw-r--r--   0        0        0     2330 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/papiers.py
+-rw-r--r--   0        0        0      200 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/phy.py
+-rw-r--r--   0        0        0      933 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/DAHU/test.py
+-rw-r--r--   0        0        0     1261 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/LICENSE
+-rw-r--r--   0        0        0      699 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/README.md
+-rw-r--r--   0        0        0      523 2023-04-08 17:02:11.016331 dahu12-0.0.0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 dahu12-0.0.0.0.2.1/PKG-INFO
```

### Comparing `dahu12-0.0.0.0.2/DAHU/donnees.py` & `dahu12-0.0.0.0.2.1/DAHU/donnees.py`

 * *Files identical despite different names*

### Comparing `dahu12-0.0.0.0.2/DAHU/erreurs.py` & `dahu12-0.0.0.0.2.1/DAHU/erreurs.py`

 * *Files identical despite different names*

### Comparing `dahu12-0.0.0.0.2/DAHU/graph.py` & `dahu12-0.0.0.0.2.1/DAHU/graph.py`

 * *Files identical despite different names*

### Comparing `dahu12-0.0.0.0.2/DAHU/main.py` & `dahu12-0.0.0.0.2.1/DAHU/main.py`

 * *Files identical despite different names*

### Comparing `dahu12-0.0.0.0.2/DAHU/maths.py` & `dahu12-0.0.0.0.2.1/DAHU/maths.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ## DAHU : Partie Mathematiques ##
 
 ## Faire les docstrings : """...""" ##
 
 ## Import des modules & packages essentiels ##
-
+## Packages extérieurs
 import giacpy
-import donnees
-import erreurs as er
-import random as r
+import random
+
+## Modules internes
+from DAHU.donnees import pi
 
 # Utilisation de Giac pour gestion des variables et des expressions et autres pitits trucs #
 
 ## Definitions d'objets mathématiques généraux ##
 
 class Expression :
 
@@ -112,15 +113,15 @@
             for i in range(nbl):
                 t=[]
                 for j in range(nbc):
                     t.append(0)
                 matrice.append(t)
             self.Matrice = matrice
         else :
-            er.Error_1()
+            pass
     
     def __repr__(self) : #Representation lors de l'utilisation de print()
         l = self.nbl
         chr = ""
         for i in range(l) :
             if i != 0 :
                 chr += "\n"
@@ -148,40 +149,40 @@
             if self.nbc == autre.nbc and self.nbl == autre.nbl :
                 mat = Matrice(self.nbl,self.nbc)
                 for i in range(self.nbl) :
                     for j in range(self.nbc) :
                         mat[i][j] = self[i][j] + autre[i][j]
                 return mat
             else :
-                er.Error_ma_6()
+                pass
         else :
             pass
 
     def __iadd__(self,autre) : #Utilisation de l'operateur +=
         if isinstance(autre,Matrice) :
             if self.nbl == autre.nbc and self.nbc == autre.nbl :
                 matreturn = self + autre
                 return matreturn
             else :
-                er.Error_ma_6()
+                pass
         else :
-            er.Error_ma_2(ty="Matrice")
+            pass
     
     def __sub__(self,autre) : #Soustraction de deux matrices
         if isinstance(autre,Matrice) :
             if self.nbc == autre.nbc and self.nbl == autre.nbl :
                 mat = Matrice(self.nbl,self.nbc)
                 for i in range(self.nbl) :
                     for j in range(self.nbc) :
                         mat[i][j] = self[i][j] - autre[i][j]
                 return mat
             else :
-                er.Error_ma_6()
+                pass
         else :
-            er.Error_ma_2(ty="Matrice")
+            pass
     
     def __isub__(self,autre) : #Utilisation de l'operateur -= !
         return self - autre
 
     def __mul__(self,autre) : #Multiplications (refaire les filtres)
         if isinstance(autre,Matrice) : #Matrice par matrice
             if self.nbc == autre.nbl :
@@ -197,15 +198,15 @@
         elif isinstance(autre,int) or isinstance(autre,float) : #Matrice par reel
             mat = Matrice(self.nbl,self.nbc)
             for i in range(self.nbl) :
                 for j in range(self.nbc) :
                     mat[i][j] = self[i][j]*float(autre)
             return mat
         else :
-            er.Error_6()
+            pass
 
     def __rmul__(autre,self) : #Commutativite de la multiplication par un scalaire (faire les filtres)
         if isinstance(autre,int) :
             return self*autre
         if isinstance(autre,Matrice):
             return autre*self
 
@@ -412,15 +413,15 @@
             self.r = self.module()
             self.th = self.a/self.r
         elif self.b == 0 and self.a != 0 :
             self.r = self.a
             self.th = 0
         elif self.a == 0 and self.b != 0 :
             self.r = self.b
-            self.th = (donnees.pi)/2
+            self.th = (pi)/2
         return (self.r, self.th)
 
 class Fonction(Expression) :
     def __init__(self,nom,expr,var) :
         self.Fonction = {"{}".format(nom) : expr, "var" : var}
         self.df = [] #Liste d'intervalles ou 1 intervalle (domaine de def)
         self.lim = [] #Liste des limites associées aux valeurs limval
@@ -446,17 +447,30 @@
             return b
     
     def etude() :
         pass
 
     ## Définition des différents types de fonctions
 
-class Polynôme :
-    def __init__(self):
-        pass
+class Polynôme() :
+    def __init__(self,coef,var):
+        self.coef = coef
+        p = ""
+        for i in range(len(self.coef)) :
+            a = float(self.coef[i])
+            p = p + "(" + str(a) + ")*" + var + "^(" + str(len(self.coef)-i)+ ")"
+            if i != len(self.coef) :
+                p += "+"
+        b = [var]
+        print(p)
+        self.expr = Expression(p,b)
+        self.expr = self.expr.simp()
+    
+    def __repr__(self):
+        return self.expr.sexpr
 
 class Ensemble :
 
     def __init__(self) :
         pass
 
 class Intervalle(Ensemble) :
@@ -464,15 +478,15 @@
     def __init__(self) :
         pass
 
 
 ## Définitions de quelques opérations ##
 
 def prodvec(vec1,vec2) : #Produit vectoriel de deux vecteurs de R3 (faire les filtres) !
-    if er.Error_ma_1(Vecteur,vec1,vec2) :
+    if True :
         if len(vec1) == len(vec2) == 3 :
             vec = Vecteur(3)
             vec[0] = vec1[1]*vec2[2] - vec1[2]*vec2[1]
             vec[1] = vec1[2]*vec2[0] - vec1[0]*vec2[2]
             vec[2] = vec1[0]*vec2[1] - vec1[1]*vec2[0]
         return vec
 
@@ -480,15 +494,15 @@
 ## Génération de matrices ##
 
 
 def randomatrice(lignes,colonnes,xmin=-15,xmax=15) : #Generation d'une matrice aux coefficients aleatoires
     mat = Matrice(lignes,colonnes)
     for i in range(lignes) :
         for j in range(colonnes) :
-            mat[i][j] = r.randint(xmin,xmax)
+            mat[i][j] = random.randint(xmin,xmax)
     return mat
 
 def matrice123(lignes,colonnes) : #Generation d'une matrice suivant la suite des entiers naturels !
     mat = Matrice(lignes,colonnes)
     t = 1
     for i in range(lignes) :
         for j in range(colonnes) :
@@ -519,15 +533,15 @@
     if cd != False :
         mat = Matrice(len(element),a)
         for i in range(len(element)) :
             for j in range(a) :
                 mat[i][j] = element[i][j]
         return mat
     else :
-        er.Error_ma_5()
+        pass
 
 def mat_creuse_1(ligne, colonne, valeur,n) : #Matrice creuse contenant 1 valeur à la position (ligne,colonne)
     mat = Matrice(n,n)
     mat[ligne][colonne] = valeur
     return mat
 
 ## Attention pour utiliser les mel il faut poser la multiplication dans le bon sens mel*mat !! ##
@@ -554,14 +568,17 @@
 
 ## Fonctions de Calcul algebrique ##
 
 
 def taylor(expr,var,pt,ordre) :
     expr.sucderiv(var,ordre)
 
+def approx_fourrier():
+    pass
+
 
 ## Fonctions Arithmétiques ##
 
 
 def PGCD(nb_1,nb_2) : #Renvoie le plus grand diviseur commun de deux nombres
     pass
```

### Comparing `dahu12-0.0.0.0.2/DAHU/meca.py` & `dahu12-0.0.0.0.2.1/DAHU/meca.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ## Librairie : Partie Mecanique ##
 
+from DAHU import main, maths, erreurs
+
 import main
 import maths as ma
 import erreurs as er
 
 
 ## Classes ##
```

### Comparing `dahu12-0.0.0.0.2/DAHU/papiers.py` & `dahu12-0.0.0.0.2.1/DAHU/papiers.py`

 * *Files identical despite different names*

### Comparing `dahu12-0.0.0.0.2/DAHU/test.py` & `dahu12-0.0.0.0.2.1/DAHU/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 # c.show()
 
 # a = ma.randomatrice(3,3)
 # print(a) 
 # b = a.pivots()
 # print (b)
 
-h = ma.Expression("2*x**3-6*x*y+2*y**3-3*x-3*y",var=["x","y"])
-print(h)
-a = h.deriv("x").simp()
-b = h.deriv("y").simp()
-print(a)
-print(b)
-print(h)
+# h = ma.Expression("2*x**3-6*x*y+2*y**3-3*x-3*y",var=["x","y"])
+# print(h)
+# a = h.deriv("x").simp()
+# b = h.deriv("y").simp()
+# print(a)
+# print(b)
+# print(h)
 
 # f = ma.Expression("e^(x^2-y)*(5-2*x+y)",var=["x","y"])
 # a = f.lim("x","+infinity")
 # print(a)
 
-a = ma.matrice123(4,4)
-print(a.eigenval())
+a = ma.Polynôme([1,2,3],"t")
+print(a)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dahu12-0.0.0.0.2/LICENSE` & `dahu12-0.0.0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dahu12-0.0.0.0.2/README.md` & `dahu12-0.0.0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dahu12-0.0.0.0.2/pyproject.toml` & `dahu12-0.0.0.0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DAHU12"
-version = "0.0.0.0.2"
+version = "0.0.0.0.2.1"
 description = "Package de calcul formel (pour l'instant ;=) )"
 authors = ["LOUVAT SEGURA Anthony","CHEMINOT Virgile"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MoiCAntho/DAHU"
 packages = [
     {include = "DAHU"},]
```

### Comparing `dahu12-0.0.0.0.2/PKG-INFO` & `dahu12-0.0.0.0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dahu12
-Version: 0.0.0.0.2
+Version: 0.0.0.0.2.1
 Summary: Package de calcul formel (pour l'instant ;=) )
 Home-page: https://github.com/MoiCAntho/DAHU
 License: MIT
 Author: LOUVAT SEGURA Anthony
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

