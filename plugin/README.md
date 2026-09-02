# Conflict-of-Interest Checker for Law Firms — Claude Desktop Plugin

A Claude Desktop plugin for solo and small-firm attorneys. One skill (`/conflict-check`): Fuzzy-matches new-matter party names against your existing client/matter list — accounting for nicknames, entity-suffix variations, and misspellings — and returns a structured possible-conflict report. Never clears or declines a matter; the attorney makes every conflict determination.

**Distributed by [Protomated](https://protomated.com) as a free download.**

---

## ⚠️ Required: Read This Before You Install

### 1. You must be on a qualifying Claude plan

Do NOT use this plugin for client work on a consumer Claude plan (claude.ai Personal or Claude Pro). Consumer plans do not provide a Data Processing Agreement (DPA) covering client-privileged content. Use **Claude for Work**, **Claude Team/Enterprise**, or the **Claude API** with a signed DPA.

### 2. Every AI output requires your review

Every document this plugin generates must be reviewed and approved by you, a licensed attorney, before use. The plugin enforces this with a required header and footer on every output: `⚠️ AI-ASSISTED DRAFT — ATTORNEY REVIEW REQUIRED`.

### 3. No action without your confirmation

This plugin reads only the text or workspace folder you explicitly paste or attach — it takes no connector-based action and writes no file without your explicit in-conversation confirmation.

---

## Installation (under 5 minutes)

### Step 1 — Download and install

1. Download `conflict-of-interest-checker.zip` from the [Releases page](https://github.com/protomated/claude-conflict-of-interest-checker/releases).
2. Double-click the `.zip` file, or drag it into Claude Desktop's **Extensions** panel.
3. Claude Desktop will install the plugin.

### Step 2 — Verify

Open a new Claude Desktop chat. Type `/skills`. You should see `/conflict-check` listed. Run it to start.

---

## The Skill

### `/conflict-check` — Conflict-of-Interest Checker

Fuzzy-matches new-matter party names against your existing client/matter list — accounting for nicknames, entity-suffix variations, and misspellings — and returns a structured possible-conflict report. Never clears or declines a matter; the attorney makes every conflict determination.

---

## License

Apache 2.0. See [LICENSE](LICENSE).

## Feedback and Issues

[GitHub Issues](https://github.com/protomated/claude-conflict-of-interest-checker/issues) | [hello@protomated.com](mailto:hello@protomated.com)
