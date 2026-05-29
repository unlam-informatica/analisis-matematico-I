---
layout: default
title: Práctica — Unidad 1
parent: Unidad 1 — Funciones
permalink: /unidad-1/practica/practica-1
nav_order: 2
---

# Práctica 1 — Funciones

Resolución completa y paso a paso de la **Práctica 1: Funciones**. 

Cada ejercicio incluye el enunciado resumido, el desarrollo con explicaciones, el resultado final en negrita y la comparación con la respuesta oficial. Los gráficos se sugiere verificarlos en **GeoGebra**; aquí se determinan analíticamente dominio, imagen, ceros, asíntotas y transformaciones.

## Ejercicio 1 — Graficar, indicar dominio e imagen

### 1a) Lineal por $P(-3,4)$ y $Q(2,-3)$

La pendiente es

$$m=\dfrac{y_Q-y_P}{x_Q-x_P}=\dfrac{-3-4}{2-(-3)}=\dfrac{-7}{5}=-\dfrac75.$$

Usando la forma punto-pendiente con $Q(2,-3)$:

$$y-(-3)=-\dfrac75(x-2)\ \Rightarrow\ y=-\dfrac75 x+\dfrac{14}{5}-3=-\dfrac75 x+\dfrac{14-15}{5}=-\dfrac75 x-\dfrac15.$$

Una recta no constante tiene dominio e imagen $\mathbb{R}$.

**Resultado: $m(x)=-\dfrac75 x-\dfrac15$, con $D=I=\mathbb{R}$.**

✓ Coincide con la respuesta oficial.

### 1b) Lineal paralela a $2x-3y+9=0$ que corta el eje $x$ en $x=-\tfrac12$

Despejamos la recta dada: $3y=2x+9\Rightarrow y=\dfrac23 x+3$, cuya pendiente es $\dfrac23$. Una paralela tiene la **misma pendiente** $m=\dfrac23$.

Pasa por $\left(-\tfrac12,0\right)$:

$$0=\dfrac23\left(-\dfrac12\right)+b=-\dfrac13+b\ \Rightarrow\ b=\dfrac13.$$

**Resultado: $f(x)=\dfrac23 x+\dfrac13$, con $D=I=\mathbb{R}$.**

✓ Coincide con la respuesta oficial.

### 1c) Cuadrática con vértice $V\left(-\tfrac12,5\right)$ que corta el eje $y$ en $(0,4)$

Forma canónica: $p(x)=a\left(x+\tfrac12\right)^2+5$. Imponemos $p(0)=4$:

$$4=a\left(\tfrac12\right)^2+5=\dfrac{a}{4}+5\ \Rightarrow\ \dfrac{a}{4}=-1\ \Rightarrow\ a=-4.$$

Como $a<0$ la parábola abre hacia abajo, el vértice es máximo, $y_{\max}=5$.

**Resultado: $p(x)=-4\left(x+\tfrac12\right)^2+5$, con $D=\mathbb{R}$, $I=(-\infty,5]$.**

✓ Coincide con la respuesta oficial.

### 1d) Cuadrática con raíces $x_1=-1$, $x_2=\tfrac57$, que pasa por $P\left(1,\tfrac87\right)$

Forma factorizada: $h(x)=a(x+1)\left(x-\tfrac57\right)$. Imponemos $h(1)=\tfrac87$:

$$\dfrac87=a(2)\left(1-\dfrac57\right)=a\cdot2\cdot\dfrac27=\dfrac{4a}{7}\ \Rightarrow\ a=\dfrac{8/7}{4/7}=2.$$

Para la imagen calculamos el vértice. La abscisa es el punto medio de las raíces:

$$x_v=\dfrac{-1+\tfrac57}{2}=\dfrac{-\tfrac27}{2}=-\dfrac17.$$

$$h\left(-\tfrac17\right)=2\left(-\tfrac17+1\right)\left(-\tfrac17-\tfrac57\right)=2\cdot\dfrac67\cdot\left(-\dfrac67\right)=-\dfrac{72}{49}.$$

Como $a>0$, abre hacia arriba: el vértice es mínimo.

**Resultado: $h(x)=2(x+1)\left(x-\tfrac57\right)$, con $D=\mathbb{R}$, $I=\left[-\tfrac{72}{49},+\infty\right)$.**

✓ Coincide con la respuesta oficial.

### 1e) $f(x)=\lvert x\rvert$

El valor absoluto está definido para todo real y nunca es negativo.

**Resultado: $D=\mathbb{R}$, $I=[0,+\infty)$.** Gráfica en "V" con vértice en el origen (verificar en GeoGebra).

✓ Coincide con la respuesta oficial.

### 1f) $g(x)=\sqrt{x}$

La raíz cuadrada real exige radicando $\ge0$, y devuelve valores $\ge0$.

**Resultado: $D=I=[0,+\infty)$.**

✓ Coincide con la respuesta oficial.

### 1g) $h(x)=\dfrac1x$

No está definida en $x=0$; tampoco toma el valor $0$. Asíntotas $x=0$ (vertical) e $y=0$ (horizontal).

**Resultado: $D=I=\mathbb{R}-\{0\}$.**

✓ Coincide con la respuesta oficial.

---

## Ejercicio 2 — Celsius y Fahrenheit

La relación es lineal $F=mC+b$. Datos: $(C,F)=(0,32)$ y $(100,212)$.

### 2a) Función

$$m=\dfrac{212-32}{100-0}=\dfrac{180}{100}=\dfrac95,\qquad b=32\ (\text{ordenada en }C=0).$$

**Resultado: $F(C)=\dfrac95 C+32$.** La terna es $F:\mathbb{R}\to\mathbb{R}$.

✓ Coincide con la respuesta oficial.

### 2b) $-10^\circ$C en °F

$$F(-10)=\dfrac95(-10)+32=-18+32=14.$$

**Resultado: $14^\circ$F.** ✓ Coincide con la respuesta oficial.

### 2c) $0^\circ$F en °C

Despejamos $C=\dfrac59(F-32)$:

$$C=\dfrac59(0-32)=-\dfrac{160}{9}\approx-17{,}8.$$

**Resultado: $\approx-17{,}8^\circ$C.** ✓ Coincide con la respuesta oficial.

### 2d) Cambio $\Delta F$ en $[0,10]$ y $[10,20]$ (en °C)

En una recta, el incremento es la pendiente por el incremento de la variable. Para $\Delta C=10$:

$$\Delta F=m\cdot\Delta C=\dfrac95\cdot10=18.$$

Esto vale igual en $[0,10]$ y en $[10,20]$ (la razón de cambio es constante).

**Resultado: $\Delta F=18^\circ$F en ambos intervalos.** ✓ Coincide con la respuesta oficial.

---

## Ejercicio 3 — Vaciado de un tanque

Recta que parte de $4000$ L en $t=0$ y llega a $0$ L en $t=16$ min.

### 3a) ¿Cuánta agua y en cuánto tiempo?

Del gráfico, el tanque pasa de $4000$ L a $0$ L.

**Resultado: se vaciaron $4000$ L en $16$ min.** ✓ Coincide con la respuesta oficial.

### 3b) Litros por minuto

La pendiente (razón de cambio) es

$$m=\dfrac{0-4000}{16-0}=-250\ \text{L/min}.$$

**Resultado: se vacían $250$ L/min** (el signo negativo indica disminución). ✓ Coincide con la respuesta oficial.

### 3c) ¿Cuándo había $1000$ L?

La fórmula es $V(t)=4000-250t$. Pedimos $V(t)=1000$:

$$1000=4000-250t\ \Rightarrow\ 250t=3000\ \Rightarrow\ t=12.$$

**Resultado: a los $12$ min.** ✓ Coincide con la respuesta oficial.

### Complementos

- **Variable independiente:** el tiempo $t$ (min). **Variable dependiente:** el volumen $V$ (L).
- **Dominio en contexto:** $[0,16]$. **Imagen en contexto:** $[0,4000]$.
- **Fórmula a los $t$ minutos:** $\boxed{V(t)=4000-250t}$.
- **Razón de cambio a los $5$ y $10$ min:** por ser una recta, es constante e igual a $-250$ L/min en cualquier instante.

---

## Ejercicio 4 — Resorte (proporcionalidad directa)

Estiramiento $y$ (pulgadas) en función de la masa $x$. Datos $x=0,\dots,8$ con $y=0;\,0{,}875;\,1{,}721;\,2{,}641;\,3{,}531;\,4{,}391;\,5{,}241;\,6{,}120;\,6{,}992$.

### 4a) Variables

**Independiente:** masa $x$. **Dependiente:** estiramiento $y$.

### 4b) Gráfica

Los puntos se alinean aproximadamente sobre una recta que pasa por el origen (proporcionalidad directa). Se grafica como nube de puntos con su recta de ajuste (verificar en GeoGebra).

### 4c) Constante de proporcionalidad y función

Como $y=kx$ y pasa por el origen, estimamos $k$ con la pendiente media. Tomando el último dato: $k\approx\dfrac{6{,}992}{8}=0{,}874\approx0{,}875$. La regresión lineal da $k\approx0{,}875$.

**Resultado: $f(x)=0{,}875\,x$.**

### 4d) Dominio e imagen en contexto

