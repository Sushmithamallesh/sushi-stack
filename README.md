# cursor-skills

Personal Cursor Agent Skills. Each skill is a directory with a `SKILL.md`.

Add skills here when you want them. Cursor loads personal skills from `~/.cursor/skills/<skill-name>/SKILL.md`.

## Use this repo as your skills folder

```bash
git clone git@github.com:Sushmithamallesh/cursor-skills.git ~/.cursor/skills
```

If `~/.cursor/skills` already exists, clone elsewhere and symlink:

```bash
git clone git@github.com:Sushmithamallesh/cursor-skills.git ~/Developer/cursor-skills
ln -s ~/Developer/cursor-skills ~/.cursor/skills
```

Do not put skills in `~/.cursor/skills-cursor/` — that folder is Cursor’s built-in skills.

## Add a skill

1. Create `skill-name/SKILL.md` (lowercase letters, numbers, hyphens).
2. Commit and push.

Project-only skills still live in a repo’s `.cursor/skills/`, not here.
