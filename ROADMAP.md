# Roadmap

Path to publishing "Boca Juniors 1905" and ideas beyond.

## 0.x — Polish (pre-publish)

- [ ] Dogfood the theme for a week across languages (Go, TypeScript, Python, YAML, Markdown) and fix low-contrast spots
- [ ] Review diff view, merge conflict view, and settings UI colors
- [ ] Check accessibility: cursor visibility, selection contrast, find-match visibility
- [ ] Add a second screenshot (terminal + panel) to the README

## 1.0 — Publish to the VS Code Marketplace

- [ ] Create an [Azure DevOps organization](https://dev.azure.com) (required for the Marketplace)
- [ ] Create a Personal Access Token with the **Marketplace → Manage** scope
- [ ] Create a publisher at [marketplace.visualstudio.com/manage](https://marketplace.visualstudio.com/manage) matching `"publisher": "rmpato"` in `package.json`
- [ ] `vsce login rmpato`, then `vsce publish` (or add the `VSCE_PAT` repo secret and uncomment the publish step in `.github/workflows/release.yml`)
- [ ] Verify the Marketplace listing: icon, banner, README rendering, screenshot
- [ ] Also publish to [Open VSX](https://open-vsx.org) so Cursor/VSCodium users can install it (`npx ovsx publish -p <token>`)

## Ideas / Backlog

- [ ] **Dark variant**: "La Bombonera de Noche" — navy editor background with gold accents
- [ ] High-contrast variant
- [ ] Product icon theme with a Boca-styled icon set
- [ ] Bracket pair and semantic token fine-tuning for more languages (Rust, Terraform/HCL like the original inspiration)
- [ ] Preview GIF cycling through file types

## Notes

- The club name and crest are trademarks of CABJ; the extension icon is an original, stylized shield. If the Marketplace listing ever draws a complaint, swap in a more generic gold/navy shield.
- Version with semver; every release is tagged `vX.Y.Z`, which CI turns into a GitHub release with the `.vsix` attached.