Las masas van de $0$ a $8$, y $f(0)=0$, $f(8)=7$.

**Resultado: $f:[0,8]\to[0,7]$.** ✓ Coincide con la respuesta oficial.

### 4e) Estiramiento con masa $10$

$$f(10)=0{,}875\cdot10=8{,}75.$$

**Resultado: $8{,}75$ pulgadas.** ✓ Coincide con la respuesta oficial. (Extrapolación fuera del rango medido.)

### 4f) Razón de cambio

Por ser lineal, la razón de cambio es la pendiente.

**Resultado: $0{,}875$ pulgadas por unidad de masa.** ✓ Coincide con la respuesta oficial.

---

## Ejercicio 5* — Canaleta de chapa

Chapa de $12$ cm de ancho; se doblan $x$ cm en cada borde. El fondo mide $12-2x$ y la altura $x$.

### 5a) Área de la sección transversal

$$A(x)=x\,(12-2x)=2x(6-x).$$

Equivalentemente $A(x)=12x-2x^2$.

**Resultado: $A(x)=2x(6-x)$** (la oficial lo expresa como volumen $V(x)=200x(6-x)$ incorporando el largo de $1\text{ m}=100$ cm, ya que $V=100\cdot A=100\cdot2x(6-x)=200x(6-x)$).

### 5b) Dominio

Necesitamos $x>0$ y $12-2x>0\Rightarrow x<6$.

**Resultado: $D=(0,6)$.**

### 5c) y 5d) Máximo

La parábola $A(x)=2x(6-x)$ tiene vértice en el punto medio de las raíces $x=0$ y $x=6$:

$$x_{\max}=\dfrac{0+6}{2}=3.$$

**Resultado: el área (y por tanto la capacidad) es máxima doblando $x=3$ cm.** $A(3)=2\cdot3\cdot3=18\text{ cm}^2$.

✓ Coincide con la respuesta oficial (máximo al doblar $3$ cm).

---

## Ejercicio 6 — Caja sin tapa

Cartón de $24\times32$ cm; se cortan cuadrados de lado $x$ en las esquinas y se doblan los lados. La base queda $(24-2x)\times(32-2x)$ y la altura $x$.

$$V(x)=(24-2x)(32-2x)\,x.$$

Sacando factor común $2$ de cada paréntesis: $V(x)=4(12-x)(16-x)x$.

**Dominio:** $x>0$, $24-2x>0\Rightarrow x<12$ (la restricción más fuerte).

**Resultado: $V(x)=(24-2x)(32-2x)x=4(12-x)(16-x)x$, con $D=(0,12)$.**

Para el máximo se deriva (Unidad 3): $V'(x)=0$ da $x\approx4{,}53$ cm. Se verifica numéricamente/GeoGebra.

✓ Coincide con la respuesta oficial.

---

## Ejercicio 7 — Fórmula y dominio

### 7a)* Área de rectángulo de perímetro $20$ m, en función de un lado $x$

Si un lado es $x$, el otro es $\dfrac{20-2x}{2}=10-x$.

$$A(x)=x(10-x).$$

Para que ambos lados sean positivos: $0<x<10$.

**Resultado: $A(x)=x(10-x)$, $D=(0,10)$.** ✓ Coincide con la respuesta oficial.

### 7b) Perímetro de rectángulo de área $16$ m², en función de un lado $x$

El otro lado es $\dfrac{16}{x}$. El perímetro es

$$P(x)=2x+2\cdot\dfrac{16}{x}=2x+\dfrac{32}{x}.$$

Con $x>0$.

**Resultado: $P(x)=2x+\dfrac{32}{x}$, $D=\mathbb{R}^+$.** ✓ Coincide con la respuesta oficial.

### 7c) Área de triángulo equilátero en función del lado $l$

La altura es $h=\dfrac{\sqrt3}{2}l$, entonces

$$A(l)=\dfrac{l\cdot h}{2}=\dfrac{l}{2}\cdot\dfrac{\sqrt3}{2}l=\dfrac{\sqrt3}{4}l^2.$$

**Resultado: $A(l)=\dfrac{\sqrt3}{4}l^2$, $D=\mathbb{R}^+$.** ✓ Coincide con la respuesta oficial.

---

## Ejercicio 8 — $C(t)=-t^2+6t$ (concentración mg/l)

### 8a) Dominio e imagen en contexto, gráfica

Las raíces son $t=0$ y $t=6$ (la concentración es $0$ al inicio y al final). El vértice está en $t=3$:

$$C(3)=-9+18=9.$$

**Resultado: $C:[0,6]\to[0,9]$.** Parábola hacia abajo con máximo $9$ mg/l a las $3$ h (GeoGebra).

✓ Coincide con la respuesta oficial.

### 8b) ¿Cuándo $C>8$?

$$-t^2+6t>8\ \Rightarrow\ t^2-6t+8<0\ \Rightarrow\ (t-2)(t-4)<0.$$

El producto es negativo entre las raíces.

**Resultado: $t\in(2,4)$.** ✓ Coincide con la respuesta oficial.

### 8c) Razón de cambio media

$$\text{RCM}[a,b]=\dfrac{C(b)-C(a)}{b-a}.$$

En $[1,2]$: $C(1)=5$, $C(2)=8$, $\dfrac{8-5}{1}=3$.

En $[1;1{,}5]$: $C(1{,}5)=-2{,}25+9=6{,}75$, $\dfrac{6{,}75-5}{0{,}5}=\dfrac{1{,}75}{0{,}5}=3{,}5$.

**Resultado: $3$ mg/l por hora en $[1,2]$; $3{,}5$ mg/l por hora en $[1;1{,}5]$.** ✓ Coincide con la respuesta oficial.

---

## Ejercicio 9 — Dominio natural

### 9a) $y=-\sqrt2\,x^4-3x+\tfrac17 x^2-2$

Es un polinomio. **Resultado: $D=\mathbb{R}$.** ✓ Coincide.

### 9b) $y=(x^2-3)^{-4}=\dfrac{1}{(x^2-3)^4}$

Se anula el denominador cuando $x^2=3\Rightarrow x=\pm\sqrt3$.

**Resultado: $D=\mathbb{R}-\{\sqrt3,-\sqrt3\}$.** ✓ Coincide.

### 9c) $y=\dfrac{x^5-2x+5}{x^2-3x+2}$

Denominador $x^2-3x+2=(x-1)(x-2)=0$ en $x=1,2$.

**Resultado: $D=\mathbb{R}-\{1,2\}$.** ✓ Coincide.

### 9d) $y=\dfrac{\lvert x-1\rvert}{x+2}$

Denominador $=0$ en $x=-2$ (el numerador existe para todo $x$).

**Resultado: $D=\mathbb{R}-\{-2\}$.** ✓ Coincide.

### 9e) $y=\sqrt{x+2}$

Radicando $\ge0\Rightarrow x\ge-2$.

**Resultado: $D=[-2,+\infty)$.** ✓ Coincide.

### 9f) $y=\sqrt{\dfrac{1}{2x+1}-2}$

Necesitamos $\dfrac{1}{2x+1}-2\ge0\Rightarrow\dfrac{1}{2x+1}\ge2\Rightarrow\dfrac{1-2(2x+1)}{2x+1}\ge0\Rightarrow\dfrac{-4x-1}{2x+1}\ge0.$

Multiplicando por $-1$ (invierte el sentido): $\dfrac{4x+1}{2x+1}\le0$. Esto ocurre cuando numerador y denominador tienen signos opuestos: $x\in\left(-\tfrac12,-\tfrac14\right]$ (se incluye $-\tfrac14$ porque allí el numerador $4x+1=0$; se excluye $-\tfrac12$ por anular el denominador).

**Resultado: $D=\left(-\tfrac12,-\tfrac14\right]$.** ✓ Coincide.

### 9g) $y=\dfrac{2x}{\sqrt{x^2-4}}$

Radicando **estricto** $>0$ (está en el denominador): $x^2-4>0\Rightarrow x<-2$ o $x>2$.

**Resultado: $D=(-\infty,-2)\cup(2,+\infty)$.** ✓ Coincide.

### 9h) $y=\dfrac{x+3}{\lvert 3x+2\rvert}+\dfrac{1}{\sqrt[4]{x+1}}$

Primer término: $\lvert3x+2\rvert\neq0\Rightarrow x\neq-\tfrac23$. Segundo término: raíz cuarta en el denominador exige $x+1>0\Rightarrow x>-1$.

Intersección: $x>-1$ y $x\neq-\tfrac23$.

**Resultado: $D=(-1,+\infty)-\{-\tfrac23\}$.** ✓ Coincide.

### 9i) $y=\dfrac{x^3+5x^2-6x}{x\sqrt[3]{x^2-1}}$

La raíz cúbica existe para todo real, pero está en el denominador junto con $x$. Hay que excluir $x=0$ y $\sqrt[3]{x^2-1}=0\Rightarrow x^2-1=0\Rightarrow x=\pm1$.

**Resultado: $D=\mathbb{R}-\{-1,0,1\}$.** ✓ Coincide.

### 9j)* $y=\sqrt{\dfrac{3x-4}{x+1}}$

Radicando $\ge0$: $\dfrac{3x-4}{x+1}\ge0$. Raíces/exclusiones: numerador $=0$ en $x=\tfrac43$, denominador $=0$ en $x=-1$.

