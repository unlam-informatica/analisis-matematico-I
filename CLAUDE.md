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
- **Practica files** (`practica/`): exercises with commented solutions or step-by-step hints.

## Units and syllabus

| Unidad | Topic | Parcial |
|--------|-------|---------|
| 1 | Funciones: definición, dominio, imagen, transformaciones, función inversa | 1er parcial |
| 2 | Límite funcional, infinitésimos, asíntotas, continuidad, discontinuidades | 1er (límites) y 2do (continuidad) |
| 3 | Derivada: definición, reglas, cadena, implícita, derivación logarítmica | 2do parcial |
| 4 | Polinomios de Taylor y Maclaurin, aproximación lineal, resto | 2do parcial |

## GitHub Pages config

- Theme: `just-the-docs/just-the-docs` (via `remote_theme`)
- URL: `https://unlam-informatica.github.io/analisis-matematico-I`
- Color scheme: dark
