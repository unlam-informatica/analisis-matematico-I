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

Una **función** f de un conjunto A en un conjunto B es una regla que asigna a cada elemento x ∈ A exactamente un elemento y ∈ B.

Se escribe: f : A → B, y = f(x)

- **Dominio (Dom f):** conjunto A — todos los valores de entrada válidos.
- **Codominio:** conjunto B.
- **Imagen (Im f):** subconjunto de B que contiene todos los valores efectivamente alcanzados por f.

### Formas de representar una función

| Representación | Descripción |
|----------------|-------------|
| Algebraica | Fórmula matemática: f(x) = x² + 1 |
| Tabular | Tabla de pares (x, f(x)) |
| Gráfica | Curva en el plano cartesiano |
| Verbal | Descripción en palabras |

---

## 2. Funciones como modelos

Las funciones permiten modelar situaciones reales: costos, poblaciones, movimiento, temperatura, etc. El dominio se restringe al contexto del problema (dominio natural o dominio práctico).

---

## 3. Ceros y signo de una función

- **Ceros (raíces):** valores de x tales que f(x) = 0.
- **Signo:** análisis de los intervalos donde f(x) > 0 (positiva) o f(x) < 0 (negativa).

**Método:** encontrar los ceros, luego evaluar el signo en cada intervalo resultante.

---

## 4. Funciones par e impar

| Tipo | Condición | Simetría gráfica |
|------|-----------|-----------------|
| Par | f(−x) = f(x) para todo x en el dominio | Respecto al eje y |
| Impar | f(−x) = −f(x) para todo x en el dominio | Respecto al origen |

> El dominio debe ser simétrico respecto al origen para que la clasificación tenga sentido.

---

## 5. Funciones algebraicas

### 5.1 Funciones polinomiales

f(x) = aₙxⁿ + aₙ₋₁xⁿ⁻¹ + … + a₁x + a₀

- Dominio: ℝ
- Continuas en todo ℝ

### 5.2 Funciones racionales

f(x) = P(x) / Q(x), con P y Q polinomios.

- Dominio: ℝ − {x : Q(x) = 0}

### 5.3 Funciones irracionales (con raíces)

f(x) = ⁿ√g(x)

- Para n par: dominio condicionado por g(x) ≥ 0.
- Para n impar: dominio = ℝ (donde g esté definida).

---

## 6. Funciones trascendentes

### 6.1 Función exponencial

f(x) = aˣ, a > 0, a ≠ 1

- Dominio: ℝ
- Imagen: (0, +∞)
- Caso más común: f(x) = eˣ

### 6.2 Función logarítmica

f(x) = logₐ(x), a > 0, a ≠ 1

- Dominio: (0, +∞)
- Imagen: ℝ
- Es la inversa de la exponencial.

### 6.3 Funciones trigonométricas

| Función | Dominio | Imagen |
|---------|---------|--------|
| sen(x) | ℝ | [−1, 1] |
| cos(x) | ℝ | [−1, 1] |
| tan(x) | ℝ − {π/2 + kπ} | ℝ |
| cot(x) | ℝ − {kπ} | ℝ |
| sec(x) | ℝ − {π/2 + kπ} | (−∞,−1] ∪ [1,+∞) |
| csc(x) | ℝ − {kπ} | (−∞,−1] ∪ [1,+∞) |

### 6.4 Funciones trigonométricas inversas

| Función | Dominio | Imagen |
|---------|---------|--------|
| arcsen(x) | [−1, 1] | [−π/2, π/2] |
| arccos(x) | [−1, 1] | [0, π] |
| arctan(x) | ℝ | (−π/2, π/2) |

---

## 7. Función acotada

Una función f está **acotada superiormente** si existe M tal que f(x) ≤ M para todo x en el dominio.
Está **acotada inferiormente** si existe m tal que f(x) ≥ m.
Está **acotada** si está acotada superior e inferiormente.

---

## 8. Álgebra de funciones

Dadas f y g con dominios Df y Dg:

| Operación | Definición | Dominio |
|-----------|------------|---------|
| (f + g)(x) | f(x) + g(x) | Df ∩ Dg |
| (f − g)(x) | f(x) − g(x) | Df ∩ Dg |
| (f · g)(x) | f(x) · g(x) | Df ∩ Dg |
| (f/g)(x) | f(x) / g(x) | Df ∩ Dg − {x : g(x) = 0} |
| (f ∘ g)(x) | f(g(x)) | {x ∈ Dg : g(x) ∈ Df} |

---

## 9. Transformaciones de funciones

A partir de y = f(x):

| Transformación | Fórmula |
|----------------|---------|
| Desplazamiento vertical (↑ c) | y = f(x) + c |
| Desplazamiento vertical (↓ c) | y = f(x) − c |
| Desplazamiento horizontal (→ c) | y = f(x − c) |
| Desplazamiento horizontal (← c) | y = f(x + c) |
| Alargamiento vertical | y = c·f(x), c > 1 |
| Contracción vertical | y = c·f(x), 0 < c < 1 |
| Reflexión respecto al eje x | y = −f(x) |
| Reflexión respecto al eje y | y = f(−x) |
| Alargamiento/contracción horizontal | y = f(c·x) |

---

## 10. Funciones biyectivas

- **Inyectiva (uno a uno):** x₁ ≠ x₂ ⟹ f(x₁) ≠ f(x₂). Equivalente: si f(x₁) = f(x₂) entonces x₁ = x₂.
- **Sobreyectiva (sobre):** Im f = codominio. Todo y del codominio tiene al menos una preimagen.
- **Biyectiva:** inyectiva y sobreyectiva. Condición necesaria para que exista la función inversa.

**Test de la recta horizontal:** f es inyectiva si y solo si toda recta horizontal corta a la gráfica en a lo sumo un punto.

---

## 11. Función inversa

Si f : A → B es biyectiva, existe f⁻¹ : B → A tal que:

f⁻¹(f(x)) = x  para todo x ∈ A  
f(f⁻¹(y)) = y  para todo y ∈ B

**Para calcular f⁻¹:**
1. Escribir y = f(x).
2. Despejar x en función de y.
3. Intercambiar x e y.

**Propiedad gráfica:** la gráfica de f⁻¹ es el simétrico de la gráfica de f respecto a la recta y = x.
