# Conflict-of-Interest Checker — Claude Desktop Plugin

A Claude Desktop plugin for solo and small-firm attorneys. One skill (`/conflict-check`): Fuzzy-matches new-matter party names against your existing client/matter list — accounting for nicknames, entity-suffix variations, and misspellings — and returns a structured possible-conflict report. Never clears or declines a matter; the attorney makes every conflict determination.

Distributed free by [Protomated](https://protomated.com).

---

## Repo layout

```text
plugin/           Installable plugin (packaged into .zip)
  .claude-plugin/plugin.json   Identity manifest
  .mcp.json                    Empty — no connector required
  skills/conflict-check/
    SKILL.md                   The single skill
    reference/                 Bundled reference material the skill cites

scripts/
  validate-plugin.mjs          Validates plugin/ structure before packing

.github/workflows/
  validate.yml     Runs on every push/PR — validates plugin structure
  release.yml      Runs on vX.Y.Z tags — builds, checksums, and publishes a GitHub Release
```

---

## Skill

| Skill | What it does |
|---|---|
| `/conflict-check` | Fuzzy-matches new-matter party names against your existing client/matter list — accounting for nicknames, entity-suffix variations, and misspellings — and returns a structured possible-conflict report. Never clears or declines a matter; the attorney makes every conflict determination. |

---

## Development

```bash
npm run validate   # validate plugin/ structure
npm run build      # validate → pack → checksum
npm run release    # build + gh release create (requires gh CLI + repo write access)
```

---

## Part of the Protomated Plugin Marketplace

This plugin also ships via the [Protomated plugin marketplace](https://github.com/protomated/protomated-plugins-official) (git-native install, no zip needed) — install this repo's zip release if you want a pinned version instead.

## License

Apache 2.0. See [LICENSE](LICENSE).
