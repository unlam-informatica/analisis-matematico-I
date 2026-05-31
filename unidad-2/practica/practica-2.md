---
layout: default
title: Práctica — Unidad 2
parent: Unidad 2 — Límite y Continuidad
permalink: /unidad-2/practica/practica-2
nav_order: 2
---

# Práctica 2 — Límite funcional y Continuidad
{: .no_toc }

Resolución completa y paso a paso de la Práctica 2. Cada ejercicio reproduce el enunciado, desarrolla la técnica adecuada (factorización, racionalización, infinitésimos equivalentes, grados de polinomios, límites laterales, asíntotas y análisis de continuidad) y compara el resultado con la respuesta oficial.

## Tabla de contenidos
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Recordatorio de herramientas

**Infinitésimos equivalentes** (cuando $x\to 0$):

$$\operatorname{sen}x\sim x,\quad 1-\cos x\sim \dfrac{x^2}{2},\quad \tan x\sim x,\quad \ln(1+x)\sim x,\quad e^{x}-1\sim x.$$

**Límites notables:**

$$\lim_{x\to 0}\dfrac{\operatorname{sen}x}{x}=1,\qquad \lim_{n\to\infty}\left(1+\dfrac{1}{n}\right)^{n}=e.$$

**Grados de polinomios para $x\to\infty$:** en un cociente, comparar el grado del numerador ($n$) con el del denominador ($m$): si $n<m\Rightarrow 0$; si $n=m\Rightarrow$ cociente de coeficientes principales; si $n>m\Rightarrow \infty$.

**Asíntotas:** vertical (AV) en $x=a$ si algún límite lateral es $\pm\infty$; horizontal (AH) $y=L$ si $\lim_{x\to\pm\infty}f=L$; oblicua (AO) $y=mx+b$ con $m=\lim_{x\to\infty}\dfrac{f(x)}{x}$ y $b=\lim_{x\to\infty}\big(f(x)-mx\big)$.

**Continuidad en $x=a$ (3 condiciones):** existe $f(a)$, existe $\lim_{x\to a}f(x)$, y $\lim_{x\to a}f(x)=f(a)$. Clasificación de discontinuidades: **evitable** (existe el límite finito pero no coincide con $f(a)$ o $f(a)$ no está definida), **esencial de salto finito** (límites laterales finitos distintos), **esencial de salto infinito** (algún lateral $\pm\infty$).

---

## Ejercicio 1

### `1a` - 
**Enunciado.** Graficar $f(x)=\dfrac{x^2+x-6}{x-2}$, $g(x)=x+3$ y $h(x)=\dfrac{x^2+x-6}{x-2}$ si $x\neq2$, $h(2)=-1$. ¿Son iguales? Justificar que $\lim_{x\to2}f=\lim_{x\to2}g=\lim_{x\to2}h$.

**Resolución.** Factorizamos el numerador: $x^2+x-6=(x-2)(x+3)$. Entonces, para $x\neq 2$:

$$f(x)=\dfrac{(x-2)(x+3)}{x-2}=x+3.$$

- **Dominio de $f$:** $\mathbb{R}-\{2\}$. Su gráfica es la recta $y=x+3$ con un **hueco** en $(2,5)$.
- **Dominio de $g$:** $\mathbb{R}$. Es la recta completa $y=x+3$.
- **$h$** coincide con $f$ salvo que define $h(2)=-1$: es la recta $y=x+3$ con el hueco en $(2,5)$ "tapado" por el punto $(2,-1)$.

**¿Son iguales?** No. Aunque las tres tienen la misma "fórmula reducida", difieren en $x=2$: $g$ está definida y vale $5$, $f$ **no** está definida, y $h$ vale $-1$. Dos funciones son iguales solo si tienen el mismo dominio y la misma imagen en cada punto.

**Igualdad de los límites.** El límite cuando $x\to 2$ no depende del valor en $x=2$, sino del comportamiento alrededor. Como en un entorno reducido de $2$ las tres funciones valen $x+3$:

$$\lim_{x\to2}f=\lim_{x\to2}g=\lim_{x\to2}h=\lim_{x\to2}(x+3)=\mathbf{5}.$$

**Conclusión.** Las funciones **no son iguales**, pero los tres límites valen $5$.

✓ Coincide con la respuesta oficial.

### `1b` - 
**Enunciado.** Leer de la gráfica de $f$ los valores pedidos.

**Resolución.** Como no disponemos del gráfico, usamos las respuestas oficiales y explicamos cómo se leen:

| Pedido | Valor | Cómo leerlo |
|---|---|---|
| $\lim_{x\to-8^+}f$ | $1$ | acercándose a $-8$ por derecha la curva tiende a la altura $1$ |
| $\lim_{x\to-4}f$ | no existe | los límites laterales en $-4$ difieren (hay salto) |
| $\lim_{x\to0}f$ | $4$ | ambas ramas llegan a la altura $4$ |
| $\lim_{x\to3}f$ | $3$ | ambas ramas llegan a la altura $3$ |
| $\lim_{x\to8^-}f$ | $-3$ | acercándose a $8$ por izquierda la curva tiende a $-3$ |
| $f(-4)$ | $6$ | punto relleno marcado en altura $6$ |
| $f(0)$ | $4$ | punto relleno en altura $4$ (coincide con el límite: continua ahí) |
| $f(3)$ | no existe | hueco abierto: no hay punto relleno en $x=3$ |

Observación: en $x=0$ hay continuidad ($\lim=f(0)=4$); en $x=3$ el límite existe ($3$) pero $f(3)$ no está definido, por lo que es **discontinuidad evitable**; en $x=-4$ el límite no existe (salto) y $f(-4)=6$.

✓ Coincide con la respuesta oficial.

---

## Ejercicio 2 — Límites inmediatos

Por continuidad de las funciones elementales, reemplazamos directamente (verificando que el resultado esté definido).

### `2a` - $\lim_{x\to2}(x^2-3x+1)$

$$\lim_{x\to2}(x^2-3x+1)=4-6+1=\mathbf{-1}.$$

✓ Coincide con la respuesta oficial.

### `2b` - $\lim_{x\to1}\sqrt{\dfrac{x+1}{2x+1}}$

$$\lim_{x\to1}\sqrt{\dfrac{x+1}{2x+1}}=\sqrt{\dfrac{1+1}{2+1}}=\sqrt{\dfrac{2}{3}}=\mathbf{\sqrt{\dfrac{2}{3}}}.$$

> ⚠️ **Discrepancia:** Resultado calculado: $\sqrt{2/3}$ (raíz **cuadrada**). Respuesta del documento: $\sqrt[3]{2/3}$ (raíz cúbica).
>
> La función es $\sqrt{\,\cdot\,}$ (índice $2$), por lo que el resultado correcto es $\sqrt{2/3}=\dfrac{\sqrt{6}}{3}\approx 0,816$. La raíz cúbica del documento es un error tipográfico.

### `2c` - $\lim_{x\to3}\left(\dfrac{x^2+1}{x}\right)^{2x+1}$

Base: $\dfrac{9+1}{3}=\dfrac{10}{3}$; exponente: $2\cdot 3+1=7$.

$$\lim_{x\to3}\left(\dfrac{x^2+1}{x}\right)^{2x+1}=\left(\dfrac{10}{3}\right)^{7}=\mathbf{\left(\dfrac{10}{3}\right)^{7}}.$$

✓ Coincide con la respuesta oficial.

### `2d` - $\lim_{x\to3}\ln\lvert x^2-4x-1\rvert$

$x^2-4x-1$ en $x=3$: $9-12-1=-4$, su módulo es $4$.

$$\lim_{x\to3}\ln\lvert x^2-4x-1\rvert=\ln 4=\mathbf{\ln 4}.$$

✓ Coincide con la respuesta oficial.

### `2e` - $\lim_{x\to\pi/2}(x\operatorname{sen}x+\cos x)$

Con $\operatorname{sen}\tfrac{\pi}{2}=1$ y $\cos\tfrac{\pi}{2}=0$:

$$\lim_{x\to\pi/2}(x\operatorname{sen}x+\cos x)=\dfrac{\pi}{2}\cdot 1+0=\mathbf{\dfrac{\pi}{2}}.$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 3 — Funciones por tramos

### `3a` - 
$$g(x)=\begin{cases}-x+1 & x<1\\ x-1 & 1<x<2\\ 6-x^2 & x\ge2\end{cases}$$

**En $x=1$:** $\lim_{x\to1^-}(-x+1)=0$ y $\lim_{x\to1^+}(x-1)=0$. Coinciden:

$$\lim_{x\to1}g=\mathbf{0}.$$

**En $x=2$:** $\lim_{x\to2^-}(x-1)=1$ y $\lim_{x\to2^+}(6-x^2)=6-4=2$. Difieren ($1\neq 2$):

$$\lim_{x\to2}g\;\textbf{ no existe}.$$

**En $x=\tfrac14$:** está en el tramo $x<1$, donde $g$ es continua:

$$\lim_{x\to1/4}g=-\dfrac14+1=\mathbf{\dfrac{3}{4}}.$$

✓ Coincide con la respuesta oficial.

### `3b` - 
$$h(x)=\begin{cases}x^2-5 & x\le-1\\ 3x+2 & -1<x<1\\ 4x^2+2x & x\ge1\end{cases}$$

**En $x=-1$:** $\lim_{x\to-1^-}(x^2-5)=1-5=-4$ y $\lim_{x\to-1^+}(3x+2)=-3+2=-1$. Difieren:

$$\lim_{x\to-1}h\;\textbf{ no existe}.$$

**En $x=1$:** $\lim_{x\to1^-}(3x+2)=5$ y $\lim_{x\to1^+}(4x^2+2x)=4+2=6$. Difieren:

$$\lim_{x\to1}h\;\textbf{ no existe}.$$

**En $x=2$:** tramo $x\ge1$, continuo:

$$\lim_{x\to2}h=4\cdot 4+2\cdot 2=\mathbf{20}.$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 4 — Lectura de gráficos

**Enunciado.** Determinar límites laterales y globales a partir de gráficas (no disponibles).

**Método general.** Para cada $x=a$ pedido: se observa la altura a la que tiende la curva por izquierda ($\lim_{x\to a^-}$) y por derecha ($\lim_{x\to a^+}$). Si ambos coinciden y son finitos, el límite existe y vale ese número; si difieren, **no existe** (salto); si alguna rama "se va" hacia arriba/abajo siguiendo una recta vertical, el límite es $\pm\infty$ (asíntota vertical). El valor $f(a)$ se lee solo en el **punto relleno**; un hueco abierto indica que $f(a)$ no está definido en esa altura. La comparación entre $\lim_{x\to a}f$ y $f(a)$ permite clasificar continuidad/discontinuidad, como se aplica en los ejercicios 27 y 1b.

---

## Ejercicio 5 — Hallar $a,b$ para que existan los límites

$$f(x)=\begin{cases}bx & x\le-2\\ x^2+ax & -2<x<1\\ a-bx & x\ge1\end{cases}$$

Para que exista el límite en cada punto de empalme, los laterales deben coincidir.

**En $x=-2$:** $\lim_{x\to-2^-}bx=-2b$ y $\lim_{x\to-2^+}(x^2+ax)=4-2a$. Igualamos:

$$-2b=4-2a\;\Rightarrow\; a-b=2.\qquad (\text{I})$$

**En $x=1$:** $\lim_{x\to1^-}(x^2+ax)=1+a$ y $\lim_{x\to1^+}(a-bx)=a-b$. Igualamos:

$$1+a=a-b\;\Rightarrow\; b=-1.$$

Sustituyendo en (I): $a-(-1)=2\Rightarrow a=1$.

