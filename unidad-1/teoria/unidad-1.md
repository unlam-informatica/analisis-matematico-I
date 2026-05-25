---
layout: default
title: Teoría — Unidad 1
parent: Unidad 1 — Funciones
permalink: /unidad-1/teoria/unidad-1
nav_order: 1
---

# Unidad 1 — Funciones

{: .no_toc }

## Tabla de contenidos
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## 1. Definición de función

Una **función** $f$ de un conjunto $A$ en un conjunto $B$ es una regla que asigna a cada elemento $x \in A$ exactamente un elemento $y \in B$.

$$f : A \to B \qquad y = f(x)$$

- **Dominio** $(\text{Dom}\, f)$: conjunto $A$ — todos los valores de entrada válidos.
- **Codominio**: conjunto $B$.
- **Imagen** $(\text{Im}\, f)$: subconjunto de $B$ que contiene todos los valores efectivamente alcanzados por $f$.

### Formas de representar una función

| Representación | Descripción |
|----------------|-------------|
| Algebraica | Fórmula matemática: $f(x) = x^2 + 1$ |
| Tabular | Tabla de pares $(x,\, f(x))$ |
| Gráfica | Curva en el plano cartesiano |
| Verbal | Descripción en palabras |

---

## 2. Funciones como modelos

Las funciones permiten modelar situaciones reales: costos, poblaciones, movimiento, temperatura, etc. El dominio se restringe al contexto del problema (dominio natural o dominio práctico).

---

## 3. Ceros y signo de una función

- **Ceros (raíces):** valores de $x$ tales que $f(x) = 0$.
- **Signo:** análisis de los intervalos donde $f(x) > 0$ (positiva) o $f(x) < 0$ (negativa).

**Método:** encontrar los ceros, luego evaluar el signo en cada intervalo resultante.

---

## 4. Funciones par e impar

| Tipo | Condición | Simetría gráfica |
|------|-----------|-----------------|
| Par | $f(-x) = f(x)$ para todo $x$ en el dominio | Respecto al eje $y$ |
| Impar | $f(-x) = -f(x)$ para todo $x$ en el dominio | Respecto al origen |

> El dominio debe ser simétrico respecto al origen para que la clasificación tenga sentido.

---

## 5. Funciones algebraicas

### 5.1 Funciones polinomiales

$$f(x) = a_n x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0$$

- Dominio: $\mathbb{R}$
- Continuas en todo $\mathbb{R}$

### 5.2 Funciones racionales

$$f(x) = \frac{P(x)}{Q(x)}, \quad \text{con } P \text{ y } Q \text{ polinomios.}$$

- Dominio: $\mathbb{R} \setminus \{x : Q(x) = 0\}$

### 5.3 Funciones irracionales (con raíces)

$$f(x) = \sqrt[n]{g(x)}$$

- Para $n$ par: dominio condicionado por $g(x) \geq 0$.
- Para $n$ impar: dominio $= \mathbb{R}$ (donde $g$ esté definida).

---

## 6. Funciones trascendentes

### 6.1 Función exponencial

$$f(x) = a^x, \quad a > 0,\ a \neq 1$$

- Dominio: $\mathbb{R}$
- Imagen: $(0, +\infty)$
- Caso más común: $f(x) = e^x$

### 6.2 Función logarítmica

$$f(x) = \log_a(x), \quad a > 0,\ a \neq 1$$

- Dominio: $(0, +\infty)$
- Imagen: $\mathbb{R}$
- Es la inversa de la exponencial.

### 6.3 Funciones trigonométricas

| Función | Dominio | Imagen |
|---------|---------|--------|
| $\sin(x)$ | $\mathbb{R}$ | $[-1,\, 1]$ |
| $\cos(x)$ | $\mathbb{R}$ | $[-1,\, 1]$ |
| $\tan(x)$ | $\mathbb{R} \setminus \{\frac{\pi}{2} + k\pi\}$ | $\mathbb{R}$ |
| $\cot(x)$ | $\mathbb{R} \setminus \{k\pi\}$ | $\mathbb{R}$ |
| $\sec(x)$ | $\mathbb{R} \setminus \{\frac{\pi}{2} + k\pi\}$ | $(-\infty,-1] \cup [1,+\infty)$ |
| $\csc(x)$ | $\mathbb{R} \setminus \{k\pi\}$ | $(-\infty,-1] \cup [1,+\infty)$ |