Estudio de signos: el cociente es positivo para $x<-1$ y para $x>\tfrac43$; en $x=\tfrac43$ vale $0$ (se incluye). En $x=-1$ no está definido.

Quedaría $(-\infty,-1)\cup\left[\tfrac43,+\infty\right)$.

> ⚠️ **Discrepancia:** Resultado calculado: $D=(-\infty,-1)\cup\left[\tfrac43,+\infty\right)$. Respuesta del documento: $\left[\tfrac43,+\infty\right)$.

**Causa probable:** en el intervalo $(-\infty,-1)$ el cociente $\dfrac{3x-4}{x+1}$ también es positivo (numerador y denominador ambos negativos), por lo que la raíz existe. La respuesta oficial parece haber omitido esa rama. **El dominio correcto es $D=(-\infty,-1)\cup\left[\tfrac43,+\infty\right)$.**

### 9k)* $y=\dfrac{\sqrt{3x-4}}{\sqrt{x+1}}$

Ahora son **dos raíces separadas**: numerador exige $3x-4\ge0\Rightarrow x\ge\tfrac43$; denominador exige $x+1>0$ (estricto, va abajo) $\Rightarrow x>-1$. La condición más fuerte es $x\ge\tfrac43$.

**Resultado: $D=\left[\tfrac43,+\infty\right)$.**

> ⚠️ **Discrepancia:** Resultado calculado: $D=\left[\tfrac43,+\infty\right)$. Respuesta del documento: $(-\infty,-1)\cup\left[\tfrac43,+\infty\right)$.

**Causa probable:** aquí **no** es válido el intervalo $(-\infty,-1)$, porque para $x<-1$ se tendría $3x-4<0$ y $\sqrt{3x-4}$ no existe en $\mathbb{R}$. La respuesta oficial confundió este caso con el del inciso j). Notar la diferencia clave: $\sqrt{\tfrac{a}{b}}$ (inciso j) **no** es lo mismo que $\tfrac{\sqrt a}{\sqrt b}$ (inciso k) en cuanto a dominio. **El dominio correcto de k) es $\left[\tfrac43,+\infty\right)$.**

### 9l) $f(x)=\sqrt{\dfrac{x-1}{x-3}}\ (x<4)$; $\ln(5-x)\ (x\ge4)$

**Tramo $x<4$:** $\dfrac{x-1}{x-3}\ge0$ con exclusión $x=3$. El cociente es $\ge0$ para $x\le1$ o $x>3$. Intersecando con $x<4$: $(-\infty,1]\cup(3,4)$.
**Tramo $x\ge4$:** $\ln(5-x)$ exige $5-x>0\Rightarrow x<5$. Intersecando con $x\ge4$: $[4,5)$.

Unión: $(-\infty,1]\cup(3,4)\cup[4,5)=(-\infty,1]\cup(3,5)$, y como $4$ está incluido queda $(-\infty,1]\cup(3,5)-\{3\}$... revisando: $(3,4)\cup[4,5)=(3,5)$. Total: $(-\infty,1]\cup(3,5)$.

> ⚠️ **Discrepancia:** Resultado calculado: $D=(-\infty,1]\cup(3,5)$. Respuesta del documento: $[1,5)-\{3\}$.

**Causa probable:** la respuesta oficial parece resolver el primer tramo como si fuera $\dfrac{x-1}{x-3}\ge0$ tomando solo el intervalo entre las raíces invertido o limitando a $[1,5)$. Con el estudio de signos correcto del cociente, para $x<1$ ambos factores son negativos ($x-1<0$, $x-3<0$) y el cociente es positivo, de modo que la raíz existe; por lo tanto todo $(-\infty,1]$ pertenece al dominio. **El dominio correcto es $D=(-\infty,1]\cup(3,5)$.**

### 9m) $f(x)=\sqrt{4-x^2}\ (x\le2)$; $\dfrac{1}{x-1}\ (x>2)$

**Tramo $x\le2$:** $4-x^2\ge0\Rightarrow-2\le x\le2$. Con $x\le2$: $[-2,2]$.
**Tramo $x>2$:** $\dfrac{1}{x-1}$ definida salvo $x=1$, pero $1\notin(2,+\infty)$, así que vale todo $(2,+\infty)$.

Unión: $[-2,2]\cup(2,+\infty)=[-2,+\infty)$.

**Resultado: $D=[-2,+\infty)$.** ✓ Coincide con la respuesta oficial.

### 9n) $f(x)=\sqrt{x^2-9}\ (x<4)$; $\dfrac{1}{x^2-1}\ (x\ge4)$

**Tramo $x<4$:** $x^2-9\ge0\Rightarrow x\le-3$ o $x\ge3$. Con $x<4$: $(-\infty,-3]\cup[3,4)$.
**Tramo $x\ge4$:** $\dfrac{1}{x^2-1}$ definida salvo $x=\pm1$, que no están en $[4,+\infty)$: vale todo $[4,+\infty)$.

Unión: $(-\infty,-3]\cup[3,4)\cup[4,+\infty)=(-\infty,-3]\cup[3,+\infty)$.

**Resultado: $D=(-\infty,-3]\cup[3,+\infty)$.** ✓ Coincide con la respuesta oficial.

### 9ñ) $f(x)=\sqrt{\dfrac{1}{5-x}}\ (x<3)$; $\sqrt{\ln(x-2)}\ (x\ge3)$

**Tramo $x<3$:** $\dfrac{1}{5-x}\ge0\Rightarrow5-x>0\Rightarrow x<5$ (con $5-x\neq0$). Con $x<3$: todo $(-\infty,3)$.
**Tramo $x\ge3$:** $\sqrt{\ln(x-2)}$ exige $\ln(x-2)\ge0\Rightarrow x-2\ge1\Rightarrow x\ge3$ (y $x-2>0$). Con $x\ge3$: todo $[3,+\infty)$.

Unión: $(-\infty,3)\cup[3,+\infty)=\mathbb{R}$.

**Resultado: $D=\mathbb{R}$.** ✓ Coincide con la respuesta oficial.

---

## Ejercicio 10 — Dominio, imagen, intersecciones, positividad/negatividad

### 10a) $f(x)=x^2+2x-8$

Raíces: $x^2+2x-8=(x+4)(x-2)=0\Rightarrow x=-4,2$. Vértice en $x=-1$, $f(-1)=1-2-8=-9$.

- $D=\mathbb{R}$, $I=[-9,+\infty)$.
- Intersecciones: $(0,-8)$, $(-4,0)$, $(2,0)$.
- $I^+=(-\infty,-4)\cup(2,+\infty)$, $I^-=(-4,2)$.

✓ Coincide con la respuesta oficial.

### 10b) $f(x)=\lvert x-2\rvert$

Gráfica en "V" con vértice $(2,0)$.

- $D=\mathbb{R}$, $I=[0,+\infty)$.
- Intersecciones: $(0,2)$ y $(2,0)$.
- $I^+=\mathbb{R}-\{2\}$ (es positiva en todo punto salvo donde se anula). $I^-$ no tiene (el valor absoluto nunca es negativo).

✓ Coincide con la respuesta oficial.

### 10c) $f(x)=\dfrac{x}{x-2}$

- $D=\mathbb{R}-\{2\}$. AV $x=2$, AH $y=1$, por lo que $I=\mathbb{R}-\{1\}$.
- Intersección: $(0,0)$.
- $I^+=(-\infty,0)\cup(2,+\infty)$, $I^-=(0,2)$.

✓ Coincide con la respuesta oficial.

### 10d)* $g(x)=\dfrac{-2x+3}{x+4}$

- $D=\mathbb{R}-\{-4\}$. AV $x=-4$. AH: cociente de grados iguales, $y=\dfrac{-2}{1}=-2$, entonces $I=\mathbb{R}-\{-2\}$.
- Intersecciones: $g(x)=0\Rightarrow -2x+3=0\Rightarrow x=\tfrac32$, punto $\left(\tfrac32,0\right)$; con eje $y$: $g(0)=\tfrac34$, punto $\left(0,\tfrac34\right)$.
- $I^+=\left(-4,\tfrac32\right)$, $I^-=(-\infty,-4)\cup\left(\tfrac32,+\infty\right)$.

✓ Coincide con la respuesta oficial.

### 10e) $f(x)=\sqrt{x-2}$

- $D=[2,+\infty)$, $I=[0,+\infty)$.
- Intersección: $(2,0)$.
- $I^+=(2,+\infty)$, $I^-$ no tiene.

✓ Coincide con la respuesta oficial.

### 10f) $f(x)=\ln(x+1)$

- $D=(-1,+\infty)$ (pues $x+1>0$), $I=\mathbb{R}$. AV $x=-1$.
- Intersección: $\ln(x+1)=0\Rightarrow x+1=1\Rightarrow x=0$, punto $(0,0)$.
- $I^+=(0,+\infty)$, $I^-=(-1,0)$.

✓ Coincide con la respuesta oficial.

### 10g) $f(x)=2^{x+1}$

- $D=\mathbb{R}$, $I=(0,+\infty)$. AH $y=0$.
- Intersección con eje $y$: $f(0)=2^1=2$, punto $(0,2)$. No corta el eje $x$.
- $I^+=\mathbb{R}$ (la exponencial es siempre positiva), $I^-$ no tiene.

