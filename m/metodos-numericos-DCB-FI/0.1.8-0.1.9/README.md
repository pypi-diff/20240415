# Comparing `tmp/metodos_numericos_dcb_fi-0.1.8.tar.gz` & `tmp/metodos_numericos_dcb_fi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "metodos_numericos_dcb_fi-0.1.9.tar", max compression
```

## Comparing `metodos_numericos_dcb_fi-0.1.8.tar` & `metodos_numericos_dcb_fi-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,13 @@
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/requirements.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/data/__init__.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/data/text_es.json
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/__init__.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/configuracion.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/extras.py
--rw-r--r--   0        0        0    12846 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/graficar.py
--rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/leerEntrada.py
--rw-r--r--   0        0        0     9634 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/mostrarResultados.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/validacion.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/README.md
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 metodos_numericos_dcb_fi-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-02 18:33:51.463488 metodos_numericos_dcb_fi-0.1.9/LICENSE
+-rw-r--r--   0        0        0      865 2024-04-09 03:34:15.508268 metodos_numericos_dcb_fi-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-04-02 18:33:51.464359 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:33:51.464625 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/data/__init__.py
+-rw-r--r--   0        0        0     4345 2024-04-02 18:33:51.464868 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/data/text_es.json
+-rw-r--r--   0        0        0      531 2024-04-02 18:33:51.465318 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/__init__.py
+-rw-r--r--   0        0        0     3386 2024-04-02 18:33:51.465574 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/configuracion.py
+-rw-r--r--   0        0        0     3510 2024-04-02 18:33:51.465811 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/extras.py
+-rw-r--r--   0        0        0    15069 2024-04-02 18:33:51.466126 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/graficar.py
+-rw-r--r--   0        0        0    10045 2024-04-02 18:33:51.466406 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/leerEntrada.py
+-rw-r--r--   0        0        0     9634 2024-04-02 18:33:51.466682 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/mostrarResultados.py
+-rw-r--r--   0        0        0     4178 2024-04-02 18:33:51.466914 metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/validacion.py
+-rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 metodos_numericos_dcb_fi-0.1.9/PKG-INFO
```

### Comparing `metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/data/text_es.json` & `metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/data/text_es.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'Utilidades'": "{'Entrada': {'variable': 'La variable {1} debe ser una letra latina, griega o "*

 * *                 "combinacion de ambas.'}}"}*

```diff
@@ -10,14 +10,15 @@
             "matriz_nxn_2": "Ingrese el tama\u00f1o de la matriz cuadrada (debe ser un numero entero mayor que 0): ",
             "matriz_nxn_3": "Ingrese el elemento {1},{2}: ",
             "opcion": "Ingrese la opci\u00f3n deseada: ",
             "polinomio_1": "Reglas para ingresar polinomios:\n1.- EL grado del polinomio debe ser un numero entero mayor a 0.\n2.- Los coeficientes deben ser n\u00fameros reales.\n3.- Al menos 1 de los coeficientes debe ser distinto de cero.",
             "polinomio_2": "Ingrese el grado del polinomio: ",
             "tolerancia_1": "La tolerancia debe ser un n\u00famero real mayor que cero.",
             "tolerancia_2": "Ingrese la tolerancia: ",
+            "variable": "La variable {1} debe ser una letra latina, griega o combinacion de ambas.",
             "vector_1": "Reglas para ingresar un vector:\n1.- Los elementos deben ser n\u00fameros reales.",
             "vector_2": "Ingrese el elemento {1}: ",
             "vector_K_1": "Si desea utilizar el vector de Krilov por defecto ingrese 0. En caso contrario ingrese 1.",
             "vector_K_2": "n2.- Al menos un elemento debe ser distinto de cero."
         },
         "Errores": {
             "biseccion": "El valor de x_i debe ser menor que el de x_s.\nValores ingresados: x_i = {1}, x_s = {2}.",
```

### Comparing `metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/__init__.py` & `metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/__init__.py`

 * *Files identical despite different names*

### Comparing `metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/configuracion.py` & `metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/configuracion.py`

 * *Files identical despite different names*

### Comparing `metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/extras.py` & `metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/extras.py`

 * *Files identical despite different names*

### Comparing `metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/graficar.py` & `metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/graficar.py`

 * *Files 13% similar despite different names*

```diff
@@ -216,7 +216,67 @@
         puntos = g.data[3]
         grafica.line.color = color
         puntos.marker.color = color
         fig.add_trace(grafica)
         fig.add_trace(puntos)
 
     fig.show() # ¡¡¡NO MODIFICAR!!!
+
+def graficar(valores:list,**configuracion:dict):
+    if configuracion['titulo'] != None:
+        titulo = configuracion['titulo']
+    else:
+        titulo = f'Grafica de f(x) con intervalo [{a}, {b}]'
+    if configuracion['labels'] != None:
+        eje_x = configuracion['labels'][0]
+        eje_y = configuracion['labels'][1]
+    else:
+        eje_x = 'x'
+        eje_y = 'f(x)'
+    
+    # Configuraciones predeterminadAs para graficar
+    if configuracion['metodo'] == 'Euler':
+        mode_ = 'makers'
+        name_='Euler'
+        markers = dict(size=8, symbol='diamond', color='lime')
+        showlegend_=True
+    elif configuracion['metodo'] == 'Euler M':
+        mode_ = 'makers'
+        name_='Euler modificado'
+        markers = dict(size=8, symbol='triangle-up', color='darkviolet')
+        showlegend_=True
+    elif configuracion['metodo'] == 'RK4':
+        mode_ = 'makers'
+        name_='Runge-Kutta 4'
+        markers = dict(size=8, symbol='triangle-down', color='hotpink')
+        showlegend_=True
+    elif configuracion['metodo'] == 'Analitica':
+        mode_ = 'lines'
+        name_ = 'Solución analítica'
+        lines = dict(color='blue', width=2)
+        showlegend_ = True
+    
+    fig = go.Figure() # Crear figura
+    fig.update_layout(title=titulo, title_x=0.5, xaxis_title=eje_x, yaxis_title=eje_y)
+    
+    if mode_ == 'makers':
+        fig.add_trace(go.Scatter(x=valores[0], y=valores[1], mode='markers', marker=markers, showlegend=showlegend_, name=name_))
+    elif mode_ == 'lines':
+        fig.add_trace(go.Scatter(x=valores[0], y=valores[1], mode='lines', line=lines, showlegend=showlegend_, name=name_))
+    fig.show() # ¡¡¡NO MODIFICAR!!!
+    return fig
+
+def compararMetodos(titulo, *graficas, **configuracion):
+    if configuracion['labels'] != None:
+        eje_x = configuracion['labels'][0]
+        eje_y = configuracion['labels'][1]
+    else:
+        eje_x = 'x'
+        eje_y = 'f(x)'
+    
+    fig = go.Figure() # Crear figura
+    fig.update_layout(title=titulo, title_x=0.5, title_y=0.9, xaxis_title=eje_x, yaxis_title=eje_y, legend_title='Métodos') # ¡¡¡NO MODIFICAR!!!
+
+    for g in graficas:
+        fig.add_trace(g)
+    fig.show() # ¡¡¡NO MODIFICAR!!!
+    return fig
```

### Comparing `metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/leerEntrada.py` & `metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/leerEntrada.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # ------------------- Importar módulos -------------------
 from metodos_numericos_dcb_fi.utilidades.configuracion import text
 from metodos_numericos_dcb_fi.utilidades.validacion import validarTipo
+from metodos_numericos_dcb_fi.utilidades.configuracion import letras_griegas, letras_latinas
 
 # ------------------- Importar bibliotecas -------------------
 import sympy as sp
 from sympy.abc import x
 import numpy as np
 
 # ------------------- Crear la clase funcion -------------------
@@ -34,19 +35,19 @@
     - f_text (str): Texto de la función.
     - f (function): Función simbólica de sympy.
     - f_ (function): Función lambda de numpy.
     """ 
         self.valores_x = []
         self.valores_y = []
         self.limites = []
-        self.f_text = None
-        self.f = None
-        self.f_ = None
+        self.f_text = None # Texto
+        self.f = None # Lambdify
+        self.f_ = None # Sympify
     
-    def setFuncion(self, f):
+    def setFuncion(self, f:str, var:str='x'):
         '''
     Establece la función de la instancia actual con la función especificada.
 
     Parámetros:
         - f (str): La función matemática especificada como una cadena de texto.
 
     Excepciones:
@@ -61,22 +62,46 @@
         validarTipo(f, str)
         f = f.replace('^', '**').replace('sen', 'sin').replace('tg', 'tan').replace('ctg', 'cot')
         self.f_text = f
         try:
             self.f_ = sp.sympify(self.f_text)
         except:
             raise Exception(f'{text["Utilidades"]["Errores"]["funcion"].replace("{1}", self.f_text)}')
-        self.f = sp.lambdify(x, self.f_, 'numpy')
+        for _ in var:
+            if _ not in letras_latinas and _ not in letras_griegas:
+                raise Exception(f'{text["Utilidades"]["Errores"]["variable"].replace("{1}", _)}')
+        self.f = sp.lambdify(var, self.f_, 'numpy')
 
     def agregarLimites(self, x_i:float, x_f:float):
         validarTipo(x_i, (int, float))
         validarTipo(x_f, (int, float))
         self.limites = [(x_i, x_f)]
 # ------------------- Funciones -------------------
-def leerFuncion(f:str='')->funcion:
+def convertirFuncion(f:str, var:str='x')->funcion:
+    '''
+    Convierte una función matemática especificada como una cadena de texto en una instancia de la clase 'funcion'.
+
+    Parámetros:
+        f (str): La función matemática especificada como una cadena de texto.
+        var (str): La variable de la función. Por defecto es 'x'.
+
+    Excepciones:
+        No se generan excepciones.
+
+    Retorno:
+        Una instancia de la clase 'funcion' con la función especificada.
+
+    Ejemplo:
+        f = convertirFuncion("x**2 + 3*x - 2")
+    '''
+    f_ = funcion()
+    f_.setFuncion(f, var)
+    return f_
+
+def leerFuncion()->funcion:
     '''
     Lee una función matemática ingresada por el usuario y la asigna a una instancia de la clase 'funcion'.
 
     Parámetros:
         f (str): la funcion en forma de scadena que se va a asignar a la instancia de la clase 'funcion'. Por defecto es una cadena vacía.
 
     Excepciones:
@@ -85,17 +110,16 @@
     Retorno:
         Una instancia de la clase 'funcion' con la función asignada.
 
     Ejemplo:
         f = leerFuncion()
     '''
     f_ = funcion()
-    if f == '':
-        print(text["Utilidades"]["Entrada"]["funcion_1"])
-        f = input(f'{text["Utilidades"]["Entrada"]["funcion_2"]}')
+    print(text["Utilidades"]["Entrada"]["funcion_1"])
+    f = input(f'{text["Utilidades"]["Entrada"]["funcion_2"]}')
     f_.setFuncion(f)
     return f_
     
 def leerTolerancia(t:str='')->float:
     '''
     Lee la tolerancia ingresada por el usuario y la devuelve como un número de punto flotante.
```

### Comparing `metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/mostrarResultados.py` & `metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/mostrarResultados.py`

 * *Files identical despite different names*

### Comparing `metodos_numericos_dcb_fi-0.1.8/src/metodos_numericos_dcb_fi/utilidades/validacion.py` & `metodos_numericos_dcb_fi-0.1.9/src/metodos_numericos_dcb_fi/utilidades/validacion.py`

 * *Files identical despite different names*

### Comparing `metodos_numericos_dcb_fi-0.1.8/LICENSE` & `metodos_numericos_dcb_fi-0.1.9/LICENSE`

 * *Files identical despite different names*

