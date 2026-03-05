# deepwiki_skill

A `SKILL.md` that emulates **DeepWiki** functionality (similar to Google CodeWiki), designed to generate a navigable, documentation-style analysis of a repository.

Place it at:

```
.agent\skills\deepwiki\SKILL.md
```

## How to invoke

Ask Antigravity something like:

```
"Analyze this repo using the DeepWiki skill"
```

You can also trigger DeepWiki-style behavior by explicitly mentioning **DeepWiki**, for example:

- "Haz un análisis como DeepWiki"
- "DeepWiki-style repo analysis"

## New: Automatic HTML output (DeepWiki-style)

`SKILL.md` now includes explicit instructions to **automatically generate HTML** in these cases:

- When you ask for a **DeepWiki-style** analysis or you mention **"como DeepWiki"**
- When you request a **full repository analysis** (this is now the **default format**)
- When you ask to **"ver"** or **"navegar"** the documentation
- When you explicitly request **HTML output**

### HTML generation flow

1. Generate the analysis in **Markdown** (as before, including navigation, Mermaid diagrams, etc.).
2. Convert the Markdown to HTML using the template:
   - `deepwiki-template.html`
   - Fill the template placeholders with the real generated content.
3. Return a ready-to-open **`.html` file**.

### What the generated HTML includes

Each generated HTML file includes:

- A navigable **sidebar**
- A dynamic **table of contents (TOC)**
- **Mermaid** diagrams rendered in the browser
- **Syntax highlighting** for code blocks
- The full **DeepWiki dark theme** styling

## Contributing

Enhancements are welcome!