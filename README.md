# Boca Juniors 1905 — VS Code Theme

Azul y Oro. A light theme inspired by Boca Juniors: gold editor background, dark navy chrome (title bar, tabs, status bar), and cream side bar and panels.

## Palette

| Role | Color |
| --- | --- |
| Editor background | `#F4B802` |
| Navy chrome (title/status/tabs) | `#002B5C` / `#012F60` |
| Cream surfaces (sidebar, panel) | `#F6F0E4` |
| Ink (keywords, strings, comments) | `#2E1500` |
| Pale gold (functions, types, fields) | `#FFF9A8` |
| Current line highlight | `#BD9008` |

## Try it locally

1. Open this folder in VS Code.
2. Press `F5` to launch an Extension Development Host.
3. In the new window: `Cmd+K Cmd+T` → select **Boca Juniors 1905**.

## Install without publishing

```bash
npm install -g @vscode/vsce
vsce package
code --install-extension boca-juniors-1905-theme-0.1.0.vsix
```

## License

MIT
