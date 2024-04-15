# Comparing `tmp/motsmeles-2.0.0.tar.gz` & `tmp/motsmeles-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motsmeles-2.0.0.tar", max compression
+gzip compressed data, was "motsmeles-2.2.0.tar", max compression
```

## Comparing `motsmeles-2.0.0.tar` & `motsmeles-2.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      930 2024-04-08 09:40:56.625407 motsmeles-2.0.0/README.md
--rw-r--r--   0        0        0     7458 2024-04-08 09:37:18.533778 motsmeles-2.0.0/motsmeles.py
--rw-r--r--   0        0        0      402 2024-04-08 09:45:19.741954 motsmeles-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 motsmeles-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      930 2024-04-08 09:40:56.625407 motsmeles-2.2.0/README.md
+-rw-r--r--   0        0        0     7509 2024-04-15 16:05:35.091048 motsmeles-2.2.0/motsmeles.py
+-rw-r--r--   0        0        0      402 2024-04-15 16:07:48.365171 motsmeles-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 motsmeles-2.2.0/PKG-INFO
```

### Comparing `motsmeles-2.0.0/README.md` & `motsmeles-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `motsmeles-2.0.0/motsmeles.py` & `motsmeles-2.2.0/motsmeles.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 
 import numpy
 import pandas as pd
 import random
 import sys
 import builtins
 
-from psutil import sensors_battery
 
 alphabet="ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 # TODO remplacer sensPossible par allow_inverse, allow_diagonal
+class GenerateError(Exception):
+    pass
 def generate(
     mots,
     dimensionsx=10,
     dimensionsy=10,
-    sensPossible={"b","d","h","g","bg","bd","hd","hg"}
-    # allow_diagonal=True,
-    # allow_reverse=True,
+    #sensPossible={"b","d","h","g","bg","bd","hd","hg"}
+    no_diagonal=False,
+    no_reverse=False,
     ):
-    # sensPossible = {"b","d"} | (
-    #     {"bg","bd","hd","hg"} if allow_diagonal else set() &\
-    #     {"h","g","hd","bg"} if allow_reverse else set())
+
+    sensPossible={"b","d","h","g","bg","bd","hd","hg"}
+    if no_diagonal:
+        sensPossible -= {"bg","bd","hd","hg"}
+    if no_reverse:
+        sensPossible -= {"h","g","hd","bg"}
     grille = numpy.empty((dimensionsy, dimensionsx), dtype=str)
     answers = pd.DataFrame(columns=['mot', 'sens', 'x', 'y','xh', 'yh'])
-    for mot in mots:
-        #Vérification du mot
-        mot = mot.upper()
-        for letter in mot:
-            assert letter in alphabet,f"Mot invalid: {mot}"
-        dim = min(dimensionsx, dimensionsy)
-        assert len(mot) <= dim, f"Mot trop long: {mot}"
-        
-        #choix de rangey, rangex, addy, addx
-        sens = random.choice(tuple(sensPossible))
-        if "h" in sens:
+    def _generate():
+        # 1. Placer les mots
+        for mot in mots:
+            #Vérification du mot
+            mot = mot.upper()
+            for letter in mot:
+                assert letter in alphabet,f"Mot invalid: {mot}"
+            dim = min(dimensionsx, dimensionsy)
+            assert len(mot) <= dim, f"Mot trop long: {mot}"
+            
+            #choix de rangey, rangex, addy, addx
+            sens = random.choice(tuple(sensPossible))
+            if "h" in sens:
+                """if count==2: #2
+                    print("math: "+str((dimensionsy-len(mots))+1))"""
+                rangey=range((dimensionsy-len(mot))+1)
+                addy=1
+            elif "b" in sens:
+                rangey=range(len(mot)-1,dimensionsy)
+                #print("b rangey :"+str(rangey))
+                addy=-1
+            else:
+                rangey=range(dimensionsy)
+                addy=0
+            if "d" in sens:
+                rangex=range((dimensionsx-len(mot))+1)
+                addx=1
+            elif "g" in sens:
+                rangex=range(len(mot)-1,dimensionsx)
+                addx=-1
+            else:
+                rangex=range(dimensionsx)
+                addx=0
             """if count==2: #2
-                print("math: "+str((dimensionsy-len(mots))+1))"""
-            rangey=range((dimensionsy-len(mot))+1)
-            addy=1
-        elif "b" in sens:
-            rangey=range(len(mot)-1,dimensionsy)
-            #print("b rangey :"+str(rangey))
-            addy=-1
-        else:
-            rangey=range(dimensionsy)
-            addy=0
-        if "d" in sens:
-            rangex=range((dimensionsx-len(mot))+1)
-            addx=1
-        elif "g" in sens:
-            rangex=range(len(mot)-1,dimensionsx)
-            addx=-1
-        else:
-            rangex=range(dimensionsx)
-            addx=0
-        """if count==2: #2
-            print("rangey: "+str(rangey)+", rangex: "+str(rangex))"""
-        for _ in range(10):
+                print("rangey: "+str(rangey)+", rangex: "+str(rangex))"""
             choixcoordonnees=[]
             for y in rangey:
 
                 for x in rangex:
 
                     #pindex=indexSurListe(x,y)
                     #index=pindex
@@ -75,81 +80,83 @@
                         if grille[yh,xh]!="":
                             if grille[yh,xh]!=letter:
                                 break
                         xh+=addx
                         yh+=addy
                     else:               
                         choixcoordonnees.append((y,x))
-            break
-        else:
-            raise ValueError(f"Impossible de placer le mot {mot}")
-        y,x=random.choice(choixcoordonnees)
-        #xh,yh=coordonnees(index)
-        xh,yh=x,y
-        for letter in mot:
-            grille[yh,xh]=letter # a big debug: replace with yh, xh
+            if not choixcoordonnees: 
+                
+                raise GenerateError(f"Impossible de placer le mot {mot}")
+            y,x=random.choice(choixcoordonnees)
             #xh,yh=coordonnees(index)
-            #print(type(x),type(addx))
-            xh+=addx
-            yh+=addy
-        answers.loc[len(answers)] = {'mot': mot, 'sens': sens, 'x': x, 'y': y,'xh': xh, 'yh': yh}
-        #answers = answers.append({'mot': mot, 'sens': sens, 'x': x, 'y': y,'xh': xh, 'yh': yh}, ignore_index=True)
-
-            #index=indexSurListe(xh+addx,yh+addy)
-    def verifsens(addx,addy):
-
-        grille[y,x]=letter 
-        mot=letter
-        xh,yh=x,y
-        while 0<=xh<dimensionsx and 0<=yh<dimensionsy:
-            if grille[yh,xh]=="":
-                return True
-            if mot in mots:
-                return False
-            #lettrespossible.append(letter)
-            mot+=grille[yh,xh]
-            xh+=addx
-            yh+=addy 
-        return True
-    #filemotsmeles("motsmeles.txt")
-    #print(VraiReponses)
-    #rrzu=input("enter")
-    # FIXME a bug of blank letters
-    for y in range(dimensionsy):
-        for x in range(dimensionsx):
-            for _ in range(1):
-                xs,ys=x,y
-                #pindex=indexSurListe(x,y)
-                #print(index)
-                #try:
-                #    anciennelettre=letters[y,x]
-                #except IndexError:
-                #    print("len(letters) :"+str(len(letters))+"index:"+str(pindex))
-                lettrespossible=[]
-                if grille[y,x]:
-                    #print(repr(letters[y,x]))
-                    break
-                for letter in alphabet:
-                    for addx,addy in [(0,1),(1,1),(1,0),(1,-1),(0,-1),(-1,-1),(-1,0),(-1,1)]:
-                        if not verifsens(addx,addy):
+            xh,yh=x,y
+            for letter in mot:
+                grille[yh,xh]=letter # a big debug: replace with yh, xh
+                #xh,yh=coordonnees(index)
+                #print(type(x),type(addx))
+                xh+=addx
+                yh+=addy
+            answers.loc[len(answers)] = {'mot': mot, 'sens': sens, 'x': x, 'y': y,'xh': xh, 'yh': yh}
+            #answers = answers.append({'mot': mot, 'sens': sens, 'x': x, 'y': y,'xh': xh, 'yh': yh}, ignore_index=True)
+
+                #index=indexSurListe(xh+addx,yh+addy)
+        def verifsens(addx,addy):
+
+            grille[y,x]=letter 
+            mot=letter
+            xh,yh=x,y
+            while 0<=xh<dimensionsx and 0<=yh<dimensionsy:
+                if grille[yh,xh]=="":
+                    return True
+                if mot in mots:
+                    return False
+                #lettrespossible.append(letter)
+                mot+=grille[yh,xh]
+                xh+=addx
+                yh+=addy 
+            return True
+        #filemotsmeles("motsmeles.txt")
+        #print(VraiReponses)
+        #rrzu=input("enter")
+        # FIXME a bug of blank letters
+        # 2. Remplir les cases vides
+        for y in range(dimensionsy):
+            for x in range(dimensionsx):
+                for _ in range(1):
+                    xs,ys=x,y
+                    #pindex=indexSurListe(x,y)
+                    #print(index)
+                    #try:
+                    #    anciennelettre=letters[y,x]
+                    #except IndexError:
+                    #    print("len(letters) :"+str(len(letters))+"index:"+str(pindex))
+                    lettrespossible=[]
+                    if grille[y,x]:
+                        #print(repr(letters[y,x]))
+                        break
+                    for letter in alphabet:
+                        for addx,addy in [(0,1),(1,1),(1,0),(1,-1),(0,-1),(-1,-1),(-1,0),(-1,1)]:
+                            if not verifsens(addx,addy):
+                                lettrespossible.append(letter)
+                                break
+                        else:
                             lettrespossible.append(letter)
-                            break
-                    else:
-                        lettrespossible.append(letter)
-                if not lettrespossible:
-                    raise ValueError(f"Impossible de placer une lettre à {x},{y}")
-                grille[y,x]=random.choice(lettrespossible)
-            if grille[ys,xs] not in alphabet:
-                pass
-            
+                    if not lettrespossible:
+                        raise GenerateError(f"Impossible de placer une lettre à {x},{y}")
+                    grille[y,x]=random.choice(lettrespossible)
+                if grille[ys,xs] not in alphabet:
+                    pass
             
-    for y in range(dimensionsy):
-        for x in range(dimensionsx):
-            if grille[y,x] not in alphabet:
-                pass
+        return grille,answers
+    for _ in range(10):
+        try:
+            return _generate()
+        except GenerateError:
+            pass
     
     # for y in range(dimensionsy):
     #     for x in range(dimensionsx):
     #         if letters[y,x]=="":
     #             pass
                 #letters[y,x]=random.choice(alphabet)
     return grille,answers
@@ -170,42 +177,26 @@
     import argparse
     
     parser = argparse.ArgumentParser(description="générateur de mots mêlés")
     parser.add_argument("mots", nargs="+", help="les mots à placer")
     parser.add_argument("-x", "--dimensionsx", type=int, default=10, help="la largeur de la grille")
     parser.add_argument("-y", "--dimensionsy", type=int, default=10, help="la hauteur de la grille")
     #parser.add_argument("-o", "--output-file", help="fichier de sortie")
-    
+    parser.add_argument("-d","--no-diagonal", action="store_true", help="ne pas autoriser les mots en diagonale")
+    parser.add_argument("-r","--no-reverse", action="store_true", help="ne pas autoriser les mots en sens inverse")
     args=parser.parse_args()
-    grille,answers=generate(args.mots,args.dimensionsx,args.dimensionsy)
+    grille,answers=generate(
+        args.mots,
+        args.dimensionsx,
+        args.dimensionsy,
+        no_diagonal=args.no_diagonal,
+        no_reverse=args.no_reverse,
+        )
     print(grille)
     builtins.print(answers)
 if __name__=="__main__":
     main()
-#datamotsmeles()
-# reponses=["c","r","s"]
-# reponse=""
-# while reponse=="":
-#     reponse=input("\nnom du fichier ?")
-# f=open(reponse,"w")
-# f.write(data)
-# f.close()
-# print("données enregistrés avec succès")
-"""while True:
-    reponse=None
-    while reponse not in reponses:
-        reponse=input("\n\nc pour voir le code\nr pour voir les réponses\ns pour enregistrer dans un fichier")
-    if reponse=="c":
-        print("\n\ncode :\n\n"+data.replace("\n",""))
-    elif reponse=="r":
-        print("\n\nRéponses :\n"+VraiReponses)
-    else:
-        reponse=input("\n\nnom du fichier?")
-        if reponse!="":
-            f=open(reponse,"w")
-            f.write(data)
-            f.close()
-            print("données enregistrés avec succès")"""
+
```

### Comparing `motsmeles-2.0.0/PKG-INFO` & `motsmeles-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motsmeles
-Version: 2.0.0
+Version: 2.2.0
 Summary: générateur de mots mêlés
 License: MIT
 Author: RadoTheProgrammer
 Author-email: rado@arazakar.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

