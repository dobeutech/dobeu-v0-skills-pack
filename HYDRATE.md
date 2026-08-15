# Hydrate this repo with the full skills/ tree (one-time, ~20 seconds)

This repository ships with the pack's docs and manifest. The full 82 skill
folders live in `dobeu-v0-skills-pack.zip` (delivered to you in chat). To make
this repo usable as a skills.sh "add GitHub repo" pack source, push the skills:

```bash
git clone https://github.com/dobeutech/dobeu-v0-skills-pack.git
cd dobeu-v0-skills-pack
unzip /path/to/dobeu-v0-skills-pack.zip -d .   # adds skills/, overwrites docs identically
git add -A
git commit -m "feat: add 82 v0-compatible skills + references"
git push
```

You do NOT need this step to create the pack: at https://skills.sh/packs → Create
pack, you can upload `dobeu-v0-skills-pack.zip` (or its unzipped folder) directly
as a source. See PACK-SETUP.md.
