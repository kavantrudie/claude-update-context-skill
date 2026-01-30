# Skills Collection

This directory contains reusable skills for AI coding agents. Each skill is organized in its own subdirectory with comprehensive documentation and examples.

## Available Skills

### update-context

Captures conversation context and creates structured markdown documentation in your project's `.claude/context-docs/` directory.

**Use cases:**
- Document feature implementations
- Capture architectural decisions
- Record bug analysis and fixes
- Preserve design discussions

**Quick start:**
```bash
/update-context feature my-feature-name
/update-context bug issue-123
/update-context architecture auth-redesign
```

[Full documentation →](./update-context/)

## How Skills Work

Each skill directory contains:
- `SKILL.md` - Skill definition with instructions for Claude Code
- `README.md` - User-facing documentation
- `template.md` - Templates used by the skill (if applicable)
- `examples/` - Sample outputs and usage examples

## Using Skills

### With Claude Code

Skills are automatically loaded when placed in:
- `~/.claude/skills/` (global installation)
- `./.claude/skills/` (project-specific)

### With Vercel Skills CLI

```bash
npx skills add https://github.com/kavantrudie/claude-update-context-skill
```

The CLI will install all skills from this repository.

## Contributing Skills

Want to add a new skill to this collection?

1. Create a new directory under `skills/` with your skill name
2. Add required files:
   - `SKILL.md` with proper frontmatter
   - `README.md` with usage instructions
   - Templates and examples as needed
3. Test the skill with Claude Code
4. Submit a pull request

See existing skills for examples of structure and format.

## Skill Development Guidelines

- Keep skills focused on a single, clear purpose
- Provide comprehensive examples
- Include error handling guidance
- Document all expected arguments
- Test with both manual and automatic invocation

---

For more information, see the [main repository README](../README.md).
