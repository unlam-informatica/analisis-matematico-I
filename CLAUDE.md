# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

Study notes, guides, and practice exercises for the "Análisis Matemático I" course at UNLaM. Published as a GitHub Pages site using the `just-the-docs` Jekyll theme (`_config.yml`). GitHub Pages builds and deploys automatically on push — no local build step needed.

## Repository structure

Each unit follows the same internal layout:

```
unidad-N/
├── index.md         # Unit overview with topic table and links
├── teoria/          # Full unit summary in Markdown
├── guias/           # Focused reference guides on specific topics
├── practica/        # Exercise files (Markdown or plain text)
└── images/          # Images referenced from the Markdown files
```

Units are:
- **Unidad 1:** Funciones
- **Unidad 2:** Límite funcional y Continuidad
- **Unidad 3:** Derivada
- **Unidad 4:** Polinomios de Taylor

## Content conventions

- **Language**: All content is written in Spanish.
- **Math notation**: Use LaTeX-style notation inline (e.g., f′(x), lim, ∞) or fenced with `$$…$$` for block equations (just-the-docs supports MathJax if enabled, otherwise use Unicode).
- **Markdown**: GitHub-flavored Markdown. Tables, fenced code blocks with language tags, and heading-based `#` anchors are used throughout.
- **Front matter**: All pages must have at minimum `layout: default`, `title`, `parent` (for subpages), and `permalink`. The root `index.md` uses `layout: home`.
- **Navigation**: The `just-the-docs` theme uses `nav_order`, `has_children: true` (on parent pages), and `parent: <Title>` (on child pages) to build the sidebar.
- **Guides** (`guias/`): self-contained reference documents covering a single specific topic with examples.
- **Teoria files** (`teoria/`): comprehensive unit summaries covering all topics in the syllabus. Include a TOC block at the top.
- **Practica files** (`practica/`): exercises with commented solutions or step-by-step hints. See the format below.

## Practica exercise format

Practice exercises must follow this exact structure so the site stays consistent. The two callouts (`enunciado`, `resolucion`) are configured in `_config.yml` and styled by `_sass/custom/setup.scss` (amber for statement, teal for solution).

**Per-exercise template:**

```markdown
### `1d`

{: .enunciado }
> Enunciado textual del ejercicio, copiado o reescrito de forma natural.

{: .resolucion }
> Texto explicativo introduciendo el primer paso.
>
> $$\text{ecuación o expresión}$$
>
> Conector que explica qué se hizo y qué sigue.
>
> $$\text{siguiente paso}$$
>
> ... (repetir tantos pasos como sea necesario)
>
> **Resultado:** expresión final con dominio e imagen cuando corresponda.
>
> **Verificación:** Coincide con la respuesta indicada en la guía.
```

**Source of truth para enunciados:** la guía oficial está en `reference/practica.pdf`. El enunciado **debe copiarse literalmente** de ese PDF, sin reescribirlo, resumirlo ni "naturalizarlo". Conservar la redacción, signos de puntuación, mayúsculas, paréntesis y notación matemática tal cual aparecen. Solo se permite traducir notación inline a LaTeX (`$…$`) cuando el PDF muestra fórmulas que en Markdown necesitan ese delimitador. Si el enunciado del PDF es ambiguo o contiene un error, no corregir en silencio: dejar el texto original y aclarar la interpretación en la resolución.

**Reglas que aplican siempre:**

- El heading del ejercicio es `### \`Nx\`` (solo la numeración entre backticks; sin descripción al lado).
- El enunciado va en un callout `{: .enunciado }` con una sola línea de blockquote `>`, **copiado textual del PDF**. Si el enunciado tiene varios renglones, prefijar cada uno con `>`.
- La resolución va en un callout `{: .resolucion }` y **todas** las líneas (texto, ecuaciones en bloque, líneas vacías de separación) deben empezar con `>` para no romper el blockquote.
- Cada paso del desarrollo se presenta como: oración explicativa → `$$ecuación$$` en bloque. Evitar amontonar varias igualdades en una sola línea; separar en pasos cortos legibles.
- Usar `\dfrac` (no `\frac`) para fracciones que aparezcan en displays.
- Cerrar siempre con dos líneas en negrita: `**Resultado:**` (la respuesta final, dominio e imagen cuando aplique) y `**Verificación:**` (confirmación contra la guía oficial).
- No usar emojis tipo ✓/✗; usar las líneas de verificación en negrita.
- Para definiciones por casos dentro de un callout, `\begin{cases}…\end{cases}` debe ir en **una sola línea** dentro de `$$…$$` (todo el `\begin…\end` en el mismo renglón, separando ramas con `\\`). Saltos de línea reales dentro del entorno rompen el blockquote del callout.
- **Nunca usar `|…|` con pipes crudos en una línea de blockquote** (callout): Kramdown los interpreta como separadores de columna de tabla y rompe el render. Para valor absoluto, normas, etc., usar siempre `\lvert … \rvert` (o `\vert`). Esto vale tanto en el enunciado como en cualquier ecuación inline o display dentro del callout.

**Agrupación por consigna:** los ejercicios de una misma consigna (por ejemplo "Graficar, indicar dominio e imagen") van bajo un único `## Ejercicio N — …`, y cada inciso `Na`, `Nb`, … usa el template de arriba.

## Units and syllabus

| Unidad | Topic | Parcial |
|--------|-------|---------|
| 1 | Funciones: definición, dominio, imagen, transformaciones, función inversa | 1er parcial |
| 2 | Límite funcional, infinitésimos, asíntotas, continuidad, discontinuidades | 1er (límites) y 2do (continuidad) |
| 3 | Derivada: definición, reglas, cadena, implícita, derivación logarítmica | 2do parcial |
| 4 | Polinomios de Taylor y Maclaurin, aproximación lineal, resto | 2do parcial |

## GitHub Pages config

- Theme: `just-the-docs/just-the-docs` (via `remote_theme`)
- URL: `https://unlam-informatica.github.io/analisis-matematico-i`
- Color scheme: dark
