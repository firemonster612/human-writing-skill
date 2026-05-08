# Human Writing Skill

A skills.sh-compatible agent skill for writing prose that reads naturally and avoids common AI-writing tells.

## Install

After this repository is pushed to GitHub:

```bash
npx skills add firemonster612/human-writing-skill --skill human-writing
```

To install globally for Codex:

```bash
npx skills add firemonster612/human-writing-skill --skill human-writing --agent codex --global --yes
```

## Structure

```text
skills/
  human-writing/
    SKILL.md
    references/
      banned-vocabulary.md
```

The `SKILL.md` file contains the required skills.sh frontmatter:

```yaml
name: human-writing
description: >
  Write text that reads as authentically human rather than AI-generated.
```

## Publishing to skills.sh

skills.sh indexes public GitHub repositories that can be installed with the `skills` CLI. Push this repository publicly, then run an install command once:

```bash
npx skills add firemonster612/human-writing-skill --skill human-writing
```

Once the CLI has seen the public source, the skill should become discoverable on skills.sh under:

```text
https://skills.sh/firemonster612/human-writing-skill/human-writing
```
