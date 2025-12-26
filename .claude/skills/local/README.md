# Local Project Skills

Project-specific Claude Code skills.

## Create a New Local Skill

1. Create skill directory:
   ```bash
   mkdir .claude/skills/local/my-skill-name
   ```

2. Create SKILL.md inside:
   ```bash
   cat > .claude/skills/local/my-skill-name/SKILL.md << 'SKILL'
   # My Skill Name

   **Purpose**: Brief description

   ## What This Skill Does
   [Description]

   ## When to Use
   - Use case 1
   - Use case 2

   ## Example
   [Example interaction]
   SKILL
   ```

3. Update [SKILLS_GUIDE.md](../SKILLS_GUIDE.md) to include your new skill

## Example: Project Assistant Skill

For a project-specific assistant skill:

```bash
mkdir .claude/skills/local/my-project-assistant
```

Then create `SKILL.md` with project-specific knowledge and examples.

## Tips

- Keep skills focused on project-specific knowledge
- Use global skills for cross-project capabilities
- Document examples clearly
- Link to relevant project documentation
