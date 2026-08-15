# Dobeu Tech Solutions — v0 Skills Pack

Curated agent skills for **v0.app** and other skills.sh-compatible agents,
maintained by Dobeu Tech Solutions LLC (dobeu.net).

The pack contains **82 validated, instruction-only** skills (design systems,
frameworks, UX, SEO, marketing, and the Dobeu brand skills `dobeu-v0-design`
and `dobeu-figma-make-design`). Every skill is a folder with a `SKILL.md`
(YAML frontmatter: `name`, `description`) and passes
`python3 tools/validate.py skills/`.

## This repository's current state

This repo ships the pack's **docs** (`PACK-SETUP.md`, `HYDRATE.md`,
`manifest/pack-ui-add-list.md`). The full `skills/` tree is delivered
separately as **`dobeu-v0-skills-pack.zip`**.

- **To create the pack now:** you don't need this repo populated — at
  https://skills.sh/packs → *Create pack*, upload `dobeu-v0-skills-pack.zip`
  (or its unzipped folder) directly as a source. See **PACK-SETUP.md**.
- **To make this repo a live skills.sh source** (so `npx skills add
  dobeutech/dobeu-v0-skills-pack` and *add GitHub repo* work): run the
  ~20-second steps in **HYDRATE.md** to push the `skills/` tree from the zip.

## Install (after the pack is created)

```bash
npx skills add https://skills.sh/p/<pack-id>
```

See **PACK-SETUP.md** for the full create-pack + v0 attach walkthrough, and
**NOTICE.md** (shipped in the zip) for third-party attribution. All
non-`dobeu-*` skills are permissively licensed (MIT or the author's own
terms); all `dobeu-*` skills are © 2026 Dobeu Tech Solutions LLC.
