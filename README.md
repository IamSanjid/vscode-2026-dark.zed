# VSCode 2026 Dark — Zed Theme

A deep, low-contrast dark theme for [Zed](https://zed.dev), converted from Visual Studio Code's "2026 Dark" theme.

**Background:** `#121314` — near-black with a subtle warmth  
**Foreground:** `#bbbebf` — muted silver, easy on the eyes  
**Accent:** `#48a0c7` — cool blue, used sparingly for focus states

## Installation

Clone/Download this repo.

1. Open Zed.
2. Open the command palette (`Ctrl+Shift+P` / `Cmd+Shift+P`) and run **zed: extensions**.
3. `Install Dev Extension` select the cloned/downloaded foler.
4. Open the theme selector (`Ctrl+K Ctrl+T` / `Cmd+K Cmd+T`) and pick **Dark 2026 (VS Code)**.

Disclaimer: Haven't published the extension yet, so you can't find this from the Zed's extension repo.

## MISC

For full VS Code-like highlighting, add these to your `settings.json`:

- For Zed to pick up richer token information from language servers. Set:
```jsonc
"languages": {
  "<language>": {
    "semantic_tokens": "combined",
  },
},
```

- Highlight function parameters in the body using the same style as VS Code:

```jsonc
"global_lsp_settings": {
  "semantic_token_rules": [
    { "token_type": "parameter", "style": ["variable.parameter"] },
    { "token_type": "errorTag", "style": ["variable.parameter"] },
  ],
},
```

## License

MIT
