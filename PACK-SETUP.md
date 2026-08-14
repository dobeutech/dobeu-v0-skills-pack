# Creating the pack (you do this once — ~3 minutes)

1. Open https://skills.sh/packs and click **Create pack**. Sign in with your Vercel
   account (the one that owns the **Dobeu Tech Solutions LLC** team).
2. Name: `dobeu-v0-pack`. Description: `Dobeu Tech Solutions design + frontend skills
   for v0.app`. Team: **Dobeu Tech Solutions LLC**.
3. Add skills — two sources:
   a. **GitHub repo:** add `dobeutech/dobeu-v0-skills-pack` (every folder under
      `skills/` is picked up; invalid files are auto-skipped).
      — OR upload `dobeu-v0-skills-pack.zip` if you prefer not to link GitHub.
   b. **Public skills:** search and add each entry in `manifest/pack-ui-add-list.md`
      (the curated Vercel skills + any of your style skills that are already public).
4. Click create, then copy the install command shown:
   `npx skills add https://skills.sh/p/<pack-id>` — paste it back to Claude for the
   post-creation verification step.

# Using it in v0.app

- v0 Skills menu (the one in your screenshot) → **Teams** section: team-shared skills
  for Dobeu Tech Solutions LLC appear here; **My skills** shows your personal ones;
  attach a skill to any prompt.
- If a pack skill does not appear under Teams automatically, use **Explore skills** →
  search its name, or attach the skill to a prompt directly. (Vercel currently surfaces
  team skills in v0 via the team association; the pack install link always works for
  CLI agents regardless.)

# Warning

Packs are UNLISTED, not private — anyone with the URL can view and install. This repo
contains no secrets (verified by the Task 4 secret scan). Keep it that way.
