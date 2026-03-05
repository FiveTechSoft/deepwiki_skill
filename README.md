# DeepWiki

## New: Automatic HTML output (DeepWiki-style)

... (existing content)

### Generating HTML from DeepWiki Markdown files

To generate HTML output from a DeepWiki Markdown file, you can use the `md2html.js` script. Below are example commands:

```bash
# Basic command
node md2html.js path/to/your/deepwiki-file.md

# Including optional flags
node md2html.js path/to/your/deepwiki-file.md --repo-owner your-owner-name --repo-name your-repo-name
```

**Note:** Ensure that `deepwiki-template.html` is present in the directory where you run the command for successful conversion.