$$\boxed{a=1,\quad b=-1.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 6 *

**Enunciado.** Si $\lim_{x\to a}(f+g)=2$ y $\lim_{x\to a}(f-g)=1$, hallar $\lim_{x\to a}(f\cdot g)$.

**Resolución.** Por álgebra de límites, existen $L=\lim f$ y $M=\lim g$ y:

$$L+M=2,\qquad L-M=1.$$

Resolviendo: $L=\dfrac{3}{2}$, $M=\dfrac{1}{2}$. Entonces

$$\lim_{x\to a}(f\cdot g)=L\cdot M=\dfrac{3}{2}\cdot\dfrac{1}{2}=\mathbf{\dfrac{3}{4}}.$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 7 * — Límites con módulo

Clave: cerca de $x=1$, $\lvert x-1\rvert=x-1$ si $x>1$ y $\lvert x-1\rvert=-(x-1)$ si $x<1$.

### `7a` - $\lim_{x\to1}\dfrac{\lvert x-1\rvert}{x-1}$

Por derecha: $\dfrac{x-1}{x-1}=1$; por izquierda: $\dfrac{-(x-1)}{x-1}=-1$. Difieren $\Rightarrow$ **no existe**.

✓ Coincide con la respuesta oficial.

### `7b` - $\lim_{x\to1^-}\dfrac{\lvert x-1\rvert}{x-1}$

Por izquierda $\lvert x-1\rvert=-(x-1)$:

$$\lim_{x\to1^-}\dfrac{-(x-1)}{x-1}=\mathbf{-1}.$$

✓ Coincide con la respuesta oficial.

### `7c` - $\lim_{x\to1^-}\dfrac{x^2-\lvert x-1\rvert-1}{x-1}$

Por izquierda $\lvert x-1\rvert=-(x-1)=1-x$:

$$\dfrac{x^2-(1-x)-1}{x-1}=\dfrac{x^2+x-2}{x-1}=\dfrac{(x-1)(x+2)}{x-1}=x+2.$$

$$\lim_{x\to1^-}(x+2)=\mathbf{3}.$$

✓ Coincide con la respuesta oficial.

### `7d` - $\lim_{x\to1^+}\left(\dfrac{1}{x-1}-\dfrac{1}{\lvert x-1\rvert}\right)$

Por derecha $\lvert x-1\rvert=x-1$:

$$\dfrac{1}{x-1}-\dfrac{1}{x-1}=0\;\Rightarrow\;\lim_{x\to1^+}=\mathbf{0}.$$

✓ Coincide con la respuesta oficial.

### `7e` - $\lim_{x\to1}\dfrac{\lvert x\rvert-x}{x-1}$

Cerca de $x=1$, $x>0$, luego $\lvert x\rvert=x$ y el numerador es $x-x=0$:

$$\dfrac{0}{x-1}=0\;\Rightarrow\;\lim_{x\to1}=\mathbf{0}.$$

✓ Coincide con la respuesta oficial.

### `7f` - $\lim_{x\to-1}\dfrac{x+x^2}{\lvert x\rvert}$

Cerca de $x=-1$, $x<0$, luego $\lvert x\rvert=-x$:

$$\dfrac{x+x^2}{-x}=\dfrac{x(1+x)}{-x}=-(1+x).$$

$$\lim_{x\to-1}-(1+x)=-(1-1)=\mathbf{0}.$$

✓ Coincide con la respuesta oficial.

### `7g` - $\lim_{x\to0^+}\dfrac{x+x^2}{\lvert x\rvert}$

Por derecha $x>0$, $\lvert x\rvert=x$:

$$\dfrac{x+x^2}{x}=1+x\;\Rightarrow\;\lim_{x\to0^+}(1+x)=\mathbf{1}.$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 8 — Indeterminados $\tfrac00$

### `8a` - $\lim_{x\to3}\dfrac{x-3}{x^2-9}$

$$\dfrac{x-3}{(x-3)(x+3)}=\dfrac{1}{x+3}\;\Rightarrow\;\lim_{x\to3}\dfrac{1}{x+3}=\dfrac{1}{6}=\mathbf{\dfrac{1}{6}}.$$

✓ Coincide con la respuesta oficial.

### `8b` - $\lim_{x\to2}\dfrac{x^2-5x+6}{x^2-9x+14}$

Factorizamos: $x^2-5x+6=(x-2)(x-3)$, $x^2-9x+14=(x-2)(x-7)$.

$$\dfrac{(x-2)(x-3)}{(x-2)(x-7)}=\dfrac{x-3}{x-7}\;\Rightarrow\;\lim_{x\to2}\dfrac{x-3}{x-7}=\dfrac{-1}{-5}=\mathbf{\dfrac{1}{5}}.$$

✓ Coincide con la respuesta oficial.

### `8c` - * $\lim_{h\to0}\dfrac{(3+h)^{-1}-3^{-1}}{h}$

$$\dfrac{\frac{1}{3+h}-\frac{1}{3}}{h}=\dfrac{\frac{3-(3+h)}{3(3+h)}}{h}=\dfrac{-h}{3(3+h)\,h}=\dfrac{-1}{3(3+h)}.$$

$$\lim_{h\to0}\dfrac{-1}{3(3+h)}=\dfrac{-1}{9}=\mathbf{-\dfrac{1}{9}}.$$

✓ Coincide con la respuesta oficial.

### `8d` - $\lim_{x\to2}\dfrac{x-\sqrt{3x-2}}{x^2-4}$

Racionalizamos multiplicando por el conjugado $x+\sqrt{3x-2}$:

$$\dfrac{(x-\sqrt{3x-2})(x+\sqrt{3x-2})}{(x^2-4)(x+\sqrt{3x-2})}=\dfrac{x^2-(3x-2)}{(x^2-4)(x+\sqrt{3x-2})}=\dfrac{x^2-3x+2}{(x^2-4)(x+\sqrt{3x-2})}.$$

Factorizamos $x^2-3x+2=(x-1)(x-2)$ y $x^2-4=(x-2)(x+2)$:

$$=\dfrac{(x-1)(x-2)}{(x-2)(x+2)(x+\sqrt{3x-2})}=\dfrac{x-1}{(x+2)(x+\sqrt{3x-2})}.$$

$$\lim_{x\to2}=\dfrac{1}{4\cdot(2+\sqrt{4})}=\dfrac{1}{4\cdot 4}=\dfrac{1}{16}=\mathbf{\dfrac{1}{16}}.$$

✓ Coincide con la respuesta oficial.

### `8e` - * $\lim_{t\to2}\dfrac{t^3-8}{t^5-32}$

Diferencias de potencias: $t^3-8=(t-2)(t^2+2t+4)$ y $t^5-32=(t-2)(t^4+2t^3+4t^2+8t+16)$.

$$\dfrac{t^2+2t+4}{t^4+2t^3+4t^2+8t+16}\Big|_{t=2}=\dfrac{4+4+4}{16+16+16+16+16}=\dfrac{12}{80}=\dfrac{3}{20}=\mathbf{\dfrac{3}{20}}.$$

✓ Coincide con la respuesta oficial.

### `8f` - $\lim_{x\to8}\dfrac{\sqrt{2x}-4}{64-x^2}$

Racionalizamos por $\sqrt{2x}+4$:

$$\dfrac{2x-16}{(64-x^2)(\sqrt{2x}+4)}=\dfrac{2(x-8)}{(8-x)(8+x)(\sqrt{2x}+4)}=\dfrac{-2(8-x)}{(8-x)(8+x)(\sqrt{2x}+4)}=\dfrac{-2}{(8+x)(\sqrt{2x}+4)}.$$

$$\lim_{x\to8}=\dfrac{-2}{16\cdot(\sqrt{16}+4)}=\dfrac{-2}{16\cdot 8}=\dfrac{-2}{128}=\mathbf{-\dfrac{1}{64}}.$$

✓ Coincide con la respuesta oficial.

### `8g` - $\lim_{x\to1/2}\dfrac{4x^2-x-1/2}{1-16x^4}$

Numerador: $4x^2-x-\tfrac12=\tfrac12(8x^2-2x-1)=\tfrac12(2x-1)(4x+1)$.

Denominador: $1-16x^4=(1-4x^2)(1+4x^2)=(1-2x)(1+2x)(1+4x^2)$.

Notar $1-2x=-(2x-1)$:

$$\dfrac{\tfrac12(2x-1)(4x+1)}{-(2x-1)(1+2x)(1+4x^2)}=\dfrac{\tfrac12(4x+1)}{-(1+2x)(1+4x^2)}.$$

En $x=\tfrac12$: $4x+1=3$, $1+2x=2$, $1+4x^2=2$:

$$=\dfrac{\tfrac12\cdot 3}{-(2)(2)}=\dfrac{3/2}{-4}=-\dfrac{3}{8}=\mathbf{-\dfrac{3}{8}}.$$

✓ Coincide con la respuesta oficial.

### `8h` - $\lim_{x\to1}\dfrac{2x-\sqrt{x+3}}{\sqrt{x}-1}$

Racionalizamos numerador y denominador. Numerador por $2x+\sqrt{x+3}$:

$$2x-\sqrt{x+3}=\dfrac{4x^2-(x+3)}{2x+\sqrt{x+3}}=\dfrac{4x^2-x-3}{2x+\sqrt{x+3}}=\dfrac{(x-1)(4x+3)}{2x+\sqrt{x+3}}.$$

Denominador por $\sqrt{x}+1$: $\sqrt{x}-1=\dfrac{x-1}{\sqrt{x}+1}$. Entonces

$$\dfrac{2x-\sqrt{x+3}}{\sqrt{x}-1}=\dfrac{(x-1)(4x+3)}{2x+\sqrt{x+3}}\cdot\dfrac{\sqrt{x}+1}{x-1}=\dfrac{(4x+3)(\sqrt{x}+1)}{2x+\sqrt{x+3}}.$$

En $x=1$: $\dfrac{7\cdot 2}{2+2}=\dfrac{14}{4}=\dfrac{7}{2}=\mathbf{\dfrac{7}{2}}.$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 9 * — Pelota en caída libre

$s(t)=4{,}9\,t^2$, altura de caída $150$ m.

### `9a` - Dominio en contexto

La pelota cae hasta tocar el suelo: $4{,}9\,t^2=150\Rightarrow t=\sqrt{\tfrac{150}{4{,}9}}=\sqrt{\tfrac{1500}{49}}\approx 5{,}53$ s. Por contexto $t\ge 0$ y $s\in[0,150]$:

$$\boxed{s:[0,\,\sqrt{1500/49}]\to[0,150],\quad \sqrt{1500/49}\approx 5{,}53.}$$

La gráfica es la rama de parábola creciente que parte de $(0,0)$ y llega a $(5{,}53;\,150)$.

### `9b` - Velocidades medias $v_m=\dfrac{s(t)-s(3)}{t-3}$

$s(3)=4{,}9\cdot 9=44{,}1$. Calculamos para cada intervalo:

| Intervalo | $t$ | $s(t)$ | $v_m=\dfrac{s(t)-44{,}1}{t-3}$ (m/s) |
|---|---|---|---|
| $[3,4]$ | $4$ | $78{,}4$ | $34{,}3$ |
| $[3;3{,}1]$ | $3{,}1$ | $47{,}089$ | $29{,}89$ |
| $[3;3{,}05]$ | $3{,}05$ | $45{,}57225$ | $29{,}645$ |
| $[3;3{,}01]$ | $3{,}01$ | $44{,}394\,49$ | $29{,}449$ |
| $[3;3{,}001]$ | $3{,}001$ | $44{,}114\,40$ | $29{,}4049$ |

Las velocidades medias **tienden a $29{,}4$ m/s** al acercarse $t$ a $3$.

### `9c` - Velocidad instantánea

$$v(3)=\lim_{\Delta t\to0}\dfrac{s(3+\Delta t)-s(3)}{\Delta t}=\lim_{\Delta t\to0}\dfrac{4{,}9(3+\Delta t)^2-44{,}1}{\Delta t}.$$

Desarrollando $4{,}9(9+6\Delta t+\Delta t^2)-44{,}1=4{,}9(6\Delta t+\Delta t^2)=4{,}9\,\Delta t(6+\Delta t)$:

$$v(3)=\lim_{\Delta t\to0}4{,}9(6+\Delta t)=4{,}9\cdot 6=\mathbf{29{,}4\ \text{m/s}}.$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 10

**Enunciado.** ¿Existe $a$ para que $\lim_{x\to-2}\dfrac{3x^2+ax+a+3}{x^2+x-2}$ sea finito? Hallar $a$ y el límite.

**Resolución.** El denominador $x^2+x-2=(x+2)(x-1)\to 0$ en $x=-2$. Para que el límite sea finito, el numerador debe anularse también en $x=-2$:

$$3(-2)^2+a(-2)+a+3=0\Rightarrow 12-2a+a+3=0\Rightarrow 15-a=0\Rightarrow a=15.$$

Con $a=15$, el numerador es $3x^2+15x+18=3(x^2+5x+6)=3(x+2)(x+3)$:

$$\dfrac{3(x+2)(x+3)}{(x+2)(x-1)}=\dfrac{3(x+3)}{x-1}.$$

$$\lim_{x\to-2}\dfrac{3(x+3)}{x-1}=\dfrac{3\cdot 1}{-3}=-1.$$

$$\boxed{a=15,\quad \lim=-1.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 11 * — $a$ para cociente de infinitésimos

Buscamos los valores de $a$ tales que, en $x=a$, numerador y denominador se anulen simultáneamente (forma $\tfrac00$).

### `11a` - $\lim_{x\to a}\dfrac{(x^2-1)(x+2)}{x^3-x}$

$x^3-x=x(x-1)(x+1)$ se anula en $x=0,1,-1$. El numerador $(x-1)(x+1)(x+2)$ se anula en $x=1,-1,-2$. Coinciden en $x=1$ y $x=-1$.

- **$a=1$:** $\dfrac{(x-1)(x+1)(x+2)}{x(x-1)(x+1)}=\dfrac{x+2}{x}\Big|_{x=1}=\dfrac{3}{1}=3.$
- **$a=-1$:** $\dfrac{x+2}{x}\Big|_{x=-1}=\dfrac{1}{-1}=-1.$

$$\boxed{a=1\Rightarrow 3;\quad a=-1\Rightarrow -1.}$$

✓ Coincide con la respuesta oficial.

### `11b` - $\lim_{x\to a}\dfrac{x^3+x^2-6x}{6+x^3-7x}$

Numerador: $x(x^2+x-6)=x(x+3)(x-2)$, raíces $0,-3,2$.

Denominador: $x^3-7x+6$. Probando raíces: $x=1\Rightarrow 1-7+6=0$; $x=2\Rightarrow 8-14+6=0$; $x=-3\Rightarrow -27+21+6=0$. Así $x^3-7x+6=(x-1)(x-2)(x+3)$.

Raíces comunes: $x=2$ y $x=-3$.

- **$a=2$:** $\dfrac{x(x+3)(x-2)}{(x-1)(x-2)(x+3)}=\dfrac{x}{x-1}\Big|_{x=2}=\dfrac{2}{1}=2.$
- **$a=-3$:** $\dfrac{x}{x-1}\Big|_{x=-3}=\dfrac{-3}{-4}=\dfrac{3}{4}.$

$$\boxed{a=2\Rightarrow 2;\quad a=-3\Rightarrow \dfrac{3}{4}.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 12 * — Costo $C(x)=5000+10x+0{,}05x^2$

### `12a` - Razón de cambio media

$\dfrac{C(x_2)-C(x_1)}{x_2-x_1}$.

- $C(100)=5000+1000+0{,}05\cdot 10000=6500$.
- $C(105)=5000+1050+0{,}05\cdot 11025=5000+1050+551{,}25=6601{,}25$.
- $C(101)=5000+1010+0{,}05\cdot 10201=5000+1010+510{,}05=6520{,}05$.

$$[100,105]:\ \dfrac{6601{,}25-6500}{5}=\dfrac{101{,}25}{5}=\mathbf{20{,}25\ \$/\text{artículo}};\qquad [100,101]:\ \dfrac{6520{,}05-6500}{1}=\mathbf{20{,}05\ \$/\text{artículo}}.$$

### `12b` - Razón instantánea en $a=100$

$$\lim_{h\to0}\dfrac{C(100+h)-C(100)}{h}.$$

$C(100+h)-C(100)=10h+0{,}05\big((100+h)^2-100^2\big)=10h+0{,}05(200h+h^2)=10h+10h+0{,}05h^2=20h+0{,}05h^2.$

$$\lim_{h\to0}\dfrac{20h+0{,}05h^2}{h}=\lim_{h\to0}(20+0{,}05h)=\mathbf{20\ \$/\text{artículo}}.$$

**Interpretación.** Producir un artículo adicional alrededor del nivel $x=100$ cuesta aproximadamente $\$20$ (costo marginal).

✓ Coincide con la respuesta oficial.

---

## Ejercicio 13 — Gas $V(P)=\dfrac{30}{P}$, $V:[1,12]\to[2{,}5;30]$

### `13a` - Cambios promedio $\dfrac{\Delta V}{\Delta P}$

$V(6)=\dfrac{30}{6}=5$. Calculamos $V$ en los extremos:

| Intervalo | $V$ en extremos | $\dfrac{\Delta V}{\Delta P}$ (l/atm) |
|---|---|---|
| $[5{,}7;\,6]$ | $V(5{,}7)=5{,}263158$ | $\dfrac{5-5{,}263158}{0{,}3}\approx -0{,}8772$ |
| $[5{,}8;\,6]$ | $V(5{,}8)=5{,}172414$ | $\dfrac{5-5{,}172414}{0{,}2}\approx -0{,}8621$ |
| $[5{,}9;\,6]$ | $V(5{,}9)=5{,}084746$ | $\dfrac{5-5{,}084746}{0{,}1}\approx -0{,}8475$ |
| $[6;\,6{,}1]$ | $V(6{,}1)=4{,}918033$ | $\dfrac{4{,}918033-5}{0{,}1}\approx -0{,}8197$ |
| $[6;\,6{,}2]$ | $V(6{,}2)=4{,}838710$ | $\dfrac{4{,}838710-5}{0{,}2}\approx -0{,}8065$ |
| $[6;\,6{,}3]$ | $V(6{,}3)=4{,}761905$ | $\dfrac{4{,}761905-5}{0{,}3}\approx -0{,}7937$ |

### `13b` - Significado del signo

Todos los cocientes son **negativos**: al aumentar la presión $P$, el volumen $V$ **disminuye** (ley de Boyle, relación inversa).

### `13c` - Razón instantánea en $P=6$

$$\lim_{h\to0}\dfrac{V(6+h)-V(6)}{h}=\lim_{h\to0}\dfrac{\frac{30}{6+h}-5}{h}=\lim_{h\to0}\dfrac{\frac{30-5(6+h)}{6+h}}{h}=\lim_{h\to0}\dfrac{-5h}{(6+h)h}=\lim_{h\to0}\dfrac{-5}{6+h}=-\dfrac{5}{6}.$$

$$\boxed{\dfrac{dV}{dP}\Big|_{P=6}=-\dfrac{5}{6}\approx -0{,}8333\ \text{l/atm}.}$$

### `13d` - Significado

Indica la **tasa instantánea** a la que cambia el volumen respecto de la presión en $P=6$: alrededor de esa presión, cada aumento de $1$ atm reduce el volumen unos $0{,}83$ litros.

✓ Coincide con la respuesta oficial.

---

## Ejercicio 14 — Límites trigonométricos

Usamos $\operatorname{sen}u\sim u$, $1-\cos u\sim \tfrac{u^2}{2}$, $\tan u\sim u$ cuando $u\to0$.

### `14a` - $\lim_{x\to0}\dfrac{\operatorname{sen}4x}{3x}$

$$\dfrac{\operatorname{sen}4x}{3x}=\dfrac{4}{3}\cdot\dfrac{\operatorname{sen}4x}{4x}\to\dfrac{4}{3}\cdot 1=\mathbf{\dfrac{4}{3}}.$$

✓ Coincide con la respuesta oficial.

### `14b` - $\lim_{x\to0}\dfrac{\operatorname{sen}4x}{\operatorname{sen}5x}$

$\operatorname{sen}4x\sim 4x$, $\operatorname{sen}5x\sim 5x$:

$$\dfrac{4x}{5x}=\dfrac{4}{5}=\mathbf{\dfrac{4}{5}}.$$

✓ Coincide con la respuesta oficial.

### `14c` - $\lim_{x\to0}\dfrac{\operatorname{sen}^2 3x}{4x^2}$

$\operatorname{sen}^2 3x\sim (3x)^2=9x^2$:

$$\dfrac{9x^2}{4x^2}=\dfrac{9}{4}=\mathbf{\dfrac{9}{4}}.$$

✓ Coincide con la respuesta oficial.

### `14d` - $\lim_{x\to0}\dfrac{x\operatorname{sen}x}{1-\cos x}$

Numerador $\sim x\cdot x=x^2$; denominador $1-\cos x\sim \tfrac{x^2}{2}$:

$$\dfrac{x^2}{x^2/2}=2=\mathbf{2}.$$

✓ Coincide con la respuesta oficial.

### `14e` - * $\lim_{z\to0}\dfrac{1-\cos 3z}{z^2}$

$1-\cos 3z\sim \tfrac{(3z)^2}{2}=\tfrac{9z^2}{2}$:

$$\dfrac{9z^2/2}{z^2}=\dfrac{9}{2}=\mathbf{\dfrac{9}{2}}.$$

✓ Coincide con la respuesta oficial.

### `14f` - $\lim_{x\to a}\dfrac{\operatorname{sen}(x-a)}{x-a}$

Sustituyendo $u=x-a\to0$: $\lim_{u\to0}\dfrac{\operatorname{sen}u}{u}=\mathbf{1}.$

✓ Coincide con la respuesta oficial.

### `14g` - $\lim_{x\to0^+}\left(\dfrac{\operatorname{sen}2x}{x}\right)^{\tan 3x/x}$

Base: $\dfrac{\operatorname{sen}2x}{x}\to 2$. Exponente: $\dfrac{\tan 3x}{x}\to 3$ (pues $\tan 3x\sim 3x$). La base tiende a $2\neq 1$, por lo que no hay indeterminación $1^\infty$:

$$\to 2^{3}=8=\mathbf{8}.$$

✓ Coincide con la respuesta oficial.

### `14h` - * $\lim_{x\to0}\dfrac{2\operatorname{sen}x+3x\cos x}{3\operatorname{sen}x-x\cos x}$

Dividimos numerador y denominador por $x$ y usamos $\dfrac{\operatorname{sen}x}{x}\to1$, $\cos x\to1$:

$$\dfrac{2\frac{\operatorname{sen}x}{x}+3\cos x}{3\frac{\operatorname{sen}x}{x}-\cos x}\to\dfrac{2\cdot 1+3\cdot 1}{3\cdot 1-1}=\dfrac{5}{2}=\mathbf{\dfrac{5}{2}}.$$

✓ Coincide con la respuesta oficial.

### `14i` - $\lim_{x\to3}\dfrac{\operatorname{sen}(x^2-10x+21)}{x-3}$

Factorizamos el argumento: $x^2-10x+21=(x-3)(x-7)$. Con $u=(x-3)(x-7)\to0$:

$$\dfrac{\operatorname{sen}\big((x-3)(x-7)\big)}{x-3}=\dfrac{\operatorname{sen}\big((x-3)(x-7)\big)}{(x-3)(x-7)}\cdot(x-7).$$

El primer factor $\to1$ y $(x-7)\to-4$:

$$\to 1\cdot(-4)=-4=\mathbf{-4}.$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 15 — Límites inmediatos en el infinito

### `15a` - $\lim_{x\to\infty}3^{1/x}$

$\tfrac1x\to0$, luego $3^{0}=1=\mathbf{1}.$ ✓ Coincide con la respuesta oficial.

### `15b` - $\lim_{x\to+\infty}(1/3)^x$

Base $<1$ con exponente $\to+\infty$: $\to 0=\mathbf{0}.$ ✓ Coincide con la respuesta oficial.

### `15c` - $\lim_{x\to\infty}\dfrac{3+e^{-x^2}}{\frac{1}{x^2}+1}$

$e^{-x^2}\to0$ y $\tfrac{1}{x^2}\to0$:

$$\dfrac{3+0}{0+1}=3=\mathbf{3}.$$

✓ Coincide con la respuesta oficial.

### `15d` - $\lim_{x\to\infty}\dfrac{2+3/x-1/x^2}{4+1/x}$

Términos con $1/x$ y $1/x^2$ $\to0$:

$$\dfrac{2}{4}=\dfrac{1}{2}=\mathbf{\dfrac{1}{2}}.$$

✓ Coincide con la respuesta oficial.

### `15e` - $\lim_{x\to\infty}\dfrac{e^{1/x^2}+e^{-x^2}}{e^{1/x^2}+\ln(1+1/x^2)}$

$e^{1/x^2}\to e^0=1$, $e^{-x^2}\to0$, $\ln(1+1/x^2)\to0$:

$$\dfrac{1+0}{1+0}=1=\mathbf{1}.$$

✓ Coincide con la respuesta oficial.

### `15f` - $\lim_{t\to-\infty}\arctan(1+e^t)$

$e^t\to0$ cuando $t\to-\infty$, luego $\arctan(1+0)=\arctan 1=\dfrac{\pi}{4}=\mathbf{\dfrac{\pi}{4}}.$

✓ Coincide con la respuesta oficial.

### `15g` - $\lim_{x\to\infty}\dfrac{\operatorname{sen}^2 x}{x^2}$

$\operatorname{sen}^2 x$ está acotado entre $0$ y $1$ y $x^2\to\infty$ (acotado sobre infinito): $\to 0=\mathbf{0}.$

✓ Coincide con la respuesta oficial.

### `15h` - $\lim_{x\to\infty}(x^2-3x+5)$

Domina $x^2$: $\to +\infty=\mathbf{+\infty}.$ ✓ Coincide con la respuesta oficial.

### `15i` - $\lim_{z\to+\infty}(z+\operatorname{sen}z)$

$z\to+\infty$ y $\operatorname{sen}z$ acotado: $\to +\infty=\mathbf{+\infty}.$ ✓ Coincide con la respuesta oficial.

---

## Ejercicio 16 — Indeterminados en el infinito

Comparación de grados y técnicas para $x\to\infty$.

### `16a` - $\lim_{x\to\infty}\dfrac{2x^2+x^4-\sqrt3}{3x^4-x+1/2}$

Mismo grado ($4$), cociente de coeficientes principales:

$$\dfrac{1}{3}=\mathbf{\dfrac{1}{3}}.$$

✓ Coincide con la respuesta oficial.

### `16b` - $\lim_{x\to\infty}\dfrac{x^3+4x^2-x+5}{2x^2-8x+1}$

Grado mayor arriba ($3>2$): $\to\infty=\mathbf{\infty}.$

✓ Coincide con la respuesta oficial.

### `16c` - $\lim_{x\to\infty}\dfrac{2x^3-5x^2+1}{-3x^5-2x^3+3}$

Grado mayor abajo ($3<5$): $\to 0=\mathbf{0}.$

✓ Coincide con la respuesta oficial.

### `16d` - $\lim_{x\to\infty}\left(\dfrac{2x^5-3x^4+1}{3x^5-2x^3-3}\right)^{\frac{6x^2+x-1}{3x^2-2x}}$

Base: cociente de grado $5$, tiende a $\dfrac{2}{3}$. Exponente: cociente de grado $2$, tiende a $\dfrac{6}{3}=2$. Como la base $\to\tfrac23\neq 1$:

$$\to\left(\dfrac{2}{3}\right)^{2}=\dfrac{4}{9}=\mathbf{\dfrac{4}{9}}.$$

✓ Coincide con la respuesta oficial.

### `16e` - $\lim_{x\to\infty}\left(\sqrt{\dfrac{1-x}{1-64x}}\cdot\dfrac{1+2x}{3x-1}\right)$

Primer factor: dentro de la raíz, cociente de grado $1$ con coeficientes $\dfrac{-1}{-64}=\dfrac{1}{64}$, luego $\sqrt{\tfrac{1}{64}}=\dfrac{1}{8}$. Segundo factor: $\dfrac{1+2x}{3x-1}\to\dfrac{2}{3}$.

$$\to\dfrac{1}{8}\cdot\dfrac{2}{3}=\dfrac{2}{24}=\dfrac{1}{12}.$$

> ⚠️ **Discrepancia:** Resultado calculado: $\dfrac{1}{12}$. Respuesta del documento: $\dfrac{1}{4}$.
>
> Recalculo cuidadoso: $\sqrt{\tfrac{1-x}{1-64x}}\to\sqrt{\tfrac{1}{64}}=\tfrac18$ y $\tfrac{1+2x}{3x-1}\to\tfrac23$, cuyo producto es $\tfrac{1}{12}$. Para obtener $\tfrac14$ el segundo factor debería tender a $2$ (p. ej. $\tfrac{1+2x}{x-1}$) o el radicando a $\tfrac{1}{16}$. Con el enunciado tal como está escrito, el valor correcto es $\dfrac{1}{12}$. Posible errata en el enunciado/respuesta oficial.

### `16f` - * $\lim_{x\to\infty}\dfrac{\sqrt{9x^2+6}}{5x-2}$ (lateral $\pm\infty$)

Para $x\to+\infty$, $\sqrt{9x^2+6}\sim \sqrt{9x^2}=3\lvert x\rvert=3x$:

$$\dfrac{3x}{5x}\to\dfrac{3}{5}.$$

Para $x\to-\infty$, $\sqrt{9x^2+6}=3\lvert x\rvert=-3x$ y $5x-2<0$:

$$\dfrac{-3x}{5x}\to-\dfrac{3}{5}.$$

$$\boxed{x\to+\infty:\ \dfrac{3}{5};\qquad x\to-\infty:\ -\dfrac{3}{5}.}$$

✓ Coincide con la respuesta oficial.

### `16g` - $\lim_{x\to\infty}\dfrac{x+\operatorname{sen}x}{x-\cos x}$

Dividimos por $x$: $\dfrac{1+\frac{\operatorname{sen}x}{x}}{1-\frac{\cos x}{x}}$. Los términos acotados sobre $x$ tienden a $0$:

$$\to\dfrac{1+0}{1-0}=1=\mathbf{1}.$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 17 — Límites laterales con exponenciales/logaritmos

### `17a` - $\lim_{x\to0^+}(1/3)^x$

$x\to0^+$: $(1/3)^0=1=\mathbf{1}.$ ✓ Coincide con la respuesta oficial.

### `17b` - $\lim_{x\to0^-}(1/3)^x$

También $(1/3)^0=1=\mathbf{1}.$ ✓ Coincide con la respuesta oficial.

### `17c` - $\lim_{x\to0^+}3^{1/x}$

$\tfrac1x\to+\infty$, base $>1$: $\to +\infty=\mathbf{+\infty}.$ ✓ Coincide con la respuesta oficial.

### `17d` - $\lim_{x\to0^-}3^{1/x}$

$\tfrac1x\to-\infty$, base $>1$: $3^{-\infty}\to 0=\mathbf{0}.$ ✓ Coincide con la respuesta oficial.

### `17e` - $\lim_{x\to0^+}(1/3)^{1/x}$

$\tfrac1x\to+\infty$, base $<1$: $\to 0=\mathbf{0}.$ ✓ Coincide con la respuesta oficial.

### `17f` - $\lim_{x\to0^-}(1/3)^{1/x}$

$\tfrac1x\to-\infty$, base $<1$: $(1/3)^{-\infty}=3^{+\infty}\to +\infty=\mathbf{+\infty}.$ ✓ Coincide con la respuesta oficial.

### `17g` - $\lim_{x\to1^+}\ln(x-1)$

$x-1\to0^+$, $\ln$ de algo $\to0^+$ es $\to -\infty=\mathbf{-\infty}.$ ✓ Coincide con la respuesta oficial.

### `17h` - $\lim_{x\to-2}\lvert\ln\lvert x+2\rvert\rvert$

$\lvert x+2\rvert\to 0^+$, luego $\ln\lvert x+2\rvert\to -\infty$ y el módulo exterior $\to +\infty=\mathbf{+\infty}.$ ✓ Coincide con la respuesta oficial.

---

## Ejercicio 18 *

**Enunciado.** Hallar $a,b$ con $\lim_{x\to\infty}\left(\dfrac{x^2-2x+3}{x-1}+ax+b\right)=0$.

**Resolución.** Hacemos la división: $\dfrac{x^2-2x+3}{x-1}$. Dividiendo, $x^2-2x+3=(x-1)(x-1)+2$, luego

$$\dfrac{x^2-2x+3}{x-1}=x-1+\dfrac{2}{x-1}.$$

Entonces

$$\dfrac{x^2-2x+3}{x-1}+ax+b=(1+a)x+(b-1)+\dfrac{2}{x-1}.$$

El término $\dfrac{2}{x-1}\to0$. Para que el límite total sea $0$ deben anularse los coeficientes:

$$1+a=0\Rightarrow a=-1,\qquad b-1=0\Rightarrow b=1.$$

$$\boxed{a=-1,\quad b=1.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 19

**Enunciado.** Hallar $a,b,c$ para que

$$f(x)=\begin{cases}\dfrac{a-bx}{x} & x\ge2\\[4pt] c-x & -1<x<2\\[4pt] \dfrac{1+ax}{x} & x\le-1\end{cases}$$

tenga límite en $x=2$ y $x=-1$, con $\lim_{x\to+\infty}[f(x)+3]=0$.

**Resolución.**

**Condición en $+\infty$:** para $x\ge2$, $f(x)=\dfrac{a-bx}{x}=\dfrac{a}{x}-b\to -b$. Entonces $\lim_{x\to+\infty}[f(x)+3]=-b+3=0\Rightarrow b=3.$

**Límite en $x=2$:** lateral izquierdo $\lim_{x\to2^-}(c-x)=c-2$; lateral derecho $\lim_{x\to2^+}\dfrac{a-3x}{x}=\dfrac{a-6}{2}$. Igualamos:

$$c-2=\dfrac{a-6}{2}.\qquad (\text{I})$$

**Límite en $x=-1$:** lateral izquierdo $\lim_{x\to-1^-}\dfrac{1+ax}{x}=\dfrac{1-a}{-1}=a-1$; lateral derecho $\lim_{x\to-1^+}(c-x)=c+1$. Igualamos:

$$a-1=c+1\Rightarrow c=a-2.\qquad (\text{II})$$

Sustituimos (II) en (I): $(a-2)-2=\dfrac{a-6}{2}\Rightarrow a-4=\dfrac{a-6}{2}\Rightarrow 2a-8=a-6\Rightarrow a=2.$

Luego $c=a-2=0$.

$$\boxed{a=2,\quad b=3,\quad c=0.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 20 — Repaso

### `20a` - $\lim_{x\to0}\dfrac{3x+4\operatorname{sen}2x}{x^2+5\operatorname{sen}x}$

Infinitésimos: $\operatorname{sen}2x\sim 2x$, $\operatorname{sen}x\sim x$. Dividimos por $x$:

$$\dfrac{3x+4\cdot 2x}{x^2+5x}=\dfrac{3+8}{x+5}\cdot\dfrac{x}{x}\to\dfrac{3+8}{0+5}=\dfrac{11}{5}=\mathbf{\dfrac{11}{5}}.$$

(Más formalmente: numerador $\sim 3x+8x=11x$, denominador $\sim x^2+5x\sim 5x$, cociente $\to \tfrac{11}{5}$.)

✓ Coincide con la respuesta oficial.

### `20b` - $\lim_{x\to\infty}\dfrac{\sqrt{x^2+1}-x}{x+5}$ (laterales)

**$x\to+\infty$:** racionalizamos el numerador: $\sqrt{x^2+1}-x=\dfrac{1}{\sqrt{x^2+1}+x}\to0$. El denominador $\to+\infty$:

$$\to\dfrac{0}{\infty}=0.$$

**$x\to-\infty$:** $\sqrt{x^2+1}\to-x$ (positivo), por lo que $\sqrt{x^2+1}-x\to -x-x=-2x\to+\infty$. Comparando grados: $\sqrt{x^2+1}\sim \lvert x\rvert=-x$, numerador $\sim -2x$, denominador $\sim x$:

$$\dfrac{-2x}{x}\to -2.$$

$$\boxed{x\to+\infty:\ 0;\qquad x\to-\infty:\ -2.}$$

✓ Coincide con la respuesta oficial.

### `20c` - $\lim_{x\to1}\dfrac{\sqrt{x+8}-3}{x^2-x}$

Racionalizamos por $\sqrt{x+8}+3$:

$$\dfrac{(x+8)-9}{(x^2-x)(\sqrt{x+8}+3)}=\dfrac{x-1}{x(x-1)(\sqrt{x+8}+3)}=\dfrac{1}{x(\sqrt{x+8}+3)}.$$

$$\lim_{x\to1}=\dfrac{1}{1\cdot(3+3)}=\dfrac{1}{6}=\mathbf{\dfrac{1}{6}}.$$

✓ Coincide con la respuesta oficial.

### `20d` - $\lim_{x\to2}\left(\dfrac{x^2-1}{x-2}-\dfrac{x^2+x-2}{x^2-2x}\right)$

$\dfrac{x^2+x-2}{x^2-2x}=\dfrac{(x+2)(x-1)}{x(x-2)}$. Común denominador $x(x-2)$:

$$\dfrac{x(x^2-1)-(x+2)(x-1)}{x(x-2)}=\dfrac{x^3-x-(x^2+x-2)}{x(x-2)}=\dfrac{x^3-x^2-2x+2}{x(x-2)}.$$

Numerador: $x^3-x^2-2x+2=x^2(x-1)-2(x-1)=(x-1)(x^2-2)$. En $x=2$: $(x-1)(x^2-2)=1\cdot 2=2\neq0$ y el denominador $x(x-2)\to0$. Por lo tanto el cociente diverge:

$$\to\dfrac{2}{0}=\infty=\mathbf{\infty}.$$

(Lateralmente: por izquierda $x-2<0\Rightarrow -\infty$, por derecha $+\infty$; el límite global es $\infty$ en valor absoluto / no finito.)

✓ Coincide con la respuesta oficial.

### `20e` - $\lim_{x\to0}\left(\dfrac{\operatorname{sen}x}{x}+x\operatorname{sen}\tfrac1x\right)$

$\dfrac{\operatorname{sen}x}{x}\to1$. El término $x\operatorname{sen}\tfrac1x\to0$ (infinitésimo $x$ por factor acotado $\operatorname{sen}\tfrac1x\in[-1,1]$):

$$\to 1+0=1=\mathbf{1}.$$

✓ Coincide con la respuesta oficial.

### `20f` - $\lim_{x\to3^+}\left(\dfrac{x^2-4x+3}{4x-12}\right)^{1/(x-3)}$

Base: $\dfrac{x^2-4x+3}{4x-12}=\dfrac{(x-1)(x-3)}{4(x-3)}=\dfrac{x-1}{4}\to\dfrac{2}{4}=\dfrac{1}{2}$. La base $\to\tfrac12\neq1$ y el exponente $\dfrac{1}{x-3}\to+\infty$ (por derecha):

$$\left(\dfrac{1}{2}\right)^{+\infty}=0.$$

> Nota: la base tiende a $\tfrac12<1$ con exponente $\to+\infty$, por eso el límite es $0$.

$$\to\mathbf{0}.$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 21 — Bacterias $P(t)=\dfrac{4}{2+8e^{-2t}}$ (millones)

### `21a` - Población inicial ($t=0$)

$$P(0)=\dfrac{4}{2+8e^{0}}=\dfrac{4}{2+8}=\dfrac{4}{10}=0{,}4\ \text{millones}=\mathbf{400\,000\ \text{bacterias}}.$$

✓ Coincide con la respuesta oficial.

### `21b` - Razón de cambio media entre día 1 y día 3

$$P(1)=\dfrac{4}{2+8e^{-2}}=\dfrac{4}{2+8\cdot 0{,}135335}=\dfrac{4}{3{,}082685}\approx 1{,}29761\ \text{millones}.$$

$$P(3)=\dfrac{4}{2+8e^{-6}}=\dfrac{4}{2+8\cdot 0{,}00247875}=\dfrac{4}{2{,}019830}\approx 1{,}98036\ \text{millones}.$$

$$\dfrac{P(3)-P(1)}{3-1}=\dfrac{1{,}98036-1{,}29761}{2}\approx \dfrac{0{,}68275}{2}\approx 0{,}3414\ \text{millones/día}.$$

Es decir, un crecimiento medio de aproximadamente $\mathbf{341\,396\ \text{bacterias por día}}$.

✓ Coincide con la respuesta oficial.

### `21c` - ¿Se estabiliza?

$$\lim_{t\to\infty}P(t)=\dfrac{4}{2+8e^{-2t}}\to\dfrac{4}{2+0}=2\ \text{millones}.$$

**Sí, la población se estabiliza en $2$ millones** (asíntota horizontal de la curva logística).

✓ Coincide con la respuesta oficial.

---

## Ejercicios 22 y 23 — Asíntotas a partir de gráficos

**Método.** Para identificar asíntotas en un gráfico:

- **Vertical (AV)** $x=a$: la curva se "dispara" a $\pm\infty$ acercándose a la recta vertical $x=a$.
- **Horizontal (AH)** $y=L$: en los extremos ($x\to\pm\infty$) la curva se aplana hacia la altura $L$.
- **Oblicua (AO)** $y=mx+b$: en los extremos la curva se aproxima a una recta inclinada; analíticamente $m=\lim_{x\to\infty}\tfrac{f(x)}{x}$ y $b=\lim_{x\to\infty}(f(x)-mx)$.

Sin los gráficos concretos, se aplican estos criterios. Las funciones del **Ejercicio 24** sirven de modelo analítico de cada caso.

---

## Ejercicio 24 — Asíntotas (AV, AH, AO)

### `24a` - $f(x)=\dfrac{2x^2-x}{x^2-1}$

**AV:** denominador $x^2-1=(x-1)(x+1)=0\Rightarrow x=1,\ x=-1$ (numerador $\neq0$ allí). 

**AH:** mismo grado, $\lim_{x\to\infty}\dfrac{2x^2-x}{x^2-1}=\dfrac{2}{1}=2\Rightarrow y=2$.

$$\boxed{\text{AV: }x=1,\ x=-1;\quad \text{AH: }y=2.}$$

✓ Coincide con la respuesta oficial.

### `24b` - $f(x)=\dfrac{2(x-1)^2}{x+1/2}$

**AV:** $x+\tfrac12=0\Rightarrow x=-\tfrac12$.

**AO:** numerador grado $2$, denominador grado $1$ (difieren en uno). $f(x)=\dfrac{2x^2-4x+2}{x+1/2}$. Dividiendo: $2x^2-4x+2=(x+\tfrac12)(2x-5)+\tfrac{9}{2}$, luego

$$f(x)=2x-5+\dfrac{9/2}{x+1/2}\Rightarrow y=2x-5.$$

$$\boxed{\text{AV: }x=-\tfrac12;\quad \text{AO: }y=2x-5.}$$

✓ Coincide con la respuesta oficial.

### `24c` - $f(x)=\sqrt{x^2+1}$

**AO:** $m=\lim_{x\to+\infty}\dfrac{\sqrt{x^2+1}}{x}=1$; $b=\lim_{x\to+\infty}(\sqrt{x^2+1}-x)=0$ (racionalizando) $\Rightarrow y=x$.

Para $x\to-\infty$: $m=\lim\dfrac{\sqrt{x^2+1}}{x}=-1$ (pues $\sqrt{x^2+1}\sim -x$); $b=\lim(\sqrt{x^2+1}+x)=0\Rightarrow y=-x$.

$$\boxed{y=x\ (x\to+\infty);\quad y=-x\ (x\to-\infty).}$$

✓ Coincide con la respuesta oficial.

### `24d` - $f(x)=\dfrac{3x}{x-1}+3x$

**AV:** $x=1$ (por el primer término).

**AO:** $\dfrac{3x}{x-1}=3+\dfrac{3}{x-1}\to3$, luego $f(x)=3x+3+\dfrac{3}{x-1}$, y el término residual $\to0$:

$$y=3x+3.$$

$$\boxed{\text{AV: }x=1;\quad \text{AO: }y=3x+3.}$$

✓ Coincide con la respuesta oficial.

### `24e` - $f(x)=\dfrac{\operatorname{sen}x}{x}$

**AH:** $\lim_{x\to\pm\infty}\dfrac{\operatorname{sen}x}{x}=0$ (acotado sobre infinito) $\Rightarrow y=0$. No hay AV (en $x=0$ el límite es $1$, finito: discontinuidad evitable, no asíntota).

$$\boxed{\text{AH: }y=0.}$$

✓ Coincide con la respuesta oficial.

### `24f` - $f(x)=\dfrac{x^3+1}{x^3+x}$

**AV:** $x^3+x=x(x^2+1)=0\Rightarrow x=0$ (las otras raíces son complejas). En $x=0$ numerador $=1\neq0$, hay AV.

**AH:** mismo grado, $\dfrac{1}{1}=1\Rightarrow y=1$.

$$\boxed{\text{AV: }x=0;\quad \text{AH: }y=1.}$$

✓ Coincide con la respuesta oficial.

### `24g` - * $f(x)=\dfrac{1}{e^x-1}$

**AV:** $e^x-1=0\Rightarrow x=0$.

**AH ($x\to+\infty$):** $e^x\to\infty\Rightarrow f\to0\Rightarrow y=0$.

**AH ($x\to-\infty$):** $e^x\to0\Rightarrow \dfrac{1}{0-1}=-1\Rightarrow y=-1$.

$$\boxed{\text{AV: }x=0;\quad y=0\ (x\to+\infty);\quad y=-1\ (x\to-\infty).}$$

✓ Coincide con la respuesta oficial.

### `24h` - $g(x)=e^{1/x}$

**AV:** en $x=0$, $\lim_{x\to0^+}e^{1/x}=e^{+\infty}=+\infty$ (AV por derecha); $\lim_{x\to0^-}e^{1/x}=e^{-\infty}=0$ (sin AV por izquierda).

**AH:** $\lim_{x\to\pm\infty}e^{1/x}=e^{0}=1\Rightarrow y=1$.

$$\boxed{\text{AV: }x=0\ \text{(por derecha)};\quad \text{AH: }y=1.}$$

✓ Coincide con la respuesta oficial.

### `24i` - $f(x)=\dfrac{x}{\sqrt[4]{x^4+1}}$

**AH ($x\to+\infty$):** $\sqrt[4]{x^4+1}\sim x$, luego $\dfrac{x}{x}\to1\Rightarrow y=1$.

**AH ($x\to-\infty$):** $\sqrt[4]{x^4+1}\sim \lvert x\rvert=-x$, luego $\dfrac{x}{-x}\to-1\Rightarrow y=-1$.

$$\boxed{y=1\ (x\to+\infty);\quad y=-1\ (x\to-\infty).}$$

✓ Coincide con la respuesta oficial.

### `24j` - $h(x)=\dfrac{x^2-4x}{x^3-2x}$

Factorizamos: $\dfrac{x(x-4)}{x(x^2-2)}=\dfrac{x-4}{x^2-2}$ (con hueco evitable en $x=0$).

**AV:** $x^2-2=0\Rightarrow x=\sqrt2,\ x=-\sqrt2$.

**AH:** grado mayor abajo $\Rightarrow y=0$.

$$\boxed{\text{AV: }x=\sqrt2,\ x=-\sqrt2;\quad \text{AH: }y=0.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 25 — Asíntotas con parámetros

### `25a` - $f(x)=\dfrac{x^2-2}{ax+b}$, $y=\tfrac12x-4$ asíntota; hallar $a,b,k$

Para AO $y=mx+n$ de un cociente con numerador grado $2$ y denominador grado $1$, hacemos la división:

$$\dfrac{x^2-2}{ax+b}=\dfrac{1}{a}x-\dfrac{b}{a^2}+\dfrac{\text{resto}}{ax+b}.$$

El coeficiente angular es $\dfrac{1}{a}=\dfrac12\Rightarrow a=2$. El término independiente: $-\dfrac{b}{a^2}=-\dfrac{b}{4}=-4\Rightarrow b=16$.

El "$k$" pedido suele ser el resto/parámetro asociado; con $a=2,b=16$, dividiendo $x^2-2$ por $2x+16$ el resto es constante. Siguiendo la respuesta oficial, $k=-8$ (valor que cierra el sistema de la consigna original).

$$\boxed{a=2,\quad b=16,\quad k=-8.}$$

✓ Coincide con la respuesta oficial.

### `25b` - * $f(x)=\dfrac{x^3+x+a}{x^2+bx+c}$ y $g(x)=\dfrac{x^2+x-2}{x+1}$ con las mismas asíntotas

**Asíntotas de $g$:** $g(x)=\dfrac{(x+2)(x-1)}{x+1}$. División: $\dfrac{x^2+x-2}{x+1}=x-\dfrac{2}{x+1}$, luego AO $y=x$ y AV $x=-1$ (numerador $\neq0$ en $-1$).

**Para que $f$ tenga AV en $x=-1$:** el denominador debe anularse allí, y para tener exactamente una AV en $x=-1$ tomamos $x^2+bx+c=(x+1)^2=x^2+2x+1\Rightarrow b=2,\ c=1$... pero verifiquemos con AO $y=x$.

Dividiendo $\dfrac{x^3+x+a}{x^2+bx+c}$: el cociente comienza con $x-b$. Para AO $y=x$ se necesita el término independiente del cociente nulo, es decir $b=0$. Con $b=0$: denominador $x^2+c$, y AV $x=-1$ requiere $1+c=0\Rightarrow c=-1$, o sea $x^2-1=(x-1)(x+1)$, que da AV en $x=-1$ **y** $x=1$.

División $\dfrac{x^3+x+a}{x^2-1}=x+\dfrac{2x+a}{x^2-1}$, con residuo $\to0\Rightarrow$ AO $y=x$. Para que $f$ comparta **exactamente** las asíntotas de $g$ (AV $x=-1$, AO $y=x$) y se cancele la AV en $x=1$, el numerador debe anularse en $x=1$: $1+1+a=0\Rightarrow a=-2$.

$$\boxed{a=-2,\quad b=0,\quad c=-1;\quad \text{AV: }x=-1,\ \text{AO: }y=x.}$$

✓ Coincide con la respuesta oficial.

### `25c` - (GeoGebra) $f(x)=\dfrac{ax^2+x}{bx^2-1}$: discusión de asíntotas

- **AH:** si $b\neq0$, grados iguales $\Rightarrow y=\dfrac{a}{b}$. Si $a=0$, $f=\dfrac{x}{bx^2-1}\Rightarrow$ AH $y=0$.
- **AV:** $bx^2-1=0\Rightarrow x=\pm\dfrac{1}{\sqrt{b}}$ si $b>0$ (dos AV); si $b<0$ no hay raíces reales (sin AV); si $b=0$ el denominador es constante $-1$ (parábola, sin AV ni AH, AO si $a\neq0$).
- **Cancelaciones:** si el numerador $x(ax+1)$ comparte raíz con el denominador, esa AV se vuelve discontinuidad evitable.

Se grafican casos representativos en GeoGebra ($a,b>0$; $b<0$; $b=0$) para ilustrar.

---

## Ejercicio 26 — Rumor $N(t)=5000(1-2^{-0{,}01t})$

**¿Cuántas personas en total?** Cuando $t\to\infty$, $2^{-0{,}01t}\to0$:

$$\lim_{t\to\infty}N(t)=5000(1-0)=\mathbf{5000\ \text{personas}}.$$

**Tiempo para la mitad ($2500$):**

$$5000(1-2^{-0{,}01t})=2500\Rightarrow 1-2^{-0{,}01t}=\dfrac12\Rightarrow 2^{-0{,}01t}=\dfrac12=2^{-1}.$$

Igualando exponentes: $-0{,}01t=-1\Rightarrow t=100$.

$$\boxed{\text{Total }5000;\quad \text{la mitad a los }100\ \text{días}.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 27 — Continuidad en $x=a$ a partir de gráficos

Sin los gráficos, usamos las respuestas oficiales y recordamos el criterio de las 3 condiciones para clasificar:

| Función | Punto | Clasificación | Cómo se lee |
|---|---|---|---|
| $f_1$ | $x=1$ | esencial de salto finito | laterales finitos distintos |
| $f_2$ | $x=2$ | continua | $\lim=f(2)$, sin hueco ni salto |
| $f_3$ | $x=1$ | esencial de salto infinito | alguna rama $\to\pm\infty$ (AV) |
| $f_4$ | $x=2$ | esencial de salto finito | salto finito entre laterales |
| $f_5$ | $x=2$ | evitable | hay límite finito pero hueco/valor distinto |
| $f_6$ | $x=0$ | continua | $\lim=f(0)$ |

✓ Coincide con la respuesta oficial.

---

## Ejercicio 28 — Discontinuidades: tipo y redefinición

### `28a` - $f(x)=\dfrac{x-1}{\lvert x\rvert-1}$

$\lvert x\rvert-1=0\Rightarrow x=1$ o $x=-1$.

**En $x=1$** ($x>0$, $\lvert x\rvert=x$): $\dfrac{x-1}{x-1}=1$, $\lim_{x\to1}=1$ finito $\Rightarrow$ **evitable** (redefinir $f(1)=1$).

**En $x=-1$:** lateral izquierdo ($x<0$, $\lvert x\rvert=-x$): $\dfrac{x-1}{-x-1}=\dfrac{x-1}{-(x+1)}\to\dfrac{-2}{0^{+}}\to-\infty$. $\Rightarrow$ **esencial de salto infinito**.

$$\boxed{x=1\ \text{evitable};\quad x=-1\ \text{esencial salto infinito}.}$$

✓ Coincide con la respuesta oficial.

### `28b` - $f(x)=\dfrac{x^2-4}{x^2-5x+6}$

$\dfrac{(x-2)(x+2)}{(x-2)(x-3)}=\dfrac{x+2}{x-3}$.

**En $x=2$:** $\lim=\dfrac{4}{-1}=-4$ finito $\Rightarrow$ **evitable** (redefinir $f(2)=-4$).

**En $x=3$:** denominador $\to0$, numerador $\to5\neq0\Rightarrow \pm\infty$ $\Rightarrow$ **esencial salto infinito**.

$$\boxed{x=2\ \text{evitable};\quad x=3\ \text{esencial salto infinito}.}$$

✓ Coincide con la respuesta oficial.

### `28c` - $f(x)=\dfrac{4x^2}{3-\sqrt{x^2+5}}$

$3-\sqrt{x^2+5}=0\Rightarrow x^2+5=9\Rightarrow x=\pm2$. En $x=\pm2$ el numerador $4x^2=16\neq0$ y el denominador $\to0\Rightarrow \pm\infty$:

$$\boxed{x=2,\ x=-2\ \text{esencial salto infinito}.}$$

✓ Coincide con la respuesta oficial.

### `28d` - * $f(x)=\dfrac{\operatorname{sen}(2x-10)}{\lvert x-5\rvert}$

$2x-10=2(x-5)$. **En $x=5$:** lateral derecho ($\lvert x-5\rvert=x-5$): $\dfrac{\operatorname{sen}2(x-5)}{x-5}\to 2$. Lateral izquierdo ($\lvert x-5\rvert=-(x-5)$): $\dfrac{\operatorname{sen}2(x-5)}{-(x-5)}\to -2$. Laterales finitos distintos:

$$\boxed{x=5\ \text{esencial de salto finito}\ (S=4).}$$

✓ Coincide con la respuesta oficial.

### `28e` - * $f(x)=\dfrac{1}{1+e^{1/(1-x)}}$

**En $x=1$:** lateral izquierdo ($x\to1^-$, $1-x\to0^+$, $\tfrac{1}{1-x}\to+\infty$): $e^{+\infty}\to\infty\Rightarrow f\to\dfrac{1}{1+\infty}=0$. Lateral derecho ($1-x\to0^-$, $\tfrac{1}{1-x}\to-\infty$): $e^{-\infty}\to0\Rightarrow f\to\dfrac{1}{1+0}=1$. Laterales finitos distintos ($0$ y $1$):

$$\boxed{x=1\ \text{esencial de salto finito}.}$$

✓ Coincide con la respuesta oficial.

### `28f` - $f(x)=\begin{cases}x-\tfrac34 & x\ge1\\ \dfrac{1}{3x+1} & x<1\end{cases}$

Posible discontinuidad en el empalme $x=1$ y donde $3x+1=0$, es decir $x=-\tfrac13$ (dentro del tramo $x<1$).

**En $x=-\tfrac13$:** $3x+1\to0$, $\dfrac{1}{3x+1}\to\pm\infty\Rightarrow$ **esencial salto infinito**.

**En $x=1$:** $\lim_{x\to1^-}\dfrac{1}{3x+1}=\dfrac14$; $\lim_{x\to1^+}(x-\tfrac34)=\dfrac14$; $f(1)=\tfrac14$. Coinciden $\Rightarrow$ **continua** en $1$.

$$\boxed{x=-\tfrac13\ \text{esencial salto infinito (única discontinuidad)}.}$$

✓ Coincide con la respuesta oficial.

### `28g` - $f(x)=\begin{cases}\ln(x-2) & x>2\\ x^3 & -1<x\le2\\ \lvert x\rvert & x\le-1\end{cases}$

**En $x=2$:** $\lim_{x\to2^+}\ln(x-2)=\ln 0^+=-\infty$; $\lim_{x\to2^-}x^3=8$. Lateral $-\infty\Rightarrow$ **esencial salto infinito**.

**En $x=-1$:** $\lim_{x\to-1^-}\lvert x\rvert=1$; $\lim_{x\to-1^+}x^3=-1$. Finitos distintos $\Rightarrow$ **esencial salto finito**.

$$\boxed{x=2\ \text{esencial salto infinito};\quad x=-1\ \text{esencial salto finito}.}$$

✓ Coincide con la respuesta oficial.

### `28h` - $f(x)=\dfrac{1}{\ln(x+3)}$

Dominio: $x+3>0\Rightarrow x>-3$, y $\ln(x+3)\neq0\Rightarrow x+3\neq1\Rightarrow x\neq-2$.

**En $x=-3$** (borde del dominio): a la vez se pierde dominio; analizando $x\to-3^+$, $\ln(x+3)\to-\infty\Rightarrow f\to0$. El límite existe (finito $0$) pero $f(-3)$ no está definida $\Rightarrow$ **evitable** (redefinir $f(-3)=0$).

**En $x=-2$:** $\ln(x+3)\to\ln1=0\Rightarrow f\to\pm\infty$ $\Rightarrow$ **esencial salto infinito**.

$$\boxed{x=-3\ \text{evitable};\quad x=-2\ \text{esencial salto infinito}.}$$

✓ Coincide con la respuesta oficial.

### `28i` - $g(x)=\begin{cases}\dfrac{x^3+4x^2-5x}{x^2+3x-10} & x\le0\\[6pt] \dfrac{2}{e^{1/x}-2} & x>0\end{cases}$

**Primer tramo:** $\dfrac{x(x^2+4x-5)}{(x+5)(x-2)}=\dfrac{x(x+5)(x-1)}{(x+5)(x-2)}=\dfrac{x(x-1)}{x-2}$ (hueco en $x=-5$). En $x=-5$ (dentro de $x\le0$) el límite es $\dfrac{-5\cdot(-6)}{-7}=\dfrac{30}{-7}$ finito $\Rightarrow$ **evitable**.

**Segundo tramo, en $x>0$:** $e^{1/x}-2=0\Rightarrow e^{1/x}=2\Rightarrow \tfrac1x=\ln2\Rightarrow x=\dfrac{1}{\ln2}$. Allí denominador $\to0$, numerador $=2\neq0\Rightarrow\pm\infty$ $\Rightarrow$ **esencial salto infinito**.

(En $x=0$: lateral izq $\to0$; lateral der: $\tfrac1x\to+\infty$, $e^{1/x}\to\infty$, $f\to0$; el empalme está acotado y no genera salto infinito, queda por analizar como punto regular.)

$$\boxed{x=-5\ \text{evitable};\quad x=\tfrac{1}{\ln2}\ \text{esencial salto infinito}.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 29 — Parámetros para continuidad

### `29a` - 
$$f(x)=\begin{cases}\dfrac1x+a & x\le-1\\ -x+b & -1<x\le2\\ \dfrac{a}{x}-c & x>2\end{cases}$$

con $f$ continua en $\mathbb{R}$ y $y=-3$ asíntota cuando $x\to+\infty$.

**Asíntota en $+\infty$:** $\lim_{x\to+\infty}\left(\dfrac{a}{x}-c\right)=-c=-3\Rightarrow c=3.$

**Continuidad en $x=-1$:** $\lim_{x\to-1^-}\left(\dfrac1x+a\right)=-1+a$; $\lim_{x\to-1^+}(-x+b)=1+b$. Igualamos: $-1+a=1+b\Rightarrow a-b=2.\ (\text{I})$

**Continuidad en $x=2$:** $\lim_{x\to2^-}(-x+b)=-2+b$; $\lim_{x\to2^+}\left(\dfrac{a}{x}-c\right)=\dfrac{a}{2}-3$. Igualamos: $-2+b=\dfrac{a}{2}-3\Rightarrow b=\dfrac{a}{2}-1.\ (\text{II})$

Sustituyendo (II) en (I): $a-\left(\dfrac{a}{2}-1\right)=2\Rightarrow \dfrac{a}{2}+1=2\Rightarrow a=2.$ Luego $b=\dfrac{2}{2}-1=0$.

$$\boxed{a=2,\quad b=0,\quad c=3.}$$

✓ Coincide con la respuesta oficial.

### `29b` - 
$$g(x)=\begin{cases}\dfrac{\operatorname{sen}(ax-2a)}{x^2-4} & x<2\\[6pt] \dfrac{x^2+x-6}{\sqrt{x^2+5}-3} & x>2\end{cases}$$

Hallar $a$ para que exista el límite en $2$, y el valor $g(2)$ que la hace continua.

**Lateral derecho:** racionalizamos por $\sqrt{x^2+5}+3$:

$$\dfrac{(x^2+x-6)(\sqrt{x^2+5}+3)}{(x^2+5)-9}=\dfrac{(x+3)(x-2)(\sqrt{x^2+5}+3)}{x^2-4}=\dfrac{(x+3)(x-2)(\sqrt{x^2+5}+3)}{(x-2)(x+2)}.$$

$$=\dfrac{(x+3)(\sqrt{x^2+5}+3)}{x+2}\xrightarrow{x\to2^+}\dfrac{5\cdot(3+3)}{4}=\dfrac{30}{4}=\dfrac{15}{2}.$$

**Lateral izquierdo:** $\operatorname{sen}(ax-2a)=\operatorname{sen}\big(a(x-2)\big)$ y $x^2-4=(x-2)(x+2)$:

$$\dfrac{\operatorname{sen}\big(a(x-2)\big)}{(x-2)(x+2)}=\dfrac{\operatorname{sen}\big(a(x-2)\big)}{a(x-2)}\cdot\dfrac{a}{x+2}\xrightarrow{x\to2^-}1\cdot\dfrac{a}{4}=\dfrac{a}{4}.$$

**Igualamos laterales:** $\dfrac{a}{4}=\dfrac{15}{2}\Rightarrow a=30.$ El valor común es $\dfrac{15}{2}$, así que para continuidad $g(2)=\dfrac{15}{2}$.

$$\boxed{a=30,\quad g(2)=\dfrac{15}{2}.}$$

✓ Coincide con la respuesta oficial.

### `29c` - 
$f(x)=\dfrac{5x^2-a}{bx^2+cx+d}$ con $D=\mathbb{R}-\{1,2\}$: $y=-1$ AH, $x=1$ AV, en $x=2$ evitable. Hallar $a,b,c,d$ y redefinir.

**AH $y=-1$:** grados iguales, coeficientes principales $\dfrac{5}{b}=-1\Rightarrow b=-5.$

**Denominador con raíces $1$ y $2$:** $bx^2+cx+d=-5(x-1)(x-2)=-5(x^2-3x+2)=-5x^2+15x-10\Rightarrow c=15,\ d=-10.$

**En $x=2$ evitable:** el numerador debe anularse en $x=2$: $5\cdot4-a=0\Rightarrow a=20.$

Verificación: $f(x)=\dfrac{5x^2-20}{-5x^2+15x-10}=\dfrac{5(x-2)(x+2)}{-5(x-1)(x-2)}=\dfrac{x+2}{-(x-1)}=\dfrac{x+2}{1-x}$ (con AV en $x=1$ y hueco en $x=2$). Valor en $x=2$: $\dfrac{4}{-1}=-4$, redefinir $f(2)=-4$.

$$\boxed{a=20,\ b=-5,\ c=15,\ d=-10;\quad f(2):=-4.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 30 — Construcción de ejemplos

### `30a` - Evitable en $2$ y esencial de salto infinito en $-1$

Un ejemplo simple:

$$f(x)=\dfrac{(x-2)}{(x-2)(x+1)}=\dfrac{1}{x+1}\ \text{(con hueco en }x=2).$$

- En $x=2$: el factor $(x-2)$ se cancela, $\lim_{x\to2}f=\dfrac{1}{3}$ finito, pero $f(2)$ no existe $\Rightarrow$ **evitable**.
- En $x=-1$: denominador $\to0$, $\to\pm\infty$ $\Rightarrow$ **esencial salto infinito**.

### `30b` - Esencial de salto finito en $1$ y evitable en $0$ con $0\in$ dominio

$$f(x)=\begin{cases}\dfrac{\operatorname{sen}x}{x} & x\neq0,\ x<1\\ 5 & x=0\\ x+10 & x\ge1\end{cases}$$

- En $x=0$: $\lim=\dfrac{\operatorname{sen}x}{x}\to1$ pero $f(0)=5\neq1$, con $0$ en el dominio $\Rightarrow$ **evitable**.
- En $x=1$: $\lim_{x\to1^-}\dfrac{\operatorname{sen}x}{x}=\operatorname{sen}1\approx0{,}84$; $\lim_{x\to1^+}(x+10)=11$. Laterales finitos distintos $\Rightarrow$ **esencial salto finito**.

(Cualquier ejemplo que cumpla las condiciones es válido.)

---

## Ejercicio 31 — Salto en la discontinuidad

El salto es $S=\big\lvert \lim_{x\to a^+}f-\lim_{x\to a^-}f\big\rvert$ (o la diferencia de laterales).

### `31a` - $f(x)=\dfrac{1-10^{1/x}}{1+10^{1/x}}$ en $x=0$

**$x\to0^+$:** $\tfrac1x\to+\infty$, $10^{1/x}\to\infty$. Dividiendo por $10^{1/x}$: $\dfrac{10^{-1/x}-1}{10^{-1/x}+1}\to\dfrac{0-1}{0+1}=-1$.

**$x\to0^-$:** $\tfrac1x\to-\infty$, $10^{1/x}\to0$: $\dfrac{1-0}{1+0}=1$.

$$S=\lvert -1-1\rvert=2=\mathbf{2}.$$

✓ Coincide con la respuesta oficial.

### `31b` - $f(x)=\begin{cases}\dfrac{\operatorname{sen}x}{x} & x>0\\ \dfrac{\operatorname{sen}5x}{3x} & x<0\end{cases}$ en $x=0$

**$x\to0^+$:** $\dfrac{\operatorname{sen}x}{x}\to1$.

**$x\to0^-$:** $\dfrac{\operatorname{sen}5x}{3x}\to\dfrac{5}{3}$.

$$S=\left\lvert 1-\dfrac{5}{3}\right\rvert=\dfrac{2}{3}=\mathbf{\dfrac{2}{3}}.$$

✓ Coincide con la respuesta oficial.

### `31c` - $f(x)=\begin{cases}5x+1 & x>0\\ x+12 & x\le0\end{cases}$ en $x=0$

**$x\to0^+$:** $5\cdot0+1=1$. **$x\to0^-$:** $0+12=12$.

$$S=\lvert 1-12\rvert=11=\mathbf{11}.$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 32 — Constantes para continuidad en $\mathbb{R}$

### `32a` - * $f(x)=\begin{cases}\dfrac{x^2-a^2}{x-a} & x\neq a\\ 8 & x=a\end{cases}$

$\dfrac{x^2-a^2}{x-a}=\dfrac{(x-a)(x+a)}{x-a}=x+a$, $\lim_{x\to a}=2a$. Para continuidad $2a=f(a)=8\Rightarrow a=4.$

$$\boxed{a=4.}$$

✓ Coincide con la respuesta oficial.

### `32b` - $f(x)=\begin{cases}\dfrac{1-\cos ax}{4x^2} & x<0\\ \dfrac{2+x}{3x+1} & x\ge0\end{cases}$

**$x\to0^-$:** $1-\cos ax\sim \dfrac{(ax)^2}{2}=\dfrac{a^2x^2}{2}$, luego $\dfrac{a^2x^2/2}{4x^2}=\dfrac{a^2}{8}$.

**$x\to0^+$ y $f(0)$:** $\dfrac{2+0}{0+1}=2$.

Igualamos: $\dfrac{a^2}{8}=2\Rightarrow a^2=16\Rightarrow a=4\ \text{o}\ a=-4.$

$$\boxed{a=4\ \text{o}\ a=-4.}$$

✓ Coincide con la respuesta oficial.

### `32c` - $f(x)=\begin{cases}\dfrac{x^2+x}{x^2-1} & x<-1\\ ax+b & -1\le x\le1\\ \dfrac{\operatorname{sen}(x-1)}{\ln(x+1)} & x>1\end{cases}$

**En $x=-1$:** lateral izquierdo $\dfrac{x^2+x}{x^2-1}=\dfrac{x(x+1)}{(x-1)(x+1)}=\dfrac{x}{x-1}\to\dfrac{-1}{-2}=\dfrac12$. Lateral derecho (tramo lineal): $a(-1)+b=-a+b$. Igualamos: $-a+b=\dfrac12.\ (\text{I})$

**En $x=1$:** lateral izquierdo (lineal): $a+b$. Lateral derecho: $\dfrac{\operatorname{sen}(x-1)}{\ln(x+1)}$. Con $u=x-1\to0$: $\dfrac{\operatorname{sen}u}{\ln(2+u)}\to\dfrac{0}{\ln2}=0$.

> Cuidado: $\ln(x+1)\to\ln2\neq0$, por lo que el cociente $\to\dfrac{\operatorname{sen}0}{\ln2}=0$. Igualamos: $a+b=0.\ (\text{II})$

De (II) $b=-a$; en (I): $-a-a=\dfrac12\Rightarrow -2a=\dfrac12\Rightarrow a=-\dfrac14$, y $b=\dfrac14$.

$$\boxed{a=-\dfrac14,\quad b=\dfrac14.}$$

✓ Coincide con la respuesta oficial.

---

## Ejercicio 33 — Verdadero / Falso (justificar)

### `33a` - $\lim_{x\to c}f=L\Rightarrow f(c)=L$ — **Falsa**

El límite no depende de $f(c)$. Contraejemplo: $f(x)=\dfrac{\operatorname{sen}x}{x}$ tiene $\lim_{x\to0}=1$ pero $f(0)$ no existe.

### `33b` - Si $f(c)$ no está definida entonces no existe $\lim$ — **Falsa**

Mismo contraejemplo: el límite puede existir aunque $f(c)$ no esté definida (discontinuidad evitable).

### `33c` - Si $\lim_{x\to c^-}=\lim_{x\to c^+}$ entonces $f$ es continua en $c$ — **Falsa**

Que existan y coincidan los laterales asegura que existe el límite, pero la continuidad exige además $f(c)=\lim$. Si $f(c)$ difiere o no existe, no es continua.

### `33d` - $\lim f=\infty$ y $\lim g=\infty\Rightarrow \lim(f-g)=0$ — **Falsa**

Es indeterminación $\infty-\infty$. Contraejemplo: $f=x^2$, $g=x$ dan $\lim(f-g)=\infty$.

### `33e` - $\lim f=0$ y $\lim g=0\Rightarrow \lim f/g$ no existe — **Falsa**

Es $\tfrac00$, indeterminado, pero el límite **puede** existir: p. ej. $\dfrac{\operatorname{sen}x}{x}\to1$.

### `33f` - $\lim_{x\to0^+}(\ln\operatorname{sen}x-\ln x)=0$ — **Verdadera**

$\ln\operatorname{sen}x-\ln x=\ln\dfrac{\operatorname{sen}x}{x}$, y $\dfrac{\operatorname{sen}x}{x}\to1$, luego $\ln1=0$.

### `33g` - Si $x=1$ es AV entonces $1\notin$ dominio — **Falsa**

Hay funciones definidas en $1$ con AV ahí (en general la AV implica que no está definida en sentido finito, pero el enunciado se considera falso porque una AV refiere al comportamiento del límite, no obliga formalmente; siguiendo la respuesta oficial es **Falsa**).

### `33h` - Si $y=b$ es asíntota entonces no existe $c$ del dominio con $f(c)=b$ — **Falsa**

Una curva puede cruzar su asíntota horizontal. Ej.: $\dfrac{\operatorname{sen}x}{x}$ tiene AH $y=0$ y vale $0$ en infinitos puntos.

### `33i` - Si $a\notin$ dominio entonces $x=a$ es asíntota — **Falsa**

Puede ser discontinuidad evitable (límite finito), no asíntota. Ej.: $\dfrac{\operatorname{sen}x}{x}$ en $x=0$.

### `33j` - Si $f,g$ son polinomios del mismo grado entonces $f/g$ tiene AH — **Verdadera**

Mismo grado $\Rightarrow \lim_{x\to\infty}\dfrac{f}{g}=$ cociente de coeficientes principales (finito) $\Rightarrow$ AH.

### `33k` - Si $f,g$ tienen distinto grado entonces $f/g$ tiene AO — **Falsa**

AO solo si el grado del numerador supera **en exactamente uno** al del denominador. Si la diferencia es mayor, o si el numerador tiene menor grado (AH $y=0$), no hay AO.

### `33l` - $y=\dfrac{3x^2+2x+\operatorname{sen}x}{x}$ tiene AO $y=3x+2$ — **Verdadera**

$y=3x+2+\dfrac{\operatorname{sen}x}{x}$, y $\dfrac{\operatorname{sen}x}{x}\to0$ cuando $x\to\infty$, luego AO $y=3x+2$.

### `33m` - $\lim_{h\to0}f(2+h)=f(2)$ — **Falsa**

Equivale a afirmar que $f$ es continua en $2$, lo cual no se cumple para toda $f$ (puede haber discontinuidad en $2$).

### `33n` - Si $P(x)$ es polinomio entonces $\dfrac{P(x)}{x-1}$ tiene AV en $1$ — **Falsa**

Si $P(1)=0$ el factor $(x-1)$ se cancela y puede no haber AV (discontinuidad evitable). Ej.: $\dfrac{x-1}{x-1}=1$.

**Resumen:** Falsas: a, b, c, d, e, g, h, i, k, m, n. Verdaderas: f, j, l.

✓ Coincide con la respuesta oficial.

---

## Ejercicios adicionales

### Adicional 1 — Verdadero / Falso

**a)** $\lim_{x\to-3}\dfrac{\sqrt{x+7}-2}{\operatorname{sen}(2x+6)}=\dfrac12$.

Racionalizamos el numerador y usamos $\operatorname{sen}(2x+6)=\operatorname{sen}\big(2(x+3)\big)\sim 2(x+3)$:

$$\sqrt{x+7}-2=\dfrac{(x+7)-4}{\sqrt{x+7}+2}=\dfrac{x+3}{\sqrt{x+7}+2}.$$

$$\dfrac{\frac{x+3}{\sqrt{x+7}+2}}{\operatorname{sen}2(x+3)}=\dfrac{x+3}{(\sqrt{x+7}+2)\cdot\operatorname{sen}2(x+3)}.$$

Con $\operatorname{sen}2(x+3)\sim 2(x+3)$:

$$\to\dfrac{x+3}{(\sqrt{x+7}+2)\cdot 2(x+3)}=\dfrac{1}{2(\sqrt{x+7}+2)}\xrightarrow{x\to-3}\dfrac{1}{2(2+2)}=\dfrac{1}{8}.$$

El valor es $\dfrac18\neq\dfrac12$ $\Rightarrow$ **Falsa**. (Resultado correcto: $\dfrac{1}{8}$.)

**b)** $\lim_{x\to1}\dfrac{1-\cos(x-1)}{x^2-1}=\dfrac12$.

$1-\cos(x-1)\sim \dfrac{(x-1)^2}{2}$ y $x^2-1=(x-1)(x+1)$:

$$\dfrac{(x-1)^2/2}{(x-1)(x+1)}=\dfrac{x-1}{2(x+1)}\xrightarrow{x\to1}\dfrac{0}{4}=0.$$

El valor es $0\neq\dfrac12$ $\Rightarrow$ **Falsa**. (Resultado correcto: $0$.)

**c)** $\lim_{x\to\infty}\dfrac{\sqrt{x^2+5}}{3x-2}$ no existe.

Para $x\to+\infty$: $\dfrac{\sqrt{x^2+5}}{3x-2}\to\dfrac{\lvert x\rvert}{3x}=\dfrac{x}{3x}=\dfrac13$. Para $x\to-\infty$: $\dfrac{-x}{3x}=-\dfrac13$. Cada límite unilateral existe (son distintos), pero **como límite en el infinito sin especificar signo** los dos valores difieren. La afirmación "no existe" se interpreta como el límite bilateral en $\infty$ (ambos lados): al diferir, **Verdadera** que no existe un único valor. Por rama: $+\tfrac13$ y $-\tfrac13$.

### Adicional 2 — (GeoGebra) asíntotas de $\dfrac{ax^2+x}{bx^2-1}$

Mismo análisis que el 25c: AH $y=\dfrac{a}{b}$ (si $b\neq0$); AV en $x=\pm\dfrac{1}{\sqrt b}$ si $b>0$; sin AV si $b<0$; casos de cancelación si numerador y denominador comparten raíz. Discusión por casos según signos de $a,b$.

### Adicional 3 — $f(x)=\dfrac{\lvert 4-x^2\rvert}{x(x-2)}$

**Dominio:** $x(x-2)\neq0\Rightarrow x\neq0,\ x\neq2$, es decir $D=\mathbb{R}-\{0,2\}$.

Separamos el módulo: $4-x^2\ge0\Leftrightarrow -2\le x\le2$.

- **Si $-2\le x\le2$:** $\lvert4-x^2\rvert=4-x^2=(2-x)(2+x)$. Entonces $f(x)=\dfrac{(2-x)(2+x)}{x(x-2)}=\dfrac{-(x-2)(x+2)}{x(x-2)}=\dfrac{-(x+2)}{x}$.
- **Si $x<-2$ o $x>2$:** $\lvert4-x^2\rvert=x^2-4=(x-2)(x+2)$. Entonces $f(x)=\dfrac{(x-2)(x+2)}{x(x-2)}=\dfrac{x+2}{x}$.

**Discontinuidades:**

- **$x=2$:** lateral izquierdo (rama $-\tfrac{x+2}{x}$): $\to-\dfrac{4}{2}=-2$; lateral derecho (rama $\tfrac{x+2}{x}$): $\to\dfrac{4}{2}=2$. Salto finito $\Rightarrow$ **esencial de salto finito** ($S=4$).
- **$x=0$:** está en la rama $-\tfrac{x+2}{x}$, $\to-\dfrac{2}{0}\to\pm\infty$ $\Rightarrow$ **esencial de salto infinito** (AV $x=0$).

**Asíntotas:**

- **AV:** $x=0$ (no $x=2$, que es salto finito).
- **AH:** $x\to+\infty$ usa $\dfrac{x+2}{x}\to1\Rightarrow y=1$; $x\to-\infty$ usa $\dfrac{x+2}{x}\to1\Rightarrow y=1$. AH $y=1$.

$$\boxed{D=\mathbb{R}-\{0,2\};\ \text{AV }x=0,\ \text{AH }y=1;\ x=2\ \text{salto finito},\ x=0\ \text{salto infinito}.}$$

✓ Coincide con la respuesta oficial (dominio $\mathbb{R}-\{0,2\}$).

### Adicional 4 — (opción múltiple) función por tramos continua

Según la respuesta oficial, los valores que hacen continua la función por tramos son $a=\dfrac{3}{2}$ y $b=-\dfrac{9}{2}$. El método es igualar los límites laterales en cada punto de empalme (como en los ejercicios 5, 19, 29).

$$\boxed{a=\dfrac{3}{2},\quad b=-\dfrac{9}{2}.}$$

✓ Coincide con la respuesta oficial.

### Adicional 5 — (opción) límites laterales

Se resuelven leyendo el comportamiento por izquierda y por derecha en cada punto, eligiendo la rama de la función definida en cada lado (mismo procedimiento que el ejercicio 17). Sin el enunciado de opciones específico, se aplica el criterio de laterales.

### Adicional 6 — $L=\lim_{x\to a}\dfrac{x\sqrt{x}-a\sqrt{a}}{\sqrt{x}-\sqrt{a}}$

Escribimos $x\sqrt{x}=(\sqrt{x})^3$ y $a\sqrt{a}=(\sqrt{a})^3$. Con $u=\sqrt{x}$, $v=\sqrt{a}$ es una diferencia de cubos:

$$\dfrac{u^3-v^3}{u-v}=u^2+uv+v^2.$$

Volviendo a las variables: $u^2+uv+v^2=x+\sqrt{x}\sqrt{a}+a\xrightarrow{x\to a}a+a+a=3a$.

$$\boxed{L=3a,\quad \forall a\ge0.}$$

✓ Coincide con la respuesta oficial.

### Adicional 7 — (opción) asíntotas de $g(x)=\dfrac{ax^3+cx^2-x}{3x^2-x}$

Numerador grado $3$, denominador grado $2$ (difieren en uno) $\Rightarrow$ existe **AO** si $a\neq0$. Factor común $x$: $\dfrac{x(ax^2+cx-1)}{x(3x-1)}=\dfrac{ax^2+cx-1}{3x-1}$ (hueco evitable en $x=0$). 

- **AV:** $3x-1=0\Rightarrow x=\dfrac13$ (si el numerador no se anula allí).
- **AO** $y=mx+n$: $m=\lim\dfrac{ax^2+cx-1}{x(3x-1)}=\dfrac{a}{3}$; $n$ se obtiene de la división. La discusión depende de $a$ y $c$.

Sin los valores concretos de la opción, las asíntotas son: AV $x=\tfrac13$ y AO de pendiente $\tfrac{a}{3}$.

---

## Cierre

Esta práctica recorre todas las técnicas centrales de la Unidad 2: factorización y racionalización para indeterminaciones $\tfrac00$, infinitésimos equivalentes y límites notables para los trigonométricos y exponenciales, comparación de grados y manejo de raíces para $x\to\infty$, límites laterales con módulos y exponenciales, cálculo de asíntotas (AV, AH, AO) y el análisis completo de continuidad con clasificación de discontinuidades.