✓ Coincide con la respuesta oficial.

---

## Ejercicio 11 — Funciones por tramos

### 11a) $f(x)=x+2\,(x\le-1);\ -x\,(-1<x\le1);\ 3x-4\,(1<x\le3);\ 2\,(x>3)$

- **Dominio:** los tramos cubren todo, $D=\mathbb{R}$.
- **Imagen:** tramo 1 ($x\le-1$): $x+2\le1$, da $(-\infty,1]$. Tramo 2 ($-1<x\le1$): $-x\in[-1,1)$. Tramo 3 ($1<x\le3$): $3x-4\in(-1,5]$. Tramo 4: $\{2\}$. La unión es $(-\infty,5]$.
- **Ceros:** $x+2=0\Rightarrow x=-2$ (válido); $-x=0\Rightarrow x=0$ (válido); $3x-4=0\Rightarrow x=\tfrac43$ (válido, está en $(1,3]$); el tramo $=2$ no se anula. Ceros $\{-2,0,\tfrac43\}$.

**Resultado: $D=\mathbb{R}$, $I=(-\infty,5]$, ceros $\{-2,0,\tfrac43\}$.** ✓ Coincide.

### 11b)* $f(x)=\dfrac{x^2-6x+9}{x-3}\ (x\neq3);\ 4\ (x=3)$

Simplificamos: $\dfrac{(x-3)^2}{x-3}=x-3$ para $x\neq3$. Es la recta $y=x-3$ con un punto desplazado: en $x=3$ vale $4$ en vez de $0$.

- $D=\mathbb{R}$.
- **Imagen:** la recta $x-3$ cubre todo $\mathbb{R}$ salvo el valor en $x=3$ (que sería $0$, pero queda excluido porque allí $f=4$). El valor $4$ ya lo aporta la recta en $x=7$. Entonces $I=\mathbb{R}-\{0\}$.
- **Ceros:** $x-3=0\Rightarrow x=3$, pero en $x=3$ la función vale $4\neq0$. No hay ceros.

**Resultado: $D=\mathbb{R}$, $I=\mathbb{R}-\{0\}$, sin ceros.** ✓ Coincide.

### 11c) $f(x)=\lvert x+\tfrac12\rvert\,(x\le2);\ \lvert x-4\rvert\,(x>2)$

- $D=\mathbb{R}$.
- **Imagen:** tramo 1 ($x\le2$): $\lvert x+\tfrac12\rvert$ tiene mínimo $0$ en $x=-\tfrac12$ y crece; en $x=2$ vale $2{,}5$, da $[0,2{,}5]$. Tramo 2 ($x>2$): $\lvert x-4\rvert$, mínimo $0$ en $x=4$; en $x\to2^+$ vale $2$ y crece sin cota, da $[0,+\infty)$. Unión: $[0,+\infty)$.
- **Ceros:** $\lvert x+\tfrac12\rvert=0\Rightarrow x=-\tfrac12$ (válido, $\le2$); $\lvert x-4\rvert=0\Rightarrow x=4$ (válido, $>2$). Ceros $\{-\tfrac12,4\}$.

**Resultado: $D=\mathbb{R}$, $I=[0,+\infty)$, ceros $\{-\tfrac12,4\}$.** ✓ Coincide.

### 11d) Interpretado como $f(x)=\sqrt{x+4}\,(x\ge-3);\ x+3\,(-4\le x<-3);\ \sqrt[3]{x}+3\,(x<-4)$

- $D=\mathbb{R}$ (los tramos cubren $x<-4$, $-4\le x<-3$ y $x\ge-3$).
- **Imagen:** tramo $x\ge-3$: $\sqrt{x+4}\ge\sqrt1=1$, da $[1,+\infty)$. Tramo $-4\le x<-3$: $x+3\in[-1,0)$. Tramo $x<-4$: $\sqrt[3]{x}+3$, con $x<-4$ se tiene $\sqrt[3]{x}<\sqrt[3]{-4}\approx-1{,}59$, da $(-\infty,\,3+\sqrt[3]{-4})=(-\infty,\approx1{,}41)$. La unión cubre $\mathbb{R}$.
- **Ceros:** $\sqrt{x+4}=0\Rightarrow x=-4$, pero $-4\notin[-3,+\infty)$: no aplica. $x+3=0\Rightarrow x=-3$, pero $-3\notin[-4,-3)$: no aplica. $\sqrt[3]{x}+3=0\Rightarrow\sqrt[3]{x}=-3\Rightarrow x=-27$ (válido, $<-4$). Cero $\{-27\}$.

**Resultado: $D=\mathbb{R}$, $I=\mathbb{R}$, cero $\{-27\}$.** ✓ Coincide.

---

## Ejercicio 12* — Beneficio (miles de euros)

$B(t)=-t^2+7t\ (0\le t\le5);\ 10\ (5<t\le8)$.

### 12a) Gráfica

Parábola hacia abajo en $[0,5]$ con vértice, luego constante en $10$ desde $t=5$ a $t=8$ (GeoGebra).

### 12b) Mayor beneficio

Vértice de $-t^2+7t$ en $t=\dfrac{7}{2}=3{,}5$: $B(3{,}5)=-12{,}25+24{,}5=12{,}25$. La constante $10$ es menor.

**Resultado: máximo $12{,}25$ (miles de euros) a los $3{,}5$ años.** ✓ Coincide.

### 12c) ¿Cuándo $11{,}250{,}000$ euros = $11{,}25$ miles? (en miles, $B=11{,}25$)

$$-t^2+7t=11{,}25\ \Rightarrow\ t^2-7t+11{,}25=0\ \Rightarrow\ t=\dfrac{7\pm\sqrt{49-45}}{2}=\dfrac{7\pm2}{2}.$$

$t=2{,}5$ o $t=4{,}5$ (ambos en $[0,5]$).

**Resultado: a los $2{,}5$ y $4{,}5$ años.** ✓ Coincide.

### 12d) ¿Qué pasó tras el $5^\circ$ año?

A partir de $t=5$ el beneficio se mantiene constante en $10$.

**Resultado: el beneficio se estabilizó en $10$ (millones/miles según unidad).** ✓ Coincide.

---

## Ejercicio 13 — Paridad

Recordatorio: **par** si $f(-x)=f(x)$ (simétrica respecto al eje $y$); **impar** si $f(-x)=-f(x)$ (simétrica respecto al origen).

| Inciso | Función | $f(-x)$ | Conclusión |
|--------|---------|---------|-----------|
| a) | $x^2-4$ | $x^2-4=f(x)$ | **Par** |
| b) | $x^2+x-2$ | $x^2-x-2\neq\pm f$ | **Ninguna** |
| c) | $\lvert x+1\rvert-\lvert x-1\rvert$ | $\lvert -x+1\rvert-\lvert -x-1\rvert=\lvert x-1\rvert-\lvert x+1\rvert=-f(x)$ | **Impar** |
| d) | $x+1$ | $-x+1\neq\pm f$ | **Ninguna** |
| e) | $\sqrt[3]{x}$ | $-\sqrt[3]{x}=-f(x)$ | **Impar** |
| f)* | $\sqrt[3]{x^2}$ | $\sqrt[3]{x^2}=f(x)$ | **Par** |
| g)* | $x-3x^3$ | $-x+3x^3=-f(x)$ | **Impar** |
| h)* | $\dfrac{1-x}{1+x}$ | $\dfrac{1+x}{1-x}\neq\pm f$ | **Ninguna** |
| i) | $\dfrac{1}{\lvert x\rvert}$ | $\dfrac{1}{\lvert x\rvert}=f(x)$ | **Par** |
| j) | $2^x+2^{-x}$ | $2^{-x}+2^{x}=f(x)$ | **Par** |

**Resultado: Pares $\{a,f,i,j\}$; Impares $\{c,e,g\}$; Ninguna $\{b,d,h\}$.**

✓ Coincide con la respuesta oficial.

---

## Ejercicio 14 — Efecto de transformaciones (con $c\in\mathbb{R}$)

- **a) $y=f(x)+c$:** desplazamiento **vertical**: hacia arriba si $c>0$, hacia abajo si $c<0$. ($\lvert c\rvert$ unidades.)
- **b) $y=f(x-c)$:** desplazamiento **horizontal**: a la derecha si $c>0$, a la izquierda si $c<0$.
- **c) $y=f(cx)$:** **escalado horizontal** (compresión si $\lvert c\rvert>1$, dilatación si $0<\lvert c\rvert<1$); si $c<0$, además refleja respecto al eje $y$.
- **d) $y=c\,f(x)$:** **escalado vertical** (estiramiento si $\lvert c\rvert>1$, compresión si $0<\lvert c\rvert<1$); si $c<0$, además refleja respecto al eje $x$.

---

## Ejercicio 15 — Reflexiones

- **a) $y=-f(x)$:** reflexión respecto al **eje $x$** (lo de arriba va abajo).
- **b) $y=f(-x)$:** reflexión respecto al **eje $y$** (izquierda y derecha se intercambian).

---

## Ejercicio 16 — Graficar con transformaciones; dominio, imagen, ceros

### 16a) $f(x)=\lvert x+2\rvert-\tfrac32$

