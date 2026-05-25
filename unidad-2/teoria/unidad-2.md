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

La **distancia** entre dos números reales a y b es |a − b|.

- **Entorno de centro a y radio δ:** V(a, δ) = (a − δ, a + δ) = {x ∈ ℝ : |x − a| < δ}
- **Entorno reducido (perforado):** V*(a, δ) = V(a, δ) − {a} = {x ∈ ℝ : 0 < |x − a| < δ}

---

## 2. Límite finito

### Definición (ε-δ)

lim f(x) = L  [cuando x → a]

si para todo ε > 0 existe δ > 0 tal que:  
0 < |x − a| < δ  ⟹  |f(x) − L| < ε

> El valor de f en x = a (si existe) **no importa** para la definición del límite.

### Interpretación gráfica

Cuando x se aproxima a a (por cualquier lado), f(x) se aproxima a L.

---

## 3. Límites laterales

- **Límite por la derecha:** lim f(x) = L⁺  [x → a⁺]
- **Límite por la izquierda:** lim f(x) = L⁻  [x → a⁻]

**Teorema:** lim f(x) = L  ⟺  lim f(x) = L⁺ = L⁻  [x → a, a⁺, a⁻ respectivamente]

---

## 4. Unicidad del límite

Si lim f(x) existe, es **único**.

**Consecuencia:** si los límites laterales son distintos, el límite global no existe.

---

## 5. Propiedades del límite (álgebra de límites)

Sean lim f(x) = L y lim g(x) = M (ambos cuando x → a). Entonces:

| Propiedad | Resultado |
|-----------|-----------|
| Suma | lim [f(x) + g(x)] = L + M |
| Diferencia | lim [f(x) − g(x)] = L − M |
| Producto | lim [f(x) · g(x)] = L · M |
| Cociente | lim [f(x)/g(x)] = L/M, si M ≠ 0 |
| Potencia | lim [f(x)]ⁿ = Lⁿ |
| Raíz | lim ⁿ√f(x) = ⁿ√L, si aplica |
| Constante | lim c = c |
| Identidad | lim x = a |

---

## 6. Teorema de intercalación (Sandwich)

Si g(x) ≤ f(x) ≤ h(x) en un entorno reducido de a, y  
lim g(x) = lim h(x) = L  [x → a]

entonces: lim f(x) = L  [x → a]

**Aplicación típica:** lim [sen(x)/x] = 1  [x → 0]

---

## 7. Infinitésimos

Una función α(x) es un **infinitésimo** cuando x → a si lim α(x) = 0.

### Álgebra de infinitésimos

- Suma de infinitésimos: infinitésimo.
- Producto de infinitésimo por función acotada: infinitésimo.

### Comparación de infinitésimos

Sean α y β infinitésimos cuando x → a:

| Caso | Nombre |
|------|--------|
| lim α/β = L ≠ 0 | α y β son del mismo orden |
| lim α/β = 0 | α es de orden superior a β (α = o(β)) |
| lim α/β = ∞ | α es de orden inferior a β |
| lim α/βᵏ = L ≠ 0 | α es de orden k respecto a β |

**Infinitésimos equivalentes (∼):** lim α/β = 1. Se pueden sustituir en productos/cocientes.

Equivalencias fundamentales cuando x → 0:
- sen(x) ∼ x
- tan(x) ∼ x
- 1 − cos(x) ∼ x²/2
- ln(1 + x) ∼ x
- eˣ − 1 ∼ x

---

## 8. Límites infinitos

lim f(x) = +∞  [x → a]

si para todo M > 0 existe δ > 0 tal que:  
0 < |x − a| < δ  ⟹  f(x) > M

Análogamente para −∞.

---

## 9. Límites de variable infinita

lim f(x) = L  [x → +∞]

si para todo ε > 0 existe N tal que:  
x > N  ⟹  |f(x) − L| < ε

---

## 10. Cálculo de límites e indeterminaciones

### Formas indeterminadas

| Forma | Técnicas habituales |
|-------|---------------------|
| 0/0 | Factorizar, racionalizar, infinitésimos equivalentes, L'Hôpital (U3) |
| ∞/∞ | Dividir por la potencia dominante, L'Hôpital |
| 0 · ∞ | Reescribir como 0/0 o ∞/∞ |
| ∞ − ∞ | Factorizar, conjugado |
| 1^∞ | Usar e^[lim (f−1)·g] |
| 0^0 | Usar logaritmo |
| ∞^0 | Usar logaritmo |

### Límites notables

- lim [(1 + 1/n)ⁿ] = e  [n → ∞]
- lim [(1 + x)^(1/x)] = e  [x → 0]
- lim [sen(x)/x] = 1  [x → 0]
- lim [(eˣ − 1)/x] = 1  [x → 0]
- lim [ln(1 + x)/x] = 1  [x → 0]

---

## 11. Asíntotas

### Asíntota vertical (AV)

La recta x = a es AV si lim |f(x)| = ∞  [x → a⁺ o x → a⁻]

### Asíntota horizontal (AH)

La recta y = L es AH si lim f(x) = L  [x → +∞ o x → −∞]

### Asíntota oblicua (AO)

La recta y = mx + b es AO si:  
m = lim [f(x)/x]  y  b = lim [f(x) − mx]  [x → ±∞]

> Si existe AH, no hay AO (en esa misma dirección).

---

## 12. Continuidad

### Función continua en un punto

f es continua en x = a si se cumplen **las tres condiciones**:

1. f(a) existe (a ∈ Dom f).
2. lim f(x) existe  [x → a].
3. lim f(x) = f(a)  [x → a].

### Continuidad en intervalos

- **Intervalo abierto (a, b):** continua en cada punto interior.
- **Intervalo cerrado [a, b]:** continua en (a, b), con límite lateral derecho en a igual a f(a) y límite lateral izquierdo en b igual a f(b).

### Álgebra de funciones continuas

Si f y g son continuas en a, entonces f+g, f−g, f·g y f/g (si g(a)≠0) son continuas en a.

### Propiedades de funciones continuas en [a, b]

- **Teorema de Weierstrass:** f alcanza su máximo y mínimo absolutos.
- **Teorema del valor intermedio (TVI):** f toma todos los valores entre f(a) y f(b).
- **Corolario (existencia de raíces):** si f(a) y f(b) tienen signos opuestos, existe c ∈ (a, b) con f(c) = 0.

---

## 13. Clasificación de discontinuidades

Sea x = a un punto de discontinuidad de f:

| Tipo | Condición | Característica |
|------|-----------|----------------|
| **Evitable** | lim f(x) existe pero ≠ f(a) (o f(a) no existe) | Se puede "rellenar" el hueco |
| **De salto (1er especie)** | Los límites laterales existen pero son distintos | Salto finito en la gráfica |
| **Esencial (2da especie)** | Al menos un límite lateral no existe (o es ∞) | Comportamiento "explosivo" |