### 6.4 Funciones trigonométricas inversas

| Función | Dominio | Imagen |
|---------|---------|--------|
| $\arcsin(x)$ | $[-1,\, 1]$ | $\left[-\dfrac{\pi}{2},\, \dfrac{\pi}{2}\right]$ |
| $\arccos(x)$ | $[-1,\, 1]$ | $[0,\, \pi]$ |
| $\arctan(x)$ | $\mathbb{R}$ | $\left(-\dfrac{\pi}{2},\, \dfrac{\pi}{2}\right)$ |

---

## 7. Función acotada

Una función $f$ está **acotada superiormente** si existe $M$ tal que $f(x) \leq M$ para todo $x$ en el dominio.
Está **acotada inferiormente** si existe $m$ tal que $f(x) \geq m$.
Está **acotada** si está acotada superior e inferiormente.

---

## 8. Álgebra de funciones

Dadas $f$ y $g$ con dominios $D_f$ y $D_g$:

| Operación | Definición | Dominio |
|-----------|------------|---------|
| $(f + g)(x)$ | $f(x) + g(x)$ | $D_f \cap D_g$ |
| $(f - g)(x)$ | $f(x) - g(x)$ | $D_f \cap D_g$ |
| $(f \cdot g)(x)$ | $f(x) \cdot g(x)$ | $D_f \cap D_g$ |
| $\left(\dfrac{f}{g}\right)(x)$ | $\dfrac{f(x)}{g(x)}$ | $D_f \cap D_g \setminus \{x : g(x) = 0\}$ |
| $(f \circ g)(x)$ | $f(g(x))$ | $\{x \in D_g : g(x) \in D_f\}$ |

---

## 9. Transformaciones de funciones

A partir de $y = f(x)$:

| Transformación | Fórmula |
|----------------|---------|
| Desplazamiento vertical (↑ $c$) | $y = f(x) + c$ |
| Desplazamiento vertical (↓ $c$) | $y = f(x) - c$ |
| Desplazamiento horizontal (→ $c$) | $y = f(x - c)$ |
| Desplazamiento horizontal (← $c$) | $y = f(x + c)$ |
| Alargamiento vertical | $y = c \cdot f(x)$, $c > 1$ |
| Contracción vertical | $y = c \cdot f(x)$, $0 < c < 1$ |
| Reflexión respecto al eje $x$ | $y = -f(x)$ |
| Reflexión respecto al eje $y$ | $y = f(-x)$ |
| Alargamiento/contracción horizontal | $y = f(c \cdot x)$ |

---

## 10. Funciones biyectivas

- **Inyectiva (uno a uno):** $x_1 \neq x_2 \implies f(x_1) \neq f(x_2)$. Equivalente: $f(x_1) = f(x_2) \implies x_1 = x_2$.
- **Sobreyectiva (sobre):** $\text{Im}\, f = \text{codominio}$. Todo $y$ del codominio tiene al menos una preimagen.
- **Biyectiva:** inyectiva y sobreyectiva. Condición necesaria para que exista la función inversa.

**Test de la recta horizontal:** $f$ es inyectiva si y solo si toda recta horizontal corta a la gráfica en a lo sumo un punto.

---

## 11. Función inversa

Si $f : A \to B$ es biyectiva, existe $f^{-1} : B \to A$ tal que:

$$f^{-1}(f(x)) = x \quad \forall\, x \in A$$

$$f(f^{-1}(y)) = y \quad \forall\, y \in B$$

**Para calcular $f^{-1}$:**
1. Escribir $y = f(x)$.
2. Despejar $x$ en función de $y$.
3. Intercambiar $x$ e $y$.

**Propiedad gráfica:** la gráfica de $f^{-1}$ es el simétrico de la gráfica de $f$ respecto a la recta $y = x$.