Base $\lvert x\rvert$: traslación **2 a la izquierda** y **$\tfrac32$ abajo**. Vértice en $\left(-2,-\tfrac32\right)$.

- $D=\mathbb{R}$, $I=\left[-\tfrac32,+\infty\right)$.
- **Ceros:** $\lvert x+2\rvert=\tfrac32\Rightarrow x+2=\pm\tfrac32\Rightarrow x=-\tfrac12$ o $x=-\tfrac72$.

**Resultado: $D=\mathbb{R}$, $I=\left[-\tfrac32,+\infty\right)$, ceros $\{-\tfrac72,-\tfrac12\}$.** ✓ Coincide.

### 16b)* $g(x)=-\sqrt{x-1}+2$

Base $\sqrt{x}$: **1 a la derecha**, **reflexión respecto al eje $x$**, **2 arriba**.

- $D=[1,+\infty)$. Como $-\sqrt{x-1}\le0$, $g(x)\le2$, máximo en $x=1$: $I=(-\infty,2]$.
- **Cero:** $-\sqrt{x-1}+2=0\Rightarrow\sqrt{x-1}=2\Rightarrow x-1=4\Rightarrow x=5$.

**Resultado: $D=[1,+\infty)$, $I=(-\infty,2]$, cero $\{5\}$.** ✓ Coincide.

### 16c) $m(x)=\dfrac{1}{2-x}$

Reescribimos $\dfrac{1}{2-x}=-\dfrac{1}{x-2}$: base $\tfrac1x$, traslación 2 a la derecha y reflexión.

- $D=\mathbb{R}-\{2\}$. AV $x=2$, AH $y=0$, $I=\mathbb{R}-\{0\}$.
- **Ceros:** el numerador es $1\neq0$: **sin ceros**.

**Resultado: $D=\mathbb{R}-\{2\}$, $I=\mathbb{R}-\{0\}$, sin ceros.** ✓ Coincide.

### 16d) $k(x)=(x+4)^3-1$

Base $x^3$: **4 a la izquierda**, **1 abajo**.

- $D=I=\mathbb{R}$ (la cúbica es biyectiva).
- **Cero:** $(x+4)^3=1\Rightarrow x+4=1\Rightarrow x=-3$.

**Resultado: $D=I=\mathbb{R}$, cero $\{-3\}$.** ✓ Coincide.

---

## Ejercicio 17* — ¿Existe $f(x)=C\cdot a^x$ por $(-1,6)$ y $(3,\tfrac38)$?

Planteamos el sistema:

$$C\,a^{-1}=6,\qquad C\,a^{3}=\dfrac38.$$

Dividiendo la segunda por la primera:

$$\dfrac{C a^3}{C a^{-1}}=a^4=\dfrac{3/8}{6}=\dfrac{3}{48}=\dfrac{1}{16}\ \Rightarrow\ a=\left(\dfrac{1}{16}\right)^{1/4}=\dfrac12.$$

Entonces $C=6\,a=6\cdot\tfrac12=3$.

**Resultado: $f(x)=3\left(\dfrac12\right)^x$.** Sí existe. ✓ Coincide con la respuesta oficial.

---

## Ejercicio 18* — Presión atmosférica

$p=760\,e^{-0{,}144h}$. La presión al nivel del mar es $760$; buscamos la mitad, $380$:

$$380=760\,e^{-0{,}144h}\ \Rightarrow\ e^{-0{,}144h}=\dfrac12\ \Rightarrow\ -0{,}144h=\ln\tfrac12\ \Rightarrow\ h=\dfrac{\ln2}{0{,}144}\approx\dfrac{0{,}6931}{0{,}144}\approx4{,}81.$$

**Resultado: $h\approx4{,}81$ km.** ✓ Coincide con la respuesta oficial.

---

## Ejercicio 19* — Población de aves

Inicia con $50$ y se triplica cada $2$ años: $A(t)=50\cdot3^{t/2}$.

### 19a) Tamaño a $6$ años

$$A(6)=50\cdot3^{6/2}=50\cdot3^3=50\cdot27=1350.$$

**Resultado: $1350$ aves.** ✓ Coincide.

### 19b) $P(t)$

**Resultado: $A:[0,+\infty)\to\mathbb{R}$ (en contexto $[50,+\infty)$), $A(t)=50\cdot3^{t/2}$.** ✓ Coincide.

### 19c) Tiempo para $1000$ aves

$$50\cdot3^{t/2}=1000\ \Rightarrow\ 3^{t/2}=20\ \Rightarrow\ \dfrac t2=\log_3 20\ \Rightarrow\ t=2\,\dfrac{\ln20}{\ln3}\approx2\cdot2{,}727\approx5{,}45.$$

$0{,}45$ años $\approx0{,}45\cdot365\approx165$ días.

**Resultado: $\approx5$ años y $165$ días.** ✓ Coincide.

---

## Ejercicio 20 — Transformaciones de $\ln x$ y $e^x$

### 20a) Sobre $\ln x$ (base: $D=(0,+\infty)$, $I=\mathbb{R}$, AV $x=0$, pasa por $(1,0)$)

| Función | Transformación | Dominio |
|---------|----------------|---------|
| $\ln(x-2)$ | 2 a la derecha (AV $x=2$) | $(2,+\infty)$ |
| $\ln x+2$ | 2 arriba | $(0,+\infty)$ |
| $-\ln x$ | reflexión respecto al eje $x$ | $(0,+\infty)$ |
| $\ln(-x)$ | reflexión respecto al eje $y$ | $(-\infty,0)$ |
| $\ln\lvert x\rvert$ | par; suma la rama izquierda reflejada | $\mathbb{R}-\{0\}$ |
| $\lvert\ln x\rvert$ | refleja hacia arriba la parte negativa ($0<x<1$) | $(0,+\infty)$ |

### 20b) Sobre $e^x$ (base: $D=\mathbb{R}$, $I=(0,+\infty)$, AH $y=0$, pasa por $(0,1)$)

| Función | Transformación | Imagen |
|---------|----------------|--------|
| $e^{x+3}$ | 3 a la izquierda | $(0,+\infty)$ |
| $e^x-1$ | 1 abajo (AH $y=-1$) | $(-1,+\infty)$ |
| $-e^x$ | reflexión respecto al eje $x$ | $(-\infty,0)$ |
| $e^{-x}$ | reflexión respecto al eje $y$ | $(0,+\infty)$ |
| $e^{\lvert x\rvert}$ | par; mínimo $1$ en $x=0$ | $[1,+\infty)$ |
| $-e^{2x+3}+1$ | compresión horiz., refl. eje $x$, 1 arriba (AH $y=1$) | $(-\infty,1)$ |

Todas se verifican en GeoGebra.

---

## Ejercicio 21 — Decibeles

$d=10\log\!\left(\dfrac{P}{P_0}\right)$. Despejamos la potencia.

**Concierto ($110$ dB):** $110=10\log\!\left(\tfrac{P_c}{P_0}\right)\Rightarrow\log\!\left(\tfrac{P_c}{P_0}\right)=11\Rightarrow P_c=10^{11}P_0$.

**Tráfico ($90$ dB):** $\log\!\left(\tfrac{P_t}{P_0}\right)=9\Rightarrow P_t=10^{9}P_0$.

Comparación:

$$\dfrac{P_c}{P_t}=\dfrac{10^{11}P_0}{10^{9}P_0}=10^2=100.$$

**Resultado: el concierto tiene $100$ veces más potencia (intensidad) que el tráfico.** ✓ Coincide.

---

## Ejercicio 22* — Efecto sobre $f(x)=\operatorname{sen}x$

Base: $D=\mathbb{R}$, $I=[-1,1]$, período $2\pi$.

- **a) $c\operatorname{sen}x\ (c>0)$:** cambia la **amplitud** a $c$. Imagen $[-c,c]$. Dominio $\mathbb{R}$.
- **b) $\operatorname{sen}(cx)\ (c>0)$:** cambia el **período** a $\dfrac{2\pi}{c}$ (compresión horizontal si $c>1$). Imagen $[-1,1]$.
- **c) $\operatorname{sen}x+c$:** desplazamiento **vertical** $c$. Imagen $[-1+c,\,1+c]$.
- **d) $\operatorname{sen}(x-c)$:** desfase **horizontal** $c$ a la derecha. Imagen $[-1,1]$.

---

## Ejercicio 23 — Transformaciones de $\operatorname{sen}x$

- **a) +3 arriba:** $y=\operatorname{sen}x+3$, imagen $[2,4]$.
- **b) $\pi/2$ a la derecha:** $y=\operatorname{sen}\!\left(x-\tfrac\pi2\right)=-\cos x$, imagen $[-1,1]$.
- **c) período a la mitad:** período $\pi\Rightarrow y=\operatorname{sen}(2x)$, imagen $[-1,1]$.
- **d) amplitud al doble:** $y=2\operatorname{sen}x$, imagen $[-2,2]$.

**Acotación:** como $-1\le\operatorname{sen}x\le1$ para todo $x$, cualquier $y=a\operatorname{sen}(bx)+c$ está **acotada** entre $c-\lvert a\rvert$ y $c+\lvert a\rvert$. La función es periódica y nunca diverge.

---

## Ejercicio 24* — Profundidad sinusoidal

