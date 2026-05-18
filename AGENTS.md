# Project Snapshot

VS Code theme extension published from `package.json`. Theme JSON files live in `themes/`, screenshots and marketplace images live in `assets/images/`.

# Key Commands

- Validate the extension manifest with `node -e "JSON.parse(require('fs').readFileSync('package.json','utf8'))"`.
- Use `rg -n "Gitlab|GitLab|gitlab" .` before release-facing changes to catch trademark-sensitive copy.

# Architecture and Conventions

- Keep marketplace metadata in `package.json`; the `icon` field should point to an original project asset under `assets/images/`.
- Keep theme labels neutral and descriptive. Avoid making third-party brand names the primary extension or theme name.
- The current marketplace display name is `VSCode Theme (Inspired by GitLab WebIDE)` and the package identifier is `unofficial-gitlab-dark-theme`.

# Known Gotchas

- Do not use the GitLab logo, tanuki/fox-like brand shapes, or GitLab as the primary extension name or icon subject. Nominative mentions such as “inspired by GitLab WebIDE” are allowed only as secondary descriptive context.
- The old `assets/images/logo.jpeg` logo asset was removed; do not restore it or point marketplace metadata to trademarked artwork.

# Memory Index

No additional `memory/*.md` files are currently needed.

# Memory Update Rules

Keep this file concise and update it only with durable repository-specific knowledge. Do not store session logs, temporary task notes, secrets, or information that is obvious from the code in a quick read.
