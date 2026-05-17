---
name: skill-creator-prompt-installer
installer_version: 1.0
---

# skill-creator-prompt

**Interactive Skill Design Assistant**

A lightweight, concise assistant that helps users design high-quality Grok skills through short, focused questions using a simple 4-phase flow (with an optional 5th phase for programming-related skills).

This package contains everything needed to install the `skill-creator-prompt` skill.

---

## Installation Instructions

Identify current `skill-creator` methods and then proceed with the following to install skill.

### Option 1: Automatic / Semi-Automatic (Recommended)

If you are sharing this with Grok or another AI:

1. Decompress / extract this `skill-creator-prompt` folder.
2. Place the entire folder into:
   ```
   /home/workdir/.grok/skills/
   ```
3. The skill should now be available.

Alternatively, ask Grok to run:

```bash
cp -r /path/to/skill-creator-prompt /home/workdir/.grok/skills/
```

### Option 2: Manual Installation

1. Create the skill directory:
   ```bash
   mkdir -p /home/workdir/.grok/skills/skill-creator-prompt/references
   ```

2. Copy the following files into place:
   - `SKILL.md` → `/home/workdir/.grok/skills/skill-creator-prompt/SKILL.md`
   - `references/archetypes.md` → `/home/workdir/.grok/skills/skill-creator-prompt/references/archetypes.md`
   - `references/scripting-guidance.md` → `/home/workdir/.grok/skills/skill-creator-prompt/references/scripting-guidance.md`

3. (Optional) Validate the skill:
   ```bash
   bash /root/.grok/skills/skill-creator/scripts/validate-skill.sh /home/workdir/.grok/skills/skill-creator-prompt
   ```

Once installed, you can activate it by saying things like:
- “Help me design a new skill”
- “Use skill-creator-prompt to create a skill for…”

---

## Folder Structure

```
skill-creator-prompt/
├── README.md
├── SKILL.md
└── references/
    ├── archetypes.md
    └── scripting-guidance.md
```

---

## What This Skill Does

- Guides users through a short, low-friction 4-phase process
- Helps decide on skill purpose, constraint level, and supporting files
- Recommends Python scripts when beneficial
- Provides clear instructions on how to save the generated skill
- Designed to minimize mental overload while producing consistent, well-structured skills

---

## Notes

- This skill works best alongside the built-in `skill-creator`.
- It focuses on the *design conversation*, while `skill-creator` handles quick initialization.
- The interaction is intentionally kept concise for better usability.

---

**This package is ready to be zipped and shared.**