Ciclo cada $4$ h, mínimo $1$ m, máximo $2$ m. Modelo $p(t)=a\operatorname{sen}(bt)+c$.

### 24a) Variables

Independiente: tiempo $t$ (h). Dependiente: profundidad $p$ (m).

### 24b) Parámetros

- **Amplitud:** $a=\dfrac{\max-\min}{2}=\dfrac{2-1}{2}=\dfrac12$.
- **Desplazamiento vertical:** $c=\dfrac{\max+\min}{2}=\dfrac{2+1}{2}=\dfrac32$.
- **Frecuencia:** período $T=4\Rightarrow b=\dfrac{2\pi}{T}=\dfrac{2\pi}{4}=\dfrac\pi2$.

**Resultado: $p(t)=\dfrac12\operatorname{sen}\!\left(\dfrac\pi2 t\right)+\dfrac32$.** ✓ Coincide ($a=\tfrac12,b=\tfrac\pi2,c=\tfrac32$).

### 24c) Dominio e imagen (terna)

**Resultado: $p:[0,+\infty)\to[1,2]$.** ✓ Coincide.

### 24d) Profundidad a $6$ h

$$p(6)=\dfrac12\operatorname{sen}\!\left(\dfrac\pi2\cdot6\right)+\dfrac32=\dfrac12\operatorname{sen}(3\pi)+\dfrac32=\dfrac12\cdot0+\dfrac32=1{,}5.$$

**Resultado: $1{,}5$ m.** ✓ Coincide.

### 24e) Variación entre $3$ y $4$ h

$p(3)=\dfrac12\operatorname{sen}\!\left(\dfrac{3\pi}{2}\right)+\dfrac32=\dfrac12(-1)+\dfrac32=1$.
$p(4)=\dfrac12\operatorname{sen}(2\pi)+\dfrac32=\dfrac32$.
Variación $=1{,}5-1=0{,}5$.

**Resultado: medio metro ($0{,}5$ m).** ✓ Coincide.

---

## Ejercicio 25 — Presión arterial $P(t)=100-20\cos\!\left(\tfrac{8\pi}{3}t\right)$

### 25a) Variables

Independiente: tiempo $t$ (s). Dependiente: presión $P$ (mmHg).

### 25b) Dominio e imagen (se mide $1$ minuto $=60$ s)

El coseno varía en $[-1,1]$, entonces $-20\cos(\cdot)\in[-20,20]$ y $P\in[80,120]$.

**Resultado: $D_P=[0,60]$, $I_P=[80,120]$.** ✓ Coincide.

### 25c) Período

$$T=\dfrac{2\pi}{8\pi/3}=2\pi\cdot\dfrac{3}{8\pi}=\dfrac{6}{8}=\dfrac34\ \text{s}.$$

**Resultado: período $\tfrac34$ s.** ✓ Coincide.

### 25d) Amplitud

**Resultado: $20$.** ✓ Coincide.

### 25e) Pulso (latidos por minuto)

Cada período es un latido. En $60$ s caben $\dfrac{60}{3/4}=80$ latidos.

**Resultado: $80$ LPM.** ✓ Coincide.

---

## Ejercicio 26 — Función inversa

Recordatorio: para invertir, $f$ debe ser **biyectiva** (inyectiva + sobreyectiva) en el dominio/codominio dados; se intercambian dominio e imagen.

### 26a) $f(x)=(x-1)^3+8$

Cúbica trasladada: biyectiva en $\mathbb{R}$. Despejamos:

$$y-8=(x-1)^3\Rightarrow x-1=\sqrt[3]{y-8}\Rightarrow x=\sqrt[3]{y-8}+1.$$

**Resultado: $f^{-1}(x)=\sqrt[3]{x-8}+1$, $\mathbb{R}\to\mathbb{R}$.** ✓ Coincide.

### 26b) $f(x)=e^{2x}+1$

Inyectiva; imagen $(1,+\infty)$.

$$y-1=e^{2x}\Rightarrow 2x=\ln(y-1)\Rightarrow x=\tfrac12\ln(y-1).$$

**Resultado: $f:\mathbb{R}\to(1,+\infty)$, $f^{-1}(x)=\tfrac12\ln(x-1)$.** ✓ Coincide.

### 26c) $f(x)=3-\sqrt{x+5}$

$D=[-5,+\infty)$; como $\sqrt{x+5}\ge0$, $f(x)\le3$, imagen $(-\infty,3]$. Inyectiva (decreciente).

$$y-3=-\sqrt{x+5}\Rightarrow\sqrt{x+5}=3-y\Rightarrow x+5=(3-y)^2\Rightarrow x=(3-y)^2-5.$$

**Resultado: $f:[-5,+\infty)\to(-\infty,3]$, $f^{-1}(x)=(3-x)^2-5$.** ✓ Coincide.

### 26d)* $f(x)=\log_3(2x-4)$

$D:2x-4>0\Rightarrow x>2$, es decir $(2,+\infty)$; imagen $\mathbb{R}$.

$$y=\log_3(2x-4)\Rightarrow 3^y=2x-4\Rightarrow x=\dfrac{3^y+4}{2}.$$

**Resultado: $f:(2,+\infty)\to\mathbb{R}$, $f^{-1}(x)=\dfrac{3^x+4}{2}$.** ✓ Coincide.

### 26e) $f(x)=2x^2-1$

No es inyectiva en $\mathbb{R}$ (parábola). Restringimos a $[0,+\infty)$ (rama derecha): imagen $[-1,+\infty)$.

$$y+1=2x^2\Rightarrow x^2=\dfrac{y+1}{2}\Rightarrow x=\sqrt{\dfrac{y+1}{2}}\ (x\ge0).$$

**Resultado: $f:[0,+\infty)\to[-1,+\infty)$, $f^{-1}(x)=\sqrt{\dfrac{x+1}{2}}$** (la rama $(-\infty,0]$ da $-\sqrt{\tfrac{x+1}{2}}$). ✓ Coincide.

### 26f)* $f(x)=2\operatorname{sen}(3x)$

Se restringe a un intervalo donde $3x\in\left[-\tfrac\pi2,\tfrac\pi2\right]$, es decir $x\in\left[-\tfrac\pi6,\tfrac\pi6\right]$; imagen $[-2,2]$.

$$y=2\operatorname{sen}(3x)\Rightarrow\operatorname{sen}(3x)=\dfrac y2\Rightarrow 3x=\arcsin\!\left(\dfrac y2\right)\Rightarrow x=\dfrac13\arcsin\!\left(\dfrac y2\right).$$

**Resultado: $f:\left[-\tfrac\pi6,\tfrac\pi6\right]\to[-2,2]$, $f^{-1}(x)=\tfrac13\arcsin\!\left(\tfrac x2\right)$.** ✓ Coincide.

### 26g) $f(x)=\dfrac{-x+3}{x-1}$

$D=\mathbb{R}-\{1\}$; AH $y=-1$, imagen $\mathbb{R}-\{-1\}$. Despejamos:

$$y(x-1)=-x+3\Rightarrow yx-y=-x+3\Rightarrow x(y+1)=y+3\Rightarrow x=\dfrac{y+3}{y+1}.$$

**Resultado: $f:\mathbb{R}-\{1\}\to\mathbb{R}-\{-1\}$, $f^{-1}(x)=\dfrac{x+3}{x+1}$.** ✓ Coincide.

---

## Ejercicio 27 — $A(t)=100(1-0{,}9^t)$, $t\in[0,10]$ (mg)

### 27a) Variables, dominio/imagen

Independiente: tiempo $t$. Dependiente: cantidad $A$ (mg). En $t=0$, $A=0$; en $t=10$, $A=100(1-0{,}9^{10})$.

**Resultado: $D=[0,10]$, $I=\left[0,\,100(1-0{,}9^{10})\right]\approx[0;\,65{,}13]$.** ✓ Coincide.

### 27b) ¿Qué es $A^{-1}$? Hallarla

$A^{-1}$ da el **tiempo** en función de la cantidad de mg absorbida.

$$A=100(1-0{,}9^t)\Rightarrow 1-0{,}9^t=\dfrac{A}{100}\Rightarrow 0{,}9^t=1-\dfrac{A}{100}\Rightarrow t=\dfrac{\ln\!\left(1-\tfrac{A}{100}\right)}{\ln0{,}9}.$$

**Resultado: $t(A)=\dfrac{\ln\!\left(1-\tfrac{A}{100}\right)}{\ln0{,}9}$.** ✓ Coincide.

### 27c) Minutos para $50$ mg

$$0{,}9^t=1-\dfrac{50}{100}=0{,}5\Rightarrow t=\dfrac{\ln0{,}5}{\ln0{,}9}\approx\dfrac{-0{,}6931}{-0{,}1054}\approx6{,}58.$$

**Resultado: $\approx6{,}58$ min.** ✓ Coincide.

---

## Ejercicio 28 — Resorte lineal $L(P)$

$7$ cm con $10$ g, $13$ cm con $80$ g.

Pendiente:

$$m=\dfrac{13-7}{80-10}=\dfrac{6}{70}=\dfrac{3}{35}.$$

Ordenada (longitud sin peso): usando $(10,7)$,

