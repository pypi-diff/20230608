# Comparing `tmp/pytc2-0.0.2.tar.gz` & `tmp/pytc2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytc2-0.0.2.tar", max compression
+gzip compressed data, was "pytc2-0.0.3.tar", max compression
```

## Comparing `pytc2-0.0.2.tar` & `pytc2-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1080 2023-04-18 22:36:19.453348 pytc2-0.0.2/LICENSE
--rw-r--r--   0        0        0      859 2023-04-18 22:36:19.457348 pytc2-0.0.2/README.md
--rw-r--r--   0        0        0      896 2023-05-09 22:54:14.724460 pytc2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1858 2023-04-18 22:36:19.477348 pytc2-0.0.2/src/pytc2/__init__.py
--rw-r--r--   0        0        0    21251 2023-05-09 22:25:00.708452 pytc2-0.0.2/src/pytc2/cuadripolos.py
--rw-r--r--   0        0        0    32307 2023-05-09 22:25:00.708452 pytc2-0.0.2/src/pytc2/dibujar.py
--rw-r--r--   0        0        0     1763 2023-04-20 20:45:17.511151 pytc2-0.0.2/src/pytc2/ej5.13 schaumann.py
--rw-r--r--   0        0        0     4811 2023-05-09 22:25:00.708452 pytc2-0.0.2/src/pytc2/general.py
--rw-r--r--   0        0        0     2376 2023-04-18 22:36:19.481348 pytc2-0.0.2/src/pytc2/imagen.py
--rw-r--r--   0        0        0     8598 2023-04-18 22:36:19.481348 pytc2-0.0.2/src/pytc2/ltspice.py
--rw-r--r--   0        0        0    16960 2023-04-19 14:59:38.942917 pytc2-0.0.2/src/pytc2/remociones.py
--rw-r--r--   0        0        0     6525 2023-04-18 22:36:19.481348 pytc2-0.0.2/src/pytc2/sintesis_dipolo.py
--rw-r--r--   0        0        0    56375 2023-04-19 15:02:51.214773 pytc2-0.0.2/src/pytc2/sistemas_lineales.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 pytc2-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1080 2023-03-16 20:30:12.472103 pytc2-0.0.3/LICENSE
+-rw-r--r--   0        0        0      859 2023-03-16 20:30:12.472103 pytc2-0.0.3/README.md
+-rw-r--r--   0        0        0      896 2023-06-08 18:46:31.720831 pytc2-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1858 2023-03-16 20:30:12.484103 pytc2-0.0.3/src/pytc2/__init__.py
+-rw-r--r--   0        0        0    25387 2023-05-17 17:46:27.675590 pytc2-0.0.3/src/pytc2/cuadripolos.py
+-rw-r--r--   0        0        0    34468 2023-05-10 15:48:49.219338 pytc2-0.0.3/src/pytc2/dibujar.py
+-rw-r--r--   0        0        0     1763 2023-04-10 11:40:38.258066 pytc2-0.0.3/src/pytc2/ej5.13 schaumann.py
+-rw-r--r--   0        0        0     5848 2023-05-17 17:40:21.343582 pytc2-0.0.3/src/pytc2/general.py
+-rw-r--r--   0        0        0      152 2023-05-17 17:40:39.227583 pytc2-0.0.3/src/pytc2/imagen.py
+-rw-r--r--   0        0        0     8598 2023-03-16 20:30:12.484103 pytc2-0.0.3/src/pytc2/ltspice.py
+-rw-r--r--   0        0        0    16960 2023-04-27 18:40:16.186351 pytc2-0.0.3/src/pytc2/remociones.py
+-rw-r--r--   0        0        0     6525 2023-03-16 20:30:12.488103 pytc2-0.0.3/src/pytc2/sintesis_dipolo.py
+-rw-r--r--   0        0        0    55723 2023-06-08 18:39:19.464827 pytc2-0.0.3/src/pytc2/sistemas_lineales.py
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 pytc2-0.0.3/PKG-INFO
```

### Comparing `pytc2-0.0.2/LICENSE` & `pytc2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.2/README.md` & `pytc2-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.2/pyproject.toml` & `pytc2-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "pytc2"
-version = "0.0.2"
+version = "0.0.3"
 description = "A circuit theory module for students at Universidad Tecnológica Nacional Regional Buen"
 authors = ["Mariano Llamedo Soria"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.12, >=3.8"
```

### Comparing `pytc2-0.0.2/src/pytc2/__init__.py` & `pytc2-0.0.3/src/pytc2/__init__.py`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.2/src/pytc2/cuadripolos.py` & `pytc2-0.0.3/src/pytc2/cuadripolos.py`

 * *Files 20% similar despite different names*

```diff
@@ -462,14 +462,137 @@
     # Y21 = -1/B
     YY[1,0] = sp.simplify(sp.expand(-1/TT[0,1]))
     # Y22 = A/B
     YY[1,1] = sp.simplify(sp.expand(TT[0,0]/TT[0,1]))
     
     return(YY)
 
+def I2Tabcd_s(gamma, z01, z02 = None):
+    '''
+    Convierte la MAD en MAI luego de levantar de referencia.
+
+    Parameters
+    ----------
+    gamma : Symbol
+        Ganancia compleja expresada en neppers (Re{gamma}) y rad (Im{gamma}).
+        
+    z01 : Symbol
+        Nivel de impedancia del puerto 1.
+
+    z02 : Symbol
+        (Opcional) Nivel de impedancia del puerto 2. Default: z02 = z01 = Zo (imp. característica). 
+
+    Returns
+    -------
+    TT : Symbolic Matrix
+        Matriz ABCD en función de los parámetros imagen 
+
+    '''
+    
+    if z02 is None:
+        z02 = z01
+    
+    TT = sp.Matrix([[sp.cosh(gamma)*sp.sqrt(z01/z02),
+                     sp.sinh(gamma)*sp.sqrt(z01*z02)], 
+                    [sp.sinh(gamma)/sp.sqrt(z01*z02),
+                     sp.cosh(gamma)*sp.sqrt(z02/z01)]])
+    
+    
+    return(TT)
+
+
+def Model_conversion( src_model, dst_model  ):
+    '''
+    Convierte modelos de cuadripolos lineales.
+
+    Parameters
+    ----------
+    src_model : Dict. 
+        Diccionario que describe al modelo de origen.
+        
+    dst_model : Dict. 
+        Diccionario que describe al modelo de salida.
+
+    Returns
+    -------
+    YY : Symbolic Matrix
+        Matriz admitancia 
+
+    Example
+    -------
+
+    # Parámetros Z (impedancia - circ. abierto)
+    ZZ = sp.Matrix([[z11, z12], [z21, z22]])
+    # vars. dependientes
+    vv = sp.Matrix([[v1], [v2]])
+    # vars. INdependientes
+    ii = sp.Matrix([[i1], [i2]])
+    
+    
+    # Parámetros Tdcba (Transmisión inversos, DCBA)
+    TTi = sp.Matrix([[Ai, Bi], [-Ci, -Di]])
+    # vars. dependientes
+    ti_dep = sp.Matrix([[v2], [i2]])
+    # vars. INdependientes. (Signo negativo de corriente)
+    ti_ind = sp.Matrix([[v1], [i1]])
+    
+    # Diccionario con la definición de cada modelo
+    src_model = { 'model_name': 'Z', 'matrix': ZZ, 'dep_var': vv, 'indep_var':ii }
+    dst_model = { 'model_name': 'T', 'matrix': TT, 'dep_var': t_dep, 'indep_var':t_ind, 'neg_i2_current': True }
+    
+    T_z = convert_params( src_model, dst_model )
+    
+    print_latex(a_equal_b_latex_s('T_Z', T_z ))
+
+
+    '''
+    
+    aa = sp.solve([ src_model['matrix'] * src_model['indep_var'] - src_model['dep_var']
+                ], 
+                dst_model['dep_var'])
+    
+    # reemplazaremos el determinante por Delta.
+    det_src_matrix = sp.det(src_model['matrix'])
+    
+    # i2 se define al revés en este modelo
+    if 'neg_i2_current' in src_model:
+        det_src_matrix = -det_src_matrix
+    
+    
+    dd = sp.Symbol('\Delta')
+    jj = 0
+    
+    QQ = sp.Matrix([[0,0],[0,0]])
+
+    for dep_var in dst_model['dep_var']:
+
+        jj += 1
+        
+        yyy = sp.collect(sp.expand(aa[dep_var]), dst_model['indep_var'][0])
+        yyy = sp.collect(yyy, dst_model['indep_var'][1])
+
+        # i2 se define al revés en este modelo
+        if dep_var.name == 'i2' and 'neg_i2_current' in dst_model:
+            yyy = -yyy
+
+        kk = 0
+        for indep_var in dst_model['indep_var']:
+            kk += 1
+            
+            bb = sp.cancel(yyy.coeff(indep_var,1))
+            # i2 se define al revés en este modelo
+            if indep_var.name == 'i2' and 'neg_i2_current' in dst_model:
+                bb = -bb
+                
+            QQ[jj-1,kk-1] = bb.subs(det_src_matrix, dd)
+            #print_latex(a_equal_b_latex_s( param_lab + '{:d}{:d}'.format(jj,kk), QQ[jj-1,kk-1] ))
+
+    return({'matrix': QQ, 'name': dst_model['model_name'] + '_{' + src_model['model_name'] + '}' })
+
+
 def Y2Tabcd(YY):
     """
     
     Parameters
     ----------
     tfa : TYPE
         DESCRIPTION.
@@ -768,14 +891,44 @@
     # C = 1/Z21
     Tpar[1,0] = Yexc
     # D = Z22/Z21
     Tpar[1,1] = 1
     
     return( Tpar ) 
 
+def I2Tabcd(gamma, z01, z02 = None):
+    '''
+    Convierte la MAD en MAI luego de levantar de referencia.
+
+    Parameters
+    ----------
+    Ymai : Symbolic Matrix
+        Matriz admitancia indefinida.
+    nodes2del : list or integer
+        Nodos que se van a eliminar.
+
+    Returns
+    -------
+    YY : Symbolic Matrix
+        Matriz admitancia 
+
+    '''
+    if z02 is None:
+        z02 = z01
+
+    # if np.sqrt(z02/z01)
+    
+    TT = np.matrix([[np.cosh(gamma)*np.sqrt(z01/z02),
+                     np.sinh(gamma)*np.sqrt(z01*z02)], 
+                    [np.sinh(gamma)/np.sqrt(z01*z02),
+                     np.cosh(gamma)*np.sqrt(z02/z01)]])
+    
+    return(TT)
+
+
 def calc_MAI_ztransf_ij_mn(Ymai, ii=2, jj=3, mm=0, nn=1, verbose=False):
     """Calcula la transferencia de impedancia V_ij / I_mn
 
     Parameters
     ----------
     tfa : TYPE
         DESCRIPTION.
```

### Comparing `pytc2-0.0.2/src/pytc2/dibujar.py` & `pytc2-0.0.3/src/pytc2/dibujar.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,41 +46,47 @@
 
     '''
     
     # Dibujo la red Tee
     
     d = Drawing(unit=4)  # unit=2 makes elements have shorter than normal leads
     
-    d = dibujar_puerto_entrada(d,
-                                   port_name = 'In' )
+    d = dibujar_puerto_entrada(d, port_name = '' )
+
+    bSymbolic = isinstance(ZZ, sp.Basic)
     
-    Za = sp.simplify(sp.expand(ZZ[0,0] - ZZ[0,1]))
-    Zb = sp.simplify(sp.expand(ZZ[0,1]))
-    Zc = sp.simplify(sp.expand(ZZ[1,1] - ZZ[0,1]))
+    Za = ZZ[0,0] - ZZ[0,1]
+    Zb = ZZ[0,1]
+    Zc = ZZ[1,1] - ZZ[0,1]
+    
+    if bSymbolic:
+        
+        Za = sp.simplify(sp.expand(Za))
+        Zb = sp.simplify(sp.expand(Zb))
+        Zc = sp.simplify(sp.expand(Zc))
+
     
     if( not Za.is_zero ):
         d = dibujar_elemento_serie(d, ResistorIEC, Za )
 
     if( not Zb.is_zero ):
         d = dibujar_elemento_derivacion(d, ResistorIEC, Zb )
     
     if( not Zc.is_zero ):
         d = dibujar_elemento_serie(d, ResistorIEC, Zc )
         
     
-    d = dibujar_puerto_salida(d, 
-                                  port_name = 'Out')
+    d = dibujar_puerto_salida(d, port_name = '')
 
     display(d)        
     
     if(return_components):
         return([Za,Zb,Zc])
     
 
-
 def dibujar_Pi(YY, return_components = False):
     '''
     Dibuja una red Pi a partir de la matriz Y.
 
     Parameters
     ----------
     Ymai : Symbolic Matrix
@@ -95,53 +101,138 @@
 
     '''
     
     # Dibujo la red Tee
     
     d = Drawing(unit=4)  # unit=2 makes elements have shorter than normal leads
     
-    d = dibujar_puerto_entrada(d,
-                                   port_name = 'In')
+    d = dibujar_puerto_entrada(d, port_name = '')
     
-    Ya = sp.simplify(sp.expand(YY[0,0] + YY[0,1]))
-    Yb = sp.simplify(sp.expand(-YY[0,1]))
-    Yc = sp.simplify(sp.expand(YY[1,1] + YY[0,1]))
+    Ya = YY[0,0] + YY[0,1]
+    Yb = -YY[0,1]
+    Yc = YY[1,1] + YY[0,1]
     
     bSymbolic = isinstance(YY[0,0], sp.Basic)
     
     if bSymbolic:
         
         Za = sp.simplify(sp.expand(1/Ya))
         Zb = sp.simplify(sp.expand(1/Yb))
         Zc = sp.simplify(sp.expand(1/Yc))
         
     else:
 
-        Za = 1/(YY[0,0] + YY[0,1])
-        Zb = 1/(-YY[0,1])
-        Zc = 1/(YY[1,1] + YY[0,1])
+        Za = 1/Ya
+        Zb = 1/Yb
+        Zc = 1/Yc
     
     if( bSymbolic and (not Ya.is_zero) or (not bSymbolic) and Ya != 0 ):
         d = dibujar_elemento_derivacion(d, ResistorIEC, Za )
 
     if( bSymbolic and (not Yb.is_zero) or (not bSymbolic) and Yb != 0 ):
         d = dibujar_elemento_serie(d, ResistorIEC, Zb )
 
     if( bSymbolic and (not Yc.is_zero) or (not bSymbolic) and Yc != 0 ):
         d = dibujar_elemento_derivacion(d, ResistorIEC, Zc )
     
-    d = dibujar_puerto_salida(d, 
-                                  port_name = 'Out')
+    d = dibujar_puerto_salida(d, port_name = '')
     
     display(d)        
 
     if(return_components):
         return([Ya, Yb, Yc])
 
 
+def dibujar_lattice(ZZ=None, return_components = False):
+    '''
+    Draws a lattice network from the Z parameters of a network.
+
+    Parameters
+    ----------
+    ZZ : Symbolic Matrix
+        Z parameters.
+    return_components : boolean
+        Returns the components of the symmetric lattice network (Za and Zb).
+
+    Returns
+    -------
+    Za, Zb : Symbolic
+        (Optional) Impedances of of the symmetric lattice network.
+
+    '''
+
+    if ZZ is None    :
+        # sin valores, solo el dibujo
+        Za_lbl = 'Za'
+        Zb_lbl = 'Zb'
+        
+        Za = 1
+        Zb = 1
+        bSymbolic = False
+        
+    else:
+        # calculo los valores de la matriz Z
+        # z11 - z12
+        Za = ZZ[0,0] - ZZ[0,1]
+        Zb = ZZ[0,0] + ZZ[0,1]
+        
+        bSymbolic = isinstance(ZZ[0,0], sp.Basic)
+        
+        if bSymbolic:
+            
+            Za = sp.simplify(Za)
+            Zb = sp.simplify(Zb)
+    
+            Za_lbl = to_latex(Za)
+            Zb_lbl = to_latex(Zb)
+            
+        else:
+                
+            Za_lbl = str_to_latex('{:3.3f}'.format(Za))
+            Zb_lbl = str_to_latex('{:3.3f}'.format(Zb))
+
+    # Dibujo la red Lattice    
+    
+    with Drawing() as d:
+        
+        d.config(fontsize=16, unit=4)
+
+        d = dibujar_puerto_entrada(d, port_name = '' )
+
+        if( bSymbolic and (not Za.is_zero) or (not bSymbolic) and Za != 0 ):
+            d += (Za_d := ResistorIEC().right().label(Za_lbl).dot().idot())
+        else:
+            d += (Za_d := Line().right().dot())
+
+        d.push()
+        
+        d += Gap().down().label('')
+
+        d += (line_down := Line(ls='dotted').left().dot().idot())
+
+        cross_line_vec = line_down.end - Za_d.end
+
+        d += Line(ls='dotted').endpoints(Za_d.end, Za_d.end + 0.25*cross_line_vec )
+
+        d += Line(ls='dotted').endpoints(Za_d.end + 0.6*cross_line_vec, line_down.end )
+
+        if( bSymbolic and (not Zb.is_zero) or (not bSymbolic) and Zb != 0 ):
+            d += (Zb_d := ResistorIEC().label(Zb_lbl).endpoints(Za_d.start, line_down.start).dot())
+        else:
+            d += (Zb_d := Line().endpoints(Za_d.start, line_down.start).dot())
+            
+        d.pop()
+
+        d = dibujar_puerto_salida(d, port_name = '' )
+
+
+    if(return_components):
+        return([Za, Zb])
+
+
 
 def dibujar_cauer_RC_RL(ki = None, y_exc = None, z_exc = None):
     '''
     Description
     -----------
     Draws a parallel non-disipative admitance following Foster synthesis method.
 
@@ -830,14 +921,15 @@
     d.push()
     d += Gap().down().label( '' )
     d += Line().left()
     d.pop()
 
     return(d)
 
+
 def dibujar_espacio_derivacion(d):
     '''
     Convierte una matriz de parámetros scattering (S) simbólica 
     al modelo de parámetros transferencia de scattering (Ts).
 
     Parameters
     ----------
```

### Comparing `pytc2-0.0.2/src/pytc2/ej5.13 schaumann.py` & `pytc2-0.0.3/src/pytc2/ej5.13 schaumann.py`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.2/src/pytc2/general.py` & `pytc2-0.0.3/src/pytc2/general.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Further modifications were added for didactic purposes
 by Mariano Llamedo llamedom _at_ frba_utn_edu_ar
 
 @author: marianux
 """
 
 import sympy as sp
+import numpy as np
 
 from IPython.display import display, Math, Markdown
 
 ##########################################
 #%% Variables para el análisis simbólico #
 ##########################################
 
@@ -228,7 +229,55 @@
         Cn = Cn_p
         
     else:
         Cn = 1
             
     return(sp.simplify(sp.expand(Cn)))
 
+
+
+'''
+  ################################################
+ ## Bloque de funciones para parametros imagen ##
+################################################
+'''
+
+
+def db2nepper(at_en_db):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
+    
+    return( at_en_db/(20*np.log10(np.exp(1))) )
+
+def nepper2db(at_en_np):
+    '''
+    Convierte una matriz de parámetros scattering (S) simbólica 
+    al modelo de parámetros transferencia de scattering (Ts).
+
+    Parameters
+    ----------
+    Spar : Symbolic Matrix
+        Matriz de parámetros S.
+
+    Returns
+    -------
+    Ts : Symbolic Matrix
+        Matriz de parámetros de transferencia scattering.
+
+    '''
+    
+    return( at_en_np*(20*np.log10(np.exp(1))) )
+
+
```

### Comparing `pytc2-0.0.2/src/pytc2/ltspice.py` & `pytc2-0.0.3/src/pytc2/ltspice.py`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.2/src/pytc2/remociones.py` & `pytc2-0.0.3/src/pytc2/remociones.py`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.2/src/pytc2/sintesis_dipolo.py` & `pytc2-0.0.3/src/pytc2/sintesis_dipolo.py`

 * *Files identical despite different names*

### Comparing `pytc2-0.0.2/src/pytc2/sistemas_lineales.py` & `pytc2-0.0.3/src/pytc2/sistemas_lineales.py`

 * *Files 1% similar despite different names*

```diff
@@ -1038,80 +1038,72 @@
     None.
 
     Example
     -------
 
     """
 
-    w_nyq = 2*np.pi*fs/2
+    ww_nyq = 2*np.pi*fs/2
     
     if isinstance(myFilter, np.ndarray):
         # SOS section
+        
+        wholeFilter = sos2tf_analog(myFilter)
+
+        # all singularities
+        this_zzpp = np.abs(np.concatenate([wholeFilter.zeros, wholeFilter.poles]))
+        this_zzpp = this_zzpp[this_zzpp > 0]
+
+        # calculate the omega axis according to singularities of the whole filter
+        if digital:
+            ww = np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, ww_nyq, npoints)
+        else:
+            ww = np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints)
+        
         cant_sos = myFilter.shape[0]
         mag = np.empty((npoints, cant_sos+1))
         phase = np.empty_like(mag)
         sos_label = []
         
         for ii in range(cant_sos):
             
             num, den = _one_sos2tf(myFilter[ii,:])
             thisFilter = TransferFunction(num, den)
             
             this_zzpp = np.abs(np.concatenate([thisFilter.zeros, thisFilter.poles]))
             this_zzpp = this_zzpp[this_zzpp > 0]
-            
-            if digital:
-                w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, w_nyq, npoints))
-            else:
-                w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
-            
-            # if digital:
-            #     w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.linspace(10**-2, w_nyq,npoints))
-            # else:
-            #     w, mag[:, ii], phase[:,ii] = thisFilter.bode(np.logspace(-2,2,npoints))
+
+            _, mag[:, ii], phase[:,ii] = thisFilter.bode(ww)
                 
             sos_label += [filter_description + ' - SOS {:d}'.format(ii)]
         
         # whole filter
-        thisFilter = sos2tf_analog(myFilter)
-
-        this_zzpp = np.abs(np.concatenate([thisFilter.zeros, thisFilter.poles]))
-        this_zzpp = this_zzpp[this_zzpp > 0]
-        
-        if digital:
-            w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, w_nyq, npoints))
-        else:
-            w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
+        _, mag[:, cant_sos], phase[:,cant_sos] = wholeFilter.bode(ww)
 
-        # if digital:
-        #     w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.linspace(10**-2, w_nyq, npoints))
-        # else:
-        #     w, mag[:, cant_sos], phase[:,cant_sos] = thisFilter.bode(np.logspace(-2,2,npoints))
-            
         sos_label += [filter_description]
         
         filter_description = sos_label
         
     else:
         # LTI object
         cant_sos = 0
         
         this_zzpp = np.abs(np.concatenate([myFilter.zeros, myFilter.poles]))
         this_zzpp = this_zzpp[this_zzpp > 0]
         
         if digital:
-            w, mag, phase = myFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, w_nyq, npoints))
+            ww, mag, phase = myFilter.bode(np.linspace(np.floor(np.log10(np.min(this_zzpp)))-1, ww_nyq, npoints))
         else:
-            w, mag, phase = myFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
+            ww, mag, phase = myFilter.bode(np.logspace(np.floor(np.log10(np.min(this_zzpp)))-1, np.ceil(np.log10(np.max(this_zzpp))) + 1 ,npoints))
         
         # if myFilter.dt is None:
         #     # filtro analógico normalizado
-        #     w, mag, phase = myFilter.bode(np.logspace(-2,2,npoints))
+        #     ww, mag, phase = myFilter.bode(np.logspace(-2,2,npoints))
         # else:
-        #     w, mag, phase = myFilter.bode(np.linspace(10**-2, w_nyq, npoints))
+        #     ww, mag, phase = myFilter.bode(np.linspace(10**-2, ww_nyq, npoints))
         
         # if isinstance(filter_description, str):
         #     filter_description = [filter_description]
         
 
     if fig_id == 'none':
         fig_hdl, axes_hdl = plt.subplots(2, 1, sharex='col')
@@ -1127,22 +1119,22 @@
 
     (mag_ax_hdl, phase_ax_hdl) = axes_hdl
     
     plt.sca(mag_ax_hdl)
 
     if digital:
         if filter_description is None:
-            aux_hdl = plt.plot(w / w_nyq, mag)    # Bode magnitude plot
+            aux_hdl = plt.plot(ww / ww_nyq, mag)    # Bode magnitude plot
         else:
-            aux_hdl = plt.plot(w / w_nyq, mag, label=filter_description)    # Bode magnitude plot
+            aux_hdl = plt.plot(ww / ww_nyq, mag, label=filter_description)    # Bode magnitude plot
     else:
         if filter_description is None:
-            aux_hdl = plt.semilogx(w, mag)    # Bode magnitude plot
+            aux_hdl = plt.semilogx(ww, mag)    # Bode magnitude plot
         else:
-            aux_hdl = plt.semilogx(w, mag, label=filter_description)    # Bode magnitude plot
+            aux_hdl = plt.semilogx(ww, mag, label=filter_description)    # Bode magnitude plot
     
     if cant_sos > 0:
         # distinguish SOS from total response
         [ aa.set_linestyle(':') for aa in  aux_hdl[:-1]]
         aux_hdl[-1].set_linewidth(2)
     
     plt.grid(True)
@@ -1155,23 +1147,23 @@
         mag_ax_hdl.legend()
 
         
     plt.sca(phase_ax_hdl)
     
     if digital:
         if filter_description is None:
-            aux_hdl = plt.plot(w / w_nyq, np.pi/180*phase)    # Bode phase plot
+            aux_hdl = plt.plot(ww / ww_nyq, np.pi/180*phase)    # Bode phase plot
         else:
-            aux_hdl = plt.plot(w / w_nyq, np.pi/180*phase, label=filter_description)    # Bode phase plot
+            aux_hdl = plt.plot(ww / ww_nyq, np.pi/180*phase, label=filter_description)    # Bode phase plot
             
     else:
         if filter_description is None:
-            aux_hdl = plt.semilogx(w, np.pi/180*phase)    # Bode phase plot
+            aux_hdl = plt.semilogx(ww, np.pi/180*phase)    # Bode phase plot
         else:
-            aux_hdl = plt.semilogx(w, np.pi/180*phase, label=filter_description)    # Bode phase plot
+            aux_hdl = plt.semilogx(ww, np.pi/180*phase, label=filter_description)    # Bode phase plot
     
     
     # Scale axes to fit
     ylim = plt.gca().get_ylim()
 
     # presentar la fase como fracciones de \pi
     ticks = np.linspace(start=np.round(ylim[0]/np.pi)*np.pi, stop=np.round(ylim[1]/np.pi)*np.pi, num = 5, endpoint=True)
@@ -1223,15 +1215,15 @@
     plt.title('Phase response')
     
     if not(filter_description is None):
         # phase_ax_hdl.legend( filter_description )
         phase_ax_hdl.legend()
     
     return fig_id, axes_hdl
-    
+
 def plot_plantilla(filter_type = 'lowpass', fpass = 0.25, ripple = 0.5, fstop = 0.6, attenuation = 40, fs = 2 ):
     """
     
     Parameters
     ----------
     tfa : TYPE
         DESCRIPTION.
@@ -1509,15 +1501,15 @@
                         idx = np.nonzero(np.isreal(p))[0]
                         assert len(idx) > 0
                         p2_idx = idx[np.argmin(np.abs(np.abs(p[idx]) - 1))]
                         p2 = p[p2_idx]
                         # find a real zero to match the added pole
                         assert np.isreal(p2)
                         
-                        if one_z_per_section:
+                        if one_z_per_section or len(z) == 0:
                             # avoid picking double zero (high-pass)
                             # prefer picking band-pass sections (Schaumann 5.3.1)
                             z2 = np.nan
                         else:
                             z2_idx = _nearest_real_complex_idx(z, p2, 'real')
                             z2 = z[z2_idx]
                             assert np.isreal(z2)
@@ -1538,15 +1530,15 @@
 
                     p2 = p1.conj()
                     
                     if np.isreal(z1):  # complex pole, complex zero
 
                         # complex pole, real zero -> possible bandpass
                         
-                        if z1 == 0:
+                        if one_z_per_section or len(z) == 0:
                             # avoid picking double zero (high-pass)
                             # prefer picking band-pass sections (Schaumann 5.3.1)
                             z2 = np.nan
                         else:
                             # z1 over the \sigma axis
                             z2_idx = _nearest_real_complex_idx(z, p1, 'real')
                             z2 = z[z2_idx]
```

### Comparing `pytc2-0.0.2/PKG-INFO` & `pytc2-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytc2
-Version: 0.0.2
+Version: 0.0.3
 Summary: A circuit theory module for students at Universidad Tecnológica Nacional Regional Buen
 License: MIT
 Author: Mariano Llamedo Soria
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

