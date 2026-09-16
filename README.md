<p align="center">
  <img src="assets/hero.svg" alt="A little tower of nigiri on a cream counter" width="920" />
</p>

<h1 align="center">sushi-stack</h1>

<p align="center">
  <em>a tiny omakase of Cursor agent skills</em><br />
  <sub>pick a piece · dip it in a chat · don’t put wasabi in the soy (that’s a built-in skill)</sub>
</p>

<p align="center">
  <a href="https://github.com/Sushmithamallesh/sushi-stack"><img alt="public" src="https://img.shields.io/badge/kitchen-open-f07858?style=for-the-badge&labelColor=fff7f0" /></a>
  <a href="https://cursor.com"><img alt="cursor skills" src="https://img.shields.io/badge/served_with-Cursor-6b3f2a?style=for-the-badge&labelColor=fff7f0" /></a>
</p>

---

This is my personal conveyor belt. Each plate is a folder with a `SKILL.md`. I add pieces when I actually want them — nothing pre-plated.

Cursor looks for personal skills here:

```text
~/.cursor/skills/<skill-name>/SKILL.md
```

So this repo *is* the wooden counter. Clone it there, or sit it somewhere comfy and symlink.

## 🍙 set the counter

```bash
git clone git@github.com:Sushmithamallesh/sushi-stack.git ~/.cursor/skills
```

Already have a `~/.cursor/skills` drawer? Clone beside it and tie the knot:

```bash
git clone git@github.com:Sushmithamallesh/sushi-stack.git ~/Developer/sushi-stack
ln -s ~/Developer/sushi-stack ~/.cursor/skills
```

Leave `~/.cursor/skills-cursor/` alone. That’s the restaurant’s own menu, not ours.

## 🍱 the menu

_Empty on purpose. The chef is still humming._

When a skill lands, it will show up as its own little plate:

```text
sushi-stack/
  some-skill/
    SKILL.md
```

## 🥢 add a piece

1. Make `skill-name/SKILL.md` (lowercase, numbers, hyphens — like a good slug of rice).
2. Commit. Push. Bow slightly.
3. Project-only recipes still live in that repo’s `.cursor/skills/`. House specials stay here.

---

<p align="center">
  <sub>no substitutions · extra ginger on request · made with rice, yaml, and vibes</sub>
</p>