$$7=\dfrac{3}{35}\cdot10+b=\dfrac{30}{35}+b=\dfrac67+b\Rightarrow b=7-\dfrac67=\dfrac{49-6}{7}=\dfrac{43}{7}.$$

**Resultado: $L(P)=\dfrac{3}{35}P+\dfrac{43}{7}$.** ✓ Coincide.

### 28a) Longitud sin peso

$L(0)=\dfrac{43}{7}\approx6{,}14$ cm. ✓ Coincide.

### 28b) Variación cada $10$ g

$\Delta L=m\cdot10=\dfrac{3}{35}\cdot10=\dfrac{30}{35}=\dfrac67$ cm. ✓ Coincide.

### 28c) Dominio (se deforma al alargarse $5$ veces la longitud inicial)

Longitud inicial $\dfrac{43}{7}$; el límite es $5\cdot\dfrac{43}{7}=\dfrac{215}{7}$. El peso máximo $P_{\max}$ cumple $L(P_{\max})=\dfrac{215}{7}$:

$$\dfrac{3}{35}P+\dfrac{43}{7}=\dfrac{215}{7}\Rightarrow\dfrac{3}{35}P=\dfrac{172}{7}\Rightarrow P=\dfrac{172}{7}\cdot\dfrac{35}{3}=\dfrac{172\cdot5}{3}=\dfrac{860}{3}.$$

**Resultado: $D=\left[0,\dfrac{860}{3}\right]$, $I=\left[\dfrac{43}{7},\dfrac{215}{7}\right]$.** ✓ Coincide.

### 28d) Inversa y significado

$$L=\dfrac{3}{35}P+\dfrac{43}{7}\Rightarrow P=\dfrac{35}{3}\left(L-\dfrac{43}{7}\right).$$

$L^{-1}$ da el **peso** necesario para una longitud dada.

---

## Ejercicio 29 — Gas (proporcionalidad inversa)

$V$ inversamente proporcional a $P$: $V=\dfrac kP$. Con $P=1,V=30\Rightarrow k=30$.

### 29a) Fórmula, dominio/imagen

Datos $P\in[1,12]$; $V(1)=30$, $V(12)=\dfrac{30}{12}=2{,}5$.

**Resultado: $V:[1,12]\to[2{,}5;\,30]$, $V(P)=\dfrac{30}{P}$.** ✓ Coincide.

### 29b) Volumen a $11$ atm

$$V(11)=\dfrac{30}{11}\approx2{,}72\ \text{litros}.$$

**Resultado: $\approx2{,}72$ litros.** ✓ Coincide.

### 29c) ¿$P$ en función de $V$?

$$P=\dfrac{30}{V}.$$

**Resultado: $P:[2{,}5;\,30]\to[1,12]$, $P=\dfrac{30}{V}$.** ✓ Coincide.

---

## Ejercicio 30 — Masa de sustancia

$t=0,1,2,5\to$ masa $25,75,225,6075$. Cada paso multiplica por $3$ ($75/25=3$, $225/75=3$, y $6075/225=27=3^3$ ✓). Crecimiento exponencial $M(t)=25\cdot3^t$.

### 30a) Masa inicial

$M(0)=25$ g. ✓ Coincide.

### 30b) $M(t)$ (experimento $8$ h)

$M(8)=25\cdot3^8=25\cdot6561=164025$.

**Resultado: $M:[0,8]\to[25,\,164025]$, $M(t)=25\cdot3^t$.** ✓ Coincide.

### 30c) Inversa y significado

$$M=25\cdot3^t\Rightarrow 3^t=\dfrac{M}{25}\Rightarrow t=\log_3\!\left(\dfrac{M}{25}\right).$$

$M^{-1}$ da el **tiempo** necesario para alcanzar una masa dada. **Resultado: $t=\log_3\!\left(\tfrac{M}{25}\right)$.** ✓ Coincide.

---

## Ejercicio 31* — Marea $y=5+4{,}9\cos\!\left(\tfrac\pi6 t\right)$

### 31a) Gráfica en $[0,24]$ y terna

Coseno de amplitud $4{,}9$ centrado en $5$; período $\dfrac{2\pi}{\pi/6}=12$ h.

**Resultado: $y:[0,24]\to[0{,}1;\,9{,}9]$** (mín $5-4{,}9=0{,}1$, máx $5+4{,}9=9{,}9$). Verificar en GeoGebra.

### 31b) Nivel en marea alta

Cuando $\cos=1$ (en $t=0,12,24$): $y=5+4{,}9=9{,}9$.

**Resultado: $9{,}9$ pies.** ✓ Coincide.

### 31c) Marea baja

Cuando $\cos=-1$: $\dfrac\pi6 t=\pi\Rightarrow t=6$ (y $t=18$). $y=5-4{,}9=0{,}1$.

**Resultado: a las $6$ h y $18$ h, $0{,}1$ pies.** ✓ Coincide.

### 31d) Período y amplitud

**Resultado: período $12$ h, amplitud $4{,}9$ pies.** ✓ Coincide.

### 31e) Inversa restringida a las primeras $6$ h

En $[0,6]$ el coseno es inyectivo (decreciente). Despejamos:

$$y-5=4{,}9\cos\!\left(\dfrac\pi6 t\right)\Rightarrow\cos\!\left(\dfrac\pi6 t\right)=\dfrac{y-5}{4{,}9}\Rightarrow\dfrac\pi6 t=\arccos\!\left(\dfrac{y-5}{4{,}9}\right)\Rightarrow t=\dfrac6\pi\arccos\!\left(\dfrac{y-5}{4{,}9}\right).$$

**Resultado: $t=\dfrac6\pi\arccos\!\left(\dfrac{h-5}{4{,}9}\right)$.** ✓ Coincide.

---

## Ejercicio 32 — Verdadero o Falso (justificar)

**a) Si $f(x)=mx+b$, entonces $\Delta y=m$ en intervalos de longitud $1$.** En una recta $\Delta y=m\,\Delta x$; con $\Delta x=1$, $\Delta y=m$. **Verdadero.** ✓

**b) Si la imagen consta de un solo número, su dominio también.** Una función constante $f(x)=k$ tiene imagen $\{k\}$ pero dominio $\mathbb{R}$. **Falso.** ✓

**c) Si $f$ y $g$ tienen el mismo dominio, $f/g$ también.** Contraejemplo: $f=x+1$, $g=x-2$ (ambas con $D=\mathbb{R}$), pero $\dfrac fg$ excluye $x=2$, $D=\mathbb{R}-\{2\}$. **Falso.** ✓

**d) Si $\cos s=\cos t$ entonces $s=t$.** El coseno no es inyectivo: $\cos0=\cos2\pi=1$ pero $0\neq2\pi$. **Falso.** ✓

**e) Si $f$ es biyectiva, entonces $f^{-1}(x)=\tfrac{1}{f(x)}$.** Confunde inversa con recíproco. Contraejemplo: $f(x)=2x$, $f^{-1}(x)=\tfrac x2\neq\tfrac{1}{2x}$. **Falso.** ✓

**f) Las rectas $ax+y=c$ y $ax-y=c$ son perpendiculares.** Pendientes $-a$ y $a$; son perpendiculares solo si $(-a)(a)=-1\Rightarrow a^2=1\Rightarrow a=\pm1$. No en general. **Falso.** ✓

**g) Si $x>0$, $(\ln x)^6=6\ln x$.** $(\ln x)^6$ es la potencia sexta; $6\ln x=\ln x^6$. Son distintas (p. ej. $x=e$: $1\neq6$). **Falso.** ✓

**h) Si $f(a)=f(b)\Rightarrow a=b$.** Eso solo vale para funciones inyectivas. Contraejemplo: $f(x)=x^2$, $f(-2)=f(2)$ pero $-2\neq2$. **Falso.** ✓

**i) Si $f$ es función, $f(ax)=af(x)$.** Solo vale para lineales homogéneas. Contraejemplo: $f=\operatorname{sen}$, $\operatorname{sen}(2x)\neq2\operatorname{sen}x$. **Falso.** ✓

**j) $f(x)=\sqrt{\dfrac{x+3}{2-5x}}$ y $g(x)=\dfrac{\sqrt{x+3}}{\sqrt{2-5x}}$ son iguales.** Estudiemos dominios. Para $f$: $\dfrac{x+3}{2-5x}\ge0\Rightarrow x\in\left[-3,\tfrac25\right)$. Para $g$: $x+3\ge0$ y $2-5x>0\Rightarrow x\ge-3$ y $x<\tfrac25\Rightarrow\left[-3,\tfrac25\right)$. Coinciden los dominios y, donde existen, los valores son iguales (ambos factores no negativos). **Verdadero.** ✓

**k) $f(x)=4+\ln(3-x)$ surge de $\ln x$ por: traslación 3 a la izquierda, reflexión respecto al eje $y$, traslación 4 arriba.** $\ln(3-x)=\ln(-(x-3))$: reflexión en $y$ y traslación; sumar $4$ desplaza arriba. La descripción es válida. **Verdadero.** ✓

**l) Toda función inyectiva es sobreyectiva.** Contraejemplo: $f:\mathbb{R}\to\mathbb{R}$, $f(x)=e^x$ es inyectiva pero su imagen es $(0,+\infty)\neq\mathbb{R}$. **Falso.** ✓

