---
layout: default
title: Teoría — Unidad 2
parent: Unidad 2 — Límite y Continuidad
permalink: /unidad-2/teoria/unidad-2
nav_order: 1
---

# Unidad 2 — Límite funcional y Continuidad

{: .no_toc }

## Tabla de contenidos
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## 1. Distancia y entorno

La **distancia** entre dos números reales $a$ y $b$ es $\lvert a - b \rvert$.

- **Entorno de centro $a$ y radio $\delta$:**

$$V(a, \delta) = (a - \delta,\; a + \delta) = \{x \in \mathbb{R} : \lvert x - a \rvert < \delta\}$$

- **Entorno reducido (perforado):**

$$\dot{V}(a, \delta) = V(a, \delta) \setminus \{a\} = \{x \in \mathbb{R} : 0 < \lvert x - a \rvert < \delta\}$$

---

## 2. Límite finito

### Definición ($\varepsilon$-$\delta$)

$$\lim_{x \to a} f(x) = L$$

si para todo $\varepsilon > 0$ existe $\delta > 0$ tal que:

$$0 < \lvert x - a \rvert < \delta \implies \lvert f(x) - L \rvert < \varepsilon$$

> El valor de $f$ en $x = a$ (si existe) **no importa** para la definición del límite.

### Interpretación gráfica

Cuando $x$ se aproxima a $a$ (por cualquier lado), $f(x)$ se aproxima a $L$.

---

## 3. Límites laterales

- **Límite por la derecha:** $\displaystyle\lim_{x \to a^+} f(x) = L^+$
- **Límite por la izquierda:** $\displaystyle\lim_{x \to a^-} f(x) = L^-$

**Teorema:**

$$\lim_{x \to a} f(x) = L \iff \lim_{x \to a^+} f(x) = \lim_{x \to a^-} f(x) = L$$

---

## 4. Unicidad del límite

Si $\displaystyle\lim_{x \to a} f(x)$ existe, es **único**.

**Consecuencia:** si los límites laterales son distintos, el límite global no existe.

---

## 5. Propiedades del límite (álgebra de límites)

Sean $\displaystyle\lim_{x \to a} f(x) = L$ y $\displaystyle\lim_{x \to a} g(x) = M$. Entonces:

| Propiedad | Resultado |
|-----------|-----------|
| Suma | $\displaystyle\lim_{x \to a}[f(x) + g(x)] = L + M$ |
| Diferencia | $\displaystyle\lim_{x \to a}[f(x) - g(x)] = L - M$ |
| Producto | $\displaystyle\lim_{x \to a}[f(x) \cdot g(x)] = L \cdot M$ |
| Cociente | $\displaystyle\lim_{x \to a}\frac{f(x)}{g(x)} = \frac{L}{M}$, si $M \neq 0$ |
| Potencia | $\displaystyle\lim_{x \to a}[f(x)]^n = L^n$ |
| Raíz | $\displaystyle\lim_{x \to a}\sqrt[n]{f(x)} = \sqrt[n]{L}$, si aplica |
| Constante | $\displaystyle\lim_{x \to a} c = c$ |
| Identidad | $\displaystyle\lim_{x \to a} x = a$ |

---

## 6. Teorema de intercalación (Sandwich)

Si $g(x) \leq f(x) \leq h(x)$ en un entorno reducido de $a$, y

$$\lim_{x \to a} g(x) = \lim_{x \to a} h(x) = L$$

entonces:

$$\lim_{x \to a} f(x) = L$$

**Aplicación típica:**

$$\lim_{x \to 0} \frac{\sin(x)}{x} = 1$$

---

## 7. Infinitésimos

Una función $\alpha(x)$ es un **infinitésimo** cuando $x \to a$ si $\displaystyle\lim_{x \to a} \alpha(x) = 0$.

### Álgebra de infinitésimos

- Suma de infinitésimos: infinitésimo.
- Producto de infinitésimo por función acotada: infinitésimo.

### Comparación de infinitésimos

Sean $\alpha$ y $\beta$ infinitésimos cuando $x \to a$:

| Caso | Nombre |
|------|--------|
| $\displaystyle\lim_{x \to a} \frac{\alpha}{\beta} = L \neq 0$ | $\alpha$ y $\beta$ son del mismo orden |
| $\displaystyle\lim_{x \to a} \frac{\alpha}{\beta} = 0$ | $\alpha$ es de orden superior a $\beta$ $\bigl(\alpha = o(\beta)\bigr)$ |
| $\displaystyle\lim_{x \to a} \frac{\alpha}{\beta} = \infty$ | $\alpha$ es de orden inferior a $\beta$ |
| $\displaystyle\lim_{x \to a} \frac{\alpha}{\beta^k} = L \neq 0$ | $\alpha$ es de orden $k$ respecto a $\beta$ |

**Infinitésimos equivalentes** ($\alpha \sim \beta$): $\displaystyle\lim_{x \to a} \frac{\alpha}{\beta} = 1$. Se pueden sustituir en productos/cocientes.

