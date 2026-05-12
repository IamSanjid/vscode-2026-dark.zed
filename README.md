# VSCode 2026 Dark — Zed Theme

A deep, low-contrast dark theme for [Zed](https://zed.dev), converted from Visual Studio Code's "2026 Dark" theme.

**Background:** `#121314` — near-black with a subtle warmth  
**Foreground:** `#bbbebf` — muted silver, easy on the eyes  
**Accent:** `#48a0c7` — cool blue, used sparingly for focus states

## Installation

1. Open Zed.
2. Open the command palette (`Ctrl+Shift+P` / `Cmd+Shift+P`) and run **zed: extensions**.
3. Search for **VSCode 2026 Dark** and click **Install**.
4. Open the theme selector (`Ctrl+K Ctrl+T` / `Cmd+K Cmd+T`) and pick **Dark 2026 (VS Code)**.

Or install via the CLI:

```
zed:install vscode-2026-dark
```

## MISC

For full VS Code-like highlighting, add these to your `settings.json`:

- For Zed to pick up richer token information from language servers. Set:
```json
"languages": {
  "<language>": {
    "semantic_tokens": "combined",
  },
},
```

- Highlight function parameters in the body using the same style as VS Code:

```json
"global_lsp_settings": {
  "semantic_token_rules": [
    { "token_type": "parameter", "style": ["variable.parameter"] }
  ]
}
```

## License

MIT
