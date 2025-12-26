# [PROJECT NAME] Documentation

> **Comprehensive documentation for [PROJECT NAME]**
> Everything you need to know to work with this project.

---

## 📖 Documentation Index

This documentation is organized into the following categories:

---

### 🚀 Quick Starts
**Get up and running fast**

- [Quick Start Guide](./quick-starts/quick-start.md) - First-time setup and basics
- [Environment Setup](./quick-starts/env-setup.md) - Configuring environment variables
- [Deployment Guide](./quick-starts/deploy.md) - Deploy to production

**When to use**: You're new to the project or need to set something up quickly.

---

### 🏗️ Architecture
**Understand how the system works**

- [System Overview](./architecture/overview.md) - High-level architecture
- [Database Schema](./architecture/database-schema.md) - Data models and relationships
- [API Design](./architecture/api-design.md) - API structure and conventions
- [Tech Stack](./architecture/tech-stack.md) - Technologies and why we chose them

**When to use**: Planning new features, understanding system design, making architectural decisions.

---

### ✨ Features
**Deep dives into specific functionality**

- [Feature 1](./features/feature-1.md) - Description
- [Feature 2](./features/feature-2.md) - Description
- [Feature 3](./features/feature-3.md) - Description

**When to use**: Working on or learning about specific features.

---

### 🔌 Integrations
**Third-party service integrations**

- [Integration 1](./integrations/integration-1.md) - Setup and usage
- [Integration 2](./integrations/integration-2.md) - Setup and usage

**When to use**: Setting up, configuring, or troubleshooting integrations.

---

### 🛠️ Development
**Developer guides and best practices**

- [Development Setup](./development/setup.md) - Local development environment
- [Coding Standards](./development/coding-standards.md) - Style guide and conventions
- [Testing Guide](./development/testing.md) - How to write and run tests
- [Debugging Tips](./development/debugging.md) - Common issues and solutions

**When to use**: Day-to-day development work.

---

### 📊 Strategy
**Planning and roadmap**

- [Roadmap](./strategy/roadmap.md) - What's next
- [Vision](./strategy/vision.md) - Long-term goals
- [Technical Decisions](./strategy/decisions.md) - Why we made certain choices

**When to use**: Planning features, understanding project direction.

---

### 🚀 Operations
**Deployment, monitoring, and maintenance**

- [Deployment](./operations/deployment.md) - How to deploy
- [Monitoring](./operations/monitoring.md) - Health checks and alerts
- [Maintenance](./operations/maintenance.md) - Regular tasks

**When to use**: Deploying, monitoring production, handling incidents.

---

## 🗺️ Finding What You Need

### By Role

**New Developer**
1. [Quick Start Guide](./quick-starts/quick-start.md)
2. [Development Setup](./development/setup.md)
3. [System Overview](./architecture/overview.md)
4. [Coding Standards](./development/coding-standards.md)

**Feature Developer**
1. [System Overview](./architecture/overview.md)
2. Relevant [Feature Docs](./features/)
3. [API Design](./architecture/api-design.md)
4. [Testing Guide](./development/testing.md)

**DevOps/Deployment**
1. [Deployment Guide](./quick-starts/deploy.md)
2. [Operations Docs](./operations/)
3. [Environment Setup](./quick-starts/env-setup.md)

**Product/Strategy**
1. [Vision](./strategy/vision.md)
2. [Roadmap](./strategy/roadmap.md)
3. [Feature Docs](./features/)

---

### By Task

| Task | Documentation |
|------|---------------|
| Set up project for first time | [Quick Start](./quick-starts/quick-start.md) |
| Configure environment variables | [Environment Setup](./quick-starts/env-setup.md) |
| Understand system architecture | [Architecture](./architecture/) |
| Add a new feature | [Architecture](./architecture/), [Features](./features/) |
| Set up integration | [Integrations](./integrations/) |
| Deploy to production | [Deployment](./operations/deployment.md) |
| Write tests | [Testing Guide](./development/testing.md) |
| Debug issue | [Debugging Tips](./development/debugging.md) |
| Understand project direction | [Strategy](./strategy/) |

---

## 🤖 AI-Assisted Development

This project includes Claude Code integration for AI-assisted development.

### Essential Context Files
- [CLAUDE.md](../CLAUDE.md) - Project context for Claude
- [.claude/SKILLS_GUIDE.md](../.claude/SKILLS_GUIDE.md) - Available skills

### Using Skills
```bash
# Brand and content
/act-brand-alignment

# [Add other relevant skills]
```

See [CLAUDE.md](../CLAUDE.md) for full details.

---

## 🌾 ACT Ecosystem

This project is part of the ACT Regenerative Innovation Ecosystem.

### LCAA Method
All development follows the **LCAA Method**:
- **Listen** - Deep listening to community and context
- **Curiosity** - Prototype boldly, test rigorously
- **Action** - Build tangible solutions
- **Art** - Translate change into culture

### Related Projects
- **ACT Main**: [ACT Regenerative Studio](https://github.com/Acurioustractor/act-regenerative-studio)
- **Empathy Ledger**: [Ethical storytelling platform](https://github.com/Acurioustractor/empathy-ledger-v2)
- **JusticeHub**: [Open justice network](https://github.com/Acurioustractor/justicehub-platform)

See [ACT ecosystem docs](https://github.com/Acurioustractor) for more.

---

## 📚 Documentation Standards

### Writing Documentation
- Use clear, concise language
- Include code examples
- Add links to related docs
- Keep it up to date

### File Organization
```
docs/
├── README.md (this file)
├── quick-starts/     # Getting started guides
├── architecture/     # System design
├── features/         # Feature documentation
├── integrations/     # Third-party integrations
├── development/      # Dev guides
├── strategy/         # Roadmap and vision
└── operations/       # Deployment and ops
```

### Templates
- Use [docs/templates/](./templates/) for common doc types
- Follow existing doc structure
- Include frontmatter when applicable

---

## 🔍 Search Tips

### Using Find
```bash
# Search all docs
grep -r "search term" docs/

# Search specific category
grep -r "search term" docs/architecture/
```

### Using Tree
```bash
# View structure
tree docs/

# View with depth limit
tree -L 2 docs/
```

---

## 🙋 Contributing to Docs

Documentation contributions are welcome!

### Making Changes
1. Find relevant file or create new one
2. Follow existing structure and tone
3. Test any code examples
4. Submit PR with clear description

### Style Guide
- Use Markdown
- Include code examples
- Add relevant links
- Keep ACT voice (see [CLAUDE.md](../CLAUDE.md))

See [CONTRIBUTING.md](../CONTRIBUTING.md) for full guidelines.

---

## 📞 Getting Help

### Documentation Issues
- **Missing docs?** Create an issue or PR
- **Outdated docs?** Submit update PR
- **Unclear docs?** Ask for clarification in issue

### Development Help
- Check [Debugging Tips](./development/debugging.md)
- Use Claude skills: `./.claude/skills-menu.sh`
- Ask in project discussions

---

## 📄 License

This documentation is part of [PROJECT NAME] and follows the same license.

---

**Last Updated**: [YYYY-MM-DD]
**Maintained By**: [Team/Person]
**Questions?** Create an issue!

🌾 Building infrastructure for a post-extractive economy 🌾