Equivalencias fundamentales cuando $x \to 0$:

$$\sin(x) \sim x \qquad \tan(x) \sim x \qquad 1 - \cos(x) \sim \frac{x^2}{2}$$

$$\ln(1 + x) \sim x \qquad e^x - 1 \sim x$$

---

## 8. Límites infinitos

$$\lim_{x \to a} f(x) = +\infty$$

si para todo $M > 0$ existe $\delta > 0$ tal que:

$$0 < \lvert x - a \rvert < \delta \implies f(x) > M$$

Análogamente para $-\infty$.

---

## 9. Límites de variable infinita

$$\lim_{x \to +\infty} f(x) = L$$

si para todo $\varepsilon > 0$ existe $N$ tal que:

$$x > N \implies \lvert f(x) - L \rvert < \varepsilon$$

---

## 10. Cálculo de límites e indeterminaciones

### Formas indeterminadas

| Forma | Técnicas habituales |
|-------|---------------------|
| $\dfrac{0}{0}$ | Factorizar, racionalizar, infinitésimos equivalentes, L'Hôpital (U3) |
| $\dfrac{\infty}{\infty}$ | Dividir por la potencia dominante, L'Hôpital |
| $0 \cdot \infty$ | Reescribir como $\dfrac{0}{0}$ o $\dfrac{\infty}{\infty}$ |
| $\infty - \infty$ | Factorizar, conjugado |
| $1^\infty$ | Usar $e^{\lim (f-1)\cdot g}$ |
| $0^0$ | Usar logaritmo |
| $\infty^0$ | Usar logaritmo |

### Límites notables

$$\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n = e \qquad \lim_{x \to 0} (1 + x)^{1/x} = e$$

$$\lim_{x \to 0} \frac{\sin(x)}{x} = 1 \qquad \lim_{x \to 0} \frac{e^x - 1}{x} = 1 \qquad \lim_{x \to 0} \frac{\ln(1+x)}{x} = 1$$

---

## 11. Asíntotas

### Asíntota vertical (AV)

La recta $x = a$ es AV si $\displaystyle\lim_{x \to a^+} f(x) = \pm\infty$ o $\displaystyle\lim_{x \to a^-} f(x) = \pm\infty$.

### Asíntota horizontal (AH)

La recta $y = L$ es AH si $\displaystyle\lim_{x \to +\infty} f(x) = L$ o $\displaystyle\lim_{x \to -\infty} f(x) = L$.

### Asíntota oblicua (AO)

La recta $y = mx + b$ es AO si:

$$m = \lim_{x \to \pm\infty} \frac{f(x)}{x} \qquad b = \lim_{x \to \pm\infty} \bigl[f(x) - mx\bigr]$$

> Si existe AH, no hay AO (en esa misma dirección).

---

## 12. Continuidad

### Función continua en un punto

$f$ es **continua en $x = a$** si se cumplen las tres condiciones:

1. $f(a)$ existe $\;(a \in \text{Dom}\, f)$.
2. $\displaystyle\lim_{x \to a} f(x)$ existe.
3. $\displaystyle\lim_{x \to a} f(x) = f(a)$.

### Continuidad en intervalos

- **Intervalo abierto $(a, b)$:** continua en cada punto interior.
- **Intervalo cerrado $[a, b]$:** continua en $(a, b)$, con $\displaystyle\lim_{x \to a^+} f(x) = f(a)$ y $\displaystyle\lim_{x \to b^-} f(x) = f(b)$.

### Álgebra de funciones continuas

Si $f$ y $g$ son continuas en $a$, entonces $f+g$, $f-g$, $f \cdot g$ y $\dfrac{f}{g}$ (si $g(a) \neq 0$) son continuas en $a$.

### Propiedades de funciones continuas en $[a, b]$

- **Teorema de Weierstrass:** $f$ alcanza su máximo y mínimo absolutos.
- **Teorema del valor intermedio (TVI):** $f$ toma todos los valores entre $f(a)$ y $f(b)$.
- **Corolario (existencia de raíces):** si $f(a) \cdot f(b) < 0$, existe $c \in (a, b)$ con $f(c) = 0$.

---

## 13. Clasificación de discontinuidades

Sea $x = a$ un punto de discontinuidad de $f$:

| Tipo | Condición | Característica |
|------|-----------|----------------|
| **Evitable** | $\displaystyle\lim_{x \to a} f(x)$ existe pero $\neq f(a)$ (o $f(a)$ no existe) | Se puede "rellenar" el hueco |
| **De salto (1ª especie)** | $\displaystyle\lim_{x \to a^+} f(x)$ y $\displaystyle\lim_{x \to a^-} f(x)$ existen pero son distintos | Salto finito en la gráfica |
| **Esencial (2ª especie)** | Al menos un límite lateral no existe o es $\pm\infty$ | Comportamiento "explosivo" |
