# scripts/export_skills.py

Combine every skill an AI agent can reach into one portable, multi-agent bundle
and emit a downloadable `.zip`. Pure standard library — no installs.

```bash
python3 scripts/export_skills.py --out ./skills-export --zip ./skills-export.zip
```

The bundle contains:

- `skills.md` — one combined index of every skill (catalog + full instructions)
- `AGENTS.md` — Codex-compatible entry point (catalog + pointers by default; use
  `--inline-agents` to inline every body)
- `skills/<name>/SKILL.md` — individual skills in Claude / skills.sh layout
- `v0/skills-list.md` — name+description list for attaching skills in v0.app
- `manifest.csv` — origin, slug, and dedup status per skill

Discovery is automatic (`~/.claude/skills/synced`, `~/.claude/plugins/synced/*/skills`,
project-local `./skills`, and `$CLAUDE_SKILLS_PATH`); point it elsewhere with
repeatable `--src <dir>`. Skills are de-duplicated by name (personal over plugin);
shadowed duplicates are recorded in `manifest.csv`, never dropped silently.

This is the same tool packaged as the standalone `skills-exporter` skill.
