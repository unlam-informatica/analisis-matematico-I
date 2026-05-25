---
layout: default
title: Teoría — Unidad 4
parent: Unidad 4 — Polinomios de Taylor
permalink: /unidad-4/teoria/unidad-4
nav_order: 1
---

# Unidad 4 — Polinomios de Taylor

{: .no_toc }

## Tabla de contenidos
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## 1. Órdenes de contacto entre dos curvas

Dos funciones f y g tienen **contacto de orden n** en x = a si:

f(a) = g(a),  f′(a) = g′(a),  …,  f⁽ⁿ⁾(a) = g⁽ⁿ⁾(a)

pero f⁽ⁿ⁺¹⁾(a) ≠ g⁽ⁿ⁺¹⁾(a).

**Equivalentemente:** lim [f(x) − g(x)] / (x − a)ⁿ = 0  y  lim [f(x) − g(x)] / (x − a)ⁿ⁺¹ ≠ 0

Cuanto mayor el orden de contacto, mejor se "ajustan" las dos curvas cerca de x = a.

---

## 2. Expresión de un polinomio por sus derivadas

Un polinomio P(x) de grado n puede escribirse en función de sus derivadas en x = a:

P(x) = P(a) + P′(a)(x−a) + P″(a)/2! · (x−a)² + … + P⁽ⁿ⁾(a)/n! · (x−a)ⁿ

Esta es la base de la construcción del polinomio de Taylor.

---

## 3. Polinomio de Taylor

El **polinomio de Taylor de orden n de f en x = a** es el único polinomio de grado ≤ n que tiene contacto de orden n con f en x = a:

$$P_n(x) = \sum_{k=0}^{n} \frac{f^{(k)}(a)}{k!}(x-a)^k$$

$$P_n(x) = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^2 + \cdots + \frac{f^{(n)}(a)}{n!}(x-a)^n$$

**Requisito:** f debe ser n veces derivable en x = a.

### Polinomios de Taylor de funciones comunes (en x = 0, Maclaurin)

| Función | Polinomio de Taylor en 0 de orden n |
|---------|--------------------------------------|
| eˣ | 1 + x + x²/2! + x³/3! + … + xⁿ/n! |
| sen(x) | x − x³/3! + x⁵/5! − … |
| cos(x) | 1 − x²/2! + x⁴/4! − … |
| ln(1+x) | x − x²/2 + x³/3 − … |
| 1/(1−x) | 1 + x + x² + x³ + … + xⁿ |
| (1+x)ᵅ | 1 + αx + α(α−1)/2! x² + … |

---

## 4. Polinomio de Maclaurin

Es el caso particular de Taylor con **a = 0**:

$$P_n(x) = f(0) + f'(0)x + \frac{f''(0)}{2!}x^2 + \cdots + \frac{f^{(n)}(0)}{n!}x^n$$

---

## 5. Aproximación lineal

El polinomio de Taylor de **orden 1** en x = a:

P₁(x) = f(a) + f′(a)(x − a)

Es la **recta tangente** a f en x = a. Constituye la mejor aproximación lineal de f cerca de ese punto.

**Uso práctico:** para x ≈ a, se puede aproximar f(x) ≈ f(a) + f′(a)(x − a).

Ejemplos útiles para x ≈ 0:
- (1 + x)ᵅ ≈ 1 + αx
- eˣ ≈ 1 + x
- ln(1 + x) ≈ x
- sen(x) ≈ x
- cos(x) ≈ 1

---

## 6. Término complementario (resto de Taylor)

La diferencia entre f(x) y su polinomio de Taylor Pₙ(x) se llama **resto** o **término complementario**:

Rₙ(x) = f(x) − Pₙ(x)

### Forma de Lagrange (resto de Lagrange)

Si f es (n+1) veces derivable en un intervalo que contiene a a y x, existe c entre a y x tal que:

$$R_n(x) = \frac{f^{(n+1)}(c)}{(n+1)!}(x-a)^{n+1}$$

### Estimación del error

Para acotar el error de aproximación:

|Rₙ(x)| ≤ M/(n+1)! · |x − a|^(n+1)

donde M es una cota de |f⁽ⁿ⁺¹⁾| en el intervalo considerado.

**Uso:** dado un error máximo tolerable ε, se puede determinar qué orden n de polinomio es suficiente para garantizar |Rₙ(x)| < ε.
