---
layout: default
title: Teoría — Unidad 3
parent: Unidad 3 — Derivada
permalink: /unidad-3/teoria/unidad-3
nav_order: 1
---

# Unidad 3 — Derivada

{: .no_toc }

## Tabla de contenidos
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## 1. Razón de cambio media

La **razón de cambio media** de f en el intervalo [x₀, x₀ + h] es:

Δf/Δx = [f(x₀ + h) − f(x₀)] / h

Geométricamente: pendiente de la **recta secante** que pasa por (x₀, f(x₀)) y (x₀+h, f(x₀+h)).

---

## 2. Derivada en un punto — razón de cambio instantánea

La **derivada de f en x₀** es el límite de la razón de cambio media cuando h → 0:

f′(x₀) = lim [f(x₀ + h) − f(x₀)] / h  [h → 0]

Si este límite existe (y es finito), f es **derivable en x₀**.

### Significado geométrico

f′(x₀) es la **pendiente de la recta tangente** a la gráfica de f en el punto (x₀, f(x₀)).

### Significado físico

Si f(t) es la posición de un objeto en el instante t, entonces f′(t₀) es la **velocidad instantánea** en t₀.

---

## 3. La derivada como función

La **función derivada** f′ : Dom f′ → ℝ asigna a cada x el valor f′(x).

Notaciones equivalentes:

f′(x) = df/dx = y′ = Df(x) = d/dx[f(x)]

---

## 4. Recta tangente y recta normal

**Recta tangente** en (x₀, f(x₀)):  
y − f(x₀) = f′(x₀) · (x − x₀)

**Recta normal** (perpendicular a la tangente) en (x₀, f(x₀)):  
y − f(x₀) = −1/f′(x₀) · (x − x₀)  [si f′(x₀) ≠ 0]

---

## 5. Derivadas laterales

- **Derivada por la derecha:** f′₊(x₀) = lim [f(x₀+h)−f(x₀)]/h  [h → 0⁺]
- **Derivada por la izquierda:** f′₋(x₀) = lim [f(x₀+h)−f(x₀)]/h  [h → 0⁻]

f es derivable en x₀  ⟺  f′₊(x₀) = f′₋(x₀) = f′(x₀)

---

## 6. Continuidad y derivabilidad

**Teorema:** Si f es derivable en x₀, entonces f es continua en x₀.

**El recíproco es falso:** f puede ser continua en x₀ sin ser derivable. Ejemplo: f(x) = |x| en x = 0.

---

## 7. Derivadas de funciones elementales

| Función f(x) | Derivada f′(x) |
|--------------|----------------|
| c (constante) | 0 |
| xⁿ | n·xⁿ⁻¹ |
| √x | 1/(2√x) |
| eˣ | eˣ |
| aˣ | aˣ·ln(a) |
| ln(x) | 1/x |
| logₐ(x) | 1/(x·ln a) |
| sen(x) | cos(x) |
| cos(x) | −sen(x) |
| tan(x) | sec²(x) = 1/cos²(x) |
| cot(x) | −csc²(x) = −1/sen²(x) |
| arcsen(x) | 1/√(1−x²) |
| arccos(x) | −1/√(1−x²) |
| arctan(x) | 1/(1+x²) |

---

## 8. Reglas de derivación

Sean f y g derivables y c una constante:

| Regla | Fórmula |
|-------|---------|
| Constante por función | (c·f)′ = c·f′ |
| Suma | (f + g)′ = f′ + g′ |
| Diferencia | (f − g)′ = f′ − g′ |
| Producto | (f · g)′ = f′·g + f·g′ |
| Cociente | (f/g)′ = (f′·g − f·g′) / g² |

---

## 9. Regla de la cadena (composición)

Si h(x) = f(g(x)), entonces:

h′(x) = f′(g(x)) · g′(x)

**Notación de Leibniz:** dy/dx = (dy/du) · (du/dx)

**Ejemplo:** si h(x) = sen(x²), entonces:  
h′(x) = cos(x²) · 2x

---

## 10. Derivada de la función inversa

Si f es biyectiva y derivable, y f⁻¹ es su inversa:

(f⁻¹)′(y) = 1 / f′(f⁻¹(y))

Equivalentemente: dx/dy = 1 / (dy/dx)

---

## 11. Derivada de funciones definidas implícitamente

Cuando y no se puede despejar explícitamente de F(x, y) = 0:

1. Derivar ambos lados respecto a x (usando la regla de la cadena para los términos con y, tratando y como función de x).
2. Despejar dy/dx.

**Ejemplo:** x² + y² = 1  →  2x + 2y·(dy/dx) = 0  →  dy/dx = −x/y

---

## 12. Derivación logarítmica

Técnica útil para funciones del tipo f(x) = [u(x)]^v(x) o productos/cocientes complejos.

**Procedimiento:**
1. Tomar logaritmo natural: ln y = v(x)·ln(u(x))
2. Derivar implícitamente: y′/y = …
3. Despejar y′ = y · (…)

**Ejemplo:** y = xˢᵉⁿ⁽ˣ⁾

ln y = sen(x) · ln(x)  
y′/y = cos(x)·ln(x) + sen(x)/x  
y′ = xˢᵉⁿ⁽ˣ⁾ · [cos(x)·ln(x) + sen(x)/x]