**Resultado: Verdaderas $\{a,j,k\}$; Falsas $\{b,c,d,e,f,g,h,i,l\}$.** ✓ Coincide con la respuesta oficial.

---

## Ejercicios adicionales

### Adicional 1 — Paridad (V/F)

**a) $h(x)=\dfrac{2x}{x^2+5}$ "no tiene paridad".**

$$h(-x)=\dfrac{2(-x)}{(-x)^2+5}=\dfrac{-2x}{x^2+5}=-h(x).$$

La función es **impar** (sí tiene paridad).

> ⚠️ **Discrepancia:** Resultado calculado: $h$ es **impar** ($h(-x)=-h(x)$). Respuesta del documento: "no tiene paridad".
>
> **Causa probable:** el enunciado afirma erróneamente que no tiene paridad. Como cumple $h(-x)=-h(x)$, es impar. La afirmación del documento es **falsa**.

**b) $h(x)=\dfrac{3x^2}{x-5}$ "es par".**

$$h(-x)=\dfrac{3x^2}{-x-5}=-\dfrac{3x^2}{x+5}.$$

Esto **no** es igual a $h(x)=\dfrac{3x^2}{x-5}$ ni a $-h(x)$. No tiene paridad (ni par ni impar).

> ⚠️ **Discrepancia:** Resultado calculado: $h$ **no es par** (no tiene paridad). Respuesta del documento: "es par".
>
> **Causa probable:** aunque el numerador $3x^2$ es par, el denominador $x-5$ rompe toda simetría; además el dominio $\mathbb{R}-\{5\}$ no es simétrico respecto al origen, condición necesaria para tener paridad. La afirmación del documento es **falsa**.

**c) $k(x)=\dfrac{x^3}{16-x^2}$ "es impar".**

$$k(-x)=\dfrac{(-x)^3}{16-(-x)^2}=\dfrac{-x^3}{16-x^2}=-k(x).$$

Cociente de impar ($x^3$) sobre par ($16-x^2$) = impar; dominio $(-4,4)\setminus$... simétrico. Es **impar**.

**Resultado: impar.** ✓ Coincide con la respuesta oficial.

### Adicional 2 — $N(t)=227\,e^{0{,}007t}$ (millones, $t$ años post-1980)

**a) Variables y función:** independiente $t$ (años desde 1980), dependiente $N$ (millones). $N(t)=227\,e^{0{,}007t}$, con $N(0)=227$.

**b) Variación 1980–1990 ($t:0\to10$):**

$$N(10)=227\,e^{0{,}07}\approx227\cdot1{,}0725\approx243{,}46.$$

Variación $\approx243{,}46-227=16{,}46$ millones. Razón media $\approx1{,}65$ millones/año.

**c) Inversa:**

$$N=227\,e^{0{,}007t}\Rightarrow e^{0{,}007t}=\dfrac{N}{227}\Rightarrow t=\dfrac{1}{0{,}007}\ln\!\left(\dfrac{N}{227}\right)=\dfrac{\ln(N/227)}{0{,}007}.$$

Da el tiempo (años desde 1980) para una población dada.

**d) ¿Cuándo más del doble de 1980?** $N=2\cdot227=454$:

$$e^{0{,}007t}=2\Rightarrow t=\dfrac{\ln2}{0{,}007}\approx\dfrac{0{,}6931}{0{,}007}\approx99{,}0.$$

**Resultado: a los $\approx99$ años (alrededor del año 2079).**

### Adicional 3 — $L(d)=-10\log_2(d)+120$ (dB)

**a) Si $L=90$, hallar la distancia:**

$$90=-10\log_2(d)+120\Rightarrow-10\log_2 d=-30\Rightarrow\log_2 d=3\Rightarrow d=2^3=8\ \text{m}.$$

Terna en contexto: $L:(0,+\infty)\to\mathbb{R}$ (físicamente acotado por la fuente). **Distancia inicial $=8$ m.**

**b) Distancia para $60$ dB:**

$$60=-10\log_2 d+120\Rightarrow\log_2 d=6\Rightarrow d=2^6=64\ \text{m}.$$

**c) Inversa:**

$$L=-10\log_2 d+120\Rightarrow\log_2 d=\dfrac{120-L}{10}\Rightarrow d=2^{(120-L)/10}.$$

**Resultado: $d(L)=2^{(120-L)/10}$.**

### Adicional 4 — $C(q)=10+3\sqrt q$ (costo)

**a) ¿Costo cero si $q=0$?** $C(0)=10+0=10\neq0$. Hay un **costo fijo de $10$** aunque no se produzca nada. (No, no es cero.)

**b) Razón de cambio media de $100$ a $101$:**

$$\dfrac{C(101)-C(100)}{1}=3\left(\sqrt{101}-\sqrt{100}\right)=3(10{,}0499-10)=3\cdot0{,}0499\approx0{,}1496\approx0{,}15.$$

**c) Costo instantáneo (marginal) en $100$ y comparación.** La derivada (Unidad 3) es $C'(q)=\dfrac{3}{2\sqrt q}$; en $q=100$: $C'(100)=\dfrac{3}{2\cdot10}=0{,}15$.

**Resultado: la razón media ($\approx0{,}15$) coincide casi exactamente con el costo marginal instantáneo ($0{,}15$), porque el intervalo es muy pequeño ($\Delta q=1$).**

### Adicional 5 — (opción múltiple) $V(t)=10\left(1-\tfrac{t}{100}\right)^2$, $0\le t\le100$

Dominio $[0,100]$; $V(0)=10$, $V(100)=0$, decreciente en ese tramo, imagen $[0,10]$.

Inversa: $\dfrac{V}{10}=\left(1-\tfrac{t}{100}\right)^2\Rightarrow1-\tfrac{t}{100}=\sqrt{\dfrac{V}{10}}$ (raíz positiva, pues $1-\tfrac t{100}\ge0$) $\Rightarrow t=100\left(1-\sqrt{\dfrac{V}{10}}\right)$.

$V^{-1}:[0,10]\to[0,100]$. **Resultado: la opción correcta es la c) (terna $V^{-1}:[0,10]\to[0,100]$, $t(V)=100\!\left(1-\sqrt{V/10}\right)$).** ✓ Coincide.

### Adicional 6 — (opción múltiple) $g(x)=\dfrac{x^3}{\sqrt{16-x^2}}$

**Dominio:** $16-x^2>0$ (estricto, en denominador) $\Rightarrow-4<x<4$, es decir $(-4,4)$.

**Paridad:**

$$g(-x)=\dfrac{(-x)^3}{\sqrt{16-x^2}}=\dfrac{-x^3}{\sqrt{16-x^2}}=-g(x).$$

Dominio simétrico y $g(-x)=-g(x)$: **impar**.

**Resultado: impar, dominio $(-4,4)$.** ✓ Coincide.

### Adicional 7 — (opción múltiple) $m(x)=3\operatorname{sen}(5x)$

Por convención se restringe $5x\in\left[-\tfrac\pi2,\tfrac\pi2\right]\Rightarrow x\in\left[-\tfrac{\pi}{10},\tfrac{\pi}{10}\right]$; imagen $[-3,3]$.

$$y=3\operatorname{sen}(5x)\Rightarrow\operatorname{sen}(5x)=\dfrac y3\Rightarrow 5x=\arcsin\!\left(\dfrac y3\right)\Rightarrow x=\dfrac15\arcsin\!\left(\dfrac y3\right).$$

**Resultado: $m^{-1}:[-3,3]\to\left[-\tfrac{\pi}{10},\tfrac{\pi}{10}\right]$, $m^{-1}(x)=\tfrac15\arcsin\!\left(\tfrac x3\right)$.** ✓ Coincide.

### Adicional 8 — (opción múltiple) $U(t)=1000(1-e^{-0{,}05t})$

Para $t\ge0$: $U(0)=0$ y $U\to1000$ cuando $t\to+\infty$ (sin alcanzarlo). Imagen $[0,1000)$.

Inversa:

$$U=1000(1-e^{-0{,}05t})\Rightarrow1-e^{-0{,}05t}=\dfrac{U}{1000}\Rightarrow e^{-0{,}05t}=1-\dfrac{U}{1000}\Rightarrow t=-20\ln\!\left(1-\dfrac{U}{1000}\right).$$

El dominio de la inversa es la imagen de $U$.

**Resultado: $t(U)=-20\ln\!\left(1-\tfrac{U}{1000}\right)$, con dominio $[0,1000)$.** ✓ Coincide.

---

## Resumen de discrepancias

Se detectaron discrepancias con la respuesta oficial en:

1. **9j)** — el dominio oficial omite la rama $(-\infty,-1)$, donde el cociente bajo la raíz también es positivo.
2. **9k)** — el dominio oficial agrega indebidamente $(-\infty,-1)$, imposible porque allí $\sqrt{3x-4}$ no existe. (j y k parecen intercambiados.)
3. **9l)** — el dominio oficial $[1,5)-\{3\}$ omite $(-\infty,1)$, donde la raíz existe.
4. **Adicional 1a)** — el enunciado dice "no tiene paridad", pero la función es **impar**.
5. **Adicional 1b)** — el enunciado dice "es par", pero la función **no tiene paridad**.

En todos los demás ejercicios el resultado **coincide** con la respuesta oficial.
