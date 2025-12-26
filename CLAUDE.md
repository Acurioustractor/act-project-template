# [PROJECT NAME] - Claude Code Context

> **Quick Reference for Claude Code**
> This document provides essential context about this codebase for AI-assisted development.

---

## 🎯 Project Overview

**Name**: [PROJECT NAME]
**Purpose**: [Brief description of what this project does]
**Tech Stack**: [e.g., Next.js 15, React 19, TypeScript, Tailwind CSS]
**Primary Focus**: [Main functionality/features]

---

## 🚀 Quick Start

### Essential Commands
```bash
# Start development server
npm run dev        # [Port number, e.g., Port 3001]

# Build for production
npm run build

# Run tests
npm test

# Lint and type check
npm run lint
npm run type-check
```

### Key Files to Read First
1. [README.md](./README.md) - Project setup and overview
2. [docs/quick-starts/quick-start.md](./docs/quick-starts/quick-start.md) - Getting started
3. [docs/architecture/overview.md](./docs/architecture/overview.md) - System architecture
4. [.claude/SKILLS_GUIDE.md](./.claude/SKILLS_GUIDE.md) - Available Claude skills

---

## 📁 Codebase Structure

### Root Directories
```
/
├── src/                    # [Description, e.g., Next.js application code]
│   ├── app/               # [e.g., App router pages and API routes]
│   ├── components/        # [e.g., React components]
│   ├── lib/               # [e.g., Utilities, clients, integrations]
│   └── types/             # [e.g., TypeScript type definitions]
├── docs/                  # Organized documentation
├── scripts/               # Build, deployment, and utility scripts
├── .claude/              # Claude Code skills and configuration
└── public/               # [e.g., Static assets]
```

### Documentation Organization (`/docs/`)

**Essential Categories:**
- **quick-starts/** - Getting started guides
- **architecture/** - System design, database schema, integration patterns
- **features/** - Feature documentation
- **integrations/** - Third-party integrations
- **development/** - Dev environment setup, best practices
- **strategy/** - Roadmaps, vision
- **operations/** - Deployment, monitoring

---

## 🔧 Core Features

### 1. [Feature Name]
**What**: [Brief description]
**Key Files**:
- `src/[path/to/file.ts]` - [Description]
- `src/app/[route]/page.tsx` - [Description]

**Docs**: [docs/features/feature-name/](./docs/features/feature-name/)

### 2. [Another Feature]
**What**: [Brief description]
**Key Files**:
- `src/[path/to/file.ts]` - [Description]

**Docs**: [docs/features/another-feature/](./docs/features/another-feature/)

---

## 🤖 Claude Code Skills

This project has specialized skills to help with common tasks. Invoke with `/skill-name`.

### Available Skills

**Global Skills** (available in all ACT projects):
- `/act-brand-alignment` - ACT voice, LCAA methodology, content creation
- `/ghl-crm-advisor` - GoHighLevel CRM strategy (if applicable)

**Local Skills** (project-specific):
- [Add project-specific skills here]

### Skill Discovery

See comprehensive guide: [.claude/SKILLS_GUIDE.md](./.claude/SKILLS_GUIDE.md)

---

## 🗄️ Database Schema

**Platform**: [e.g., Supabase (PostgreSQL), MongoDB, etc.]
**Key Tables/Collections**:
- `table_name` - [Description]
- `another_table` - [Description]

**Schema Docs**: [docs/architecture/database-schema.md](./docs/architecture/database-schema.md)

---

## 🔐 Environment Variables

**Required**:
```bash
# [Service Name]
SERVICE_API_KEY=...
SERVICE_URL=...

# [Another Service]
ANOTHER_SERVICE_KEY=...
```

**Setup Guide**: [docs/quick-starts/env-setup.md](./docs/quick-starts/env-setup.md)

---

## 🎨 ACT Brand Voice & Methodology

### LCAA Method
**Listen** → **Curiosity** → **Action** → **Art**

Frame all solutions through this lens:
- **Listen**: Deep listening to place, people, history, community voice
- **Curiosity**: Think deeply, prototype boldly, test rigorously
- **Action**: Build tangible solutions alongside communities
- **Art**: Translate change into culture, challenge status quo

### Voice Characteristics
- **Grounded yet Visionary** - Plant seeds today for forests tomorrow
- **Humble yet Confident** - We don't have all answers, but we're cultivating solutions
- **Warm yet Challenging** - Let's get our hands dirty with hard truths
- **Poetic yet Clear** - Use metaphor to illuminate, not obscure

### Avoid
- Savior narratives, paternalistic framing, luxury positioning
- Corporate jargon, glossy marketing speak, overclaiming

**Brand Docs**: Use `/act-brand-alignment` skill for all user-facing content

---

## 🛠️ Development Workflows

### Adding a New Feature
1. Read relevant architecture docs in `docs/architecture/`
2. Check existing patterns in `src/lib/` and `src/components/`
3. Update database schema if needed
4. Write feature code following existing patterns
5. Test locally
6. Document in appropriate `docs/features/` file

### Common Development Tasks
- **Adding a route**: [Describe process]
- **Creating a component**: [Describe process]
- **Adding an integration**: [Describe process]

---

## 📚 Finding Documentation

### By Task
- **Getting started?** → `docs/quick-starts/`
- **Understanding architecture?** → `docs/architecture/`
- **Setting up integration?** → `docs/integrations/`
- **Learning about features?** → `docs/features/`
- **Strategic planning?** → `docs/strategy/`

### Navigation Aids
- [docs/README.md](./docs/README.md) - Documentation index
- [.claude/SKILLS_GUIDE.md](./.claude/SKILLS_GUIDE.md) - Skills guide
- This file (CLAUDE.md) - You are here!

---

## 🚦 Common Tasks Reference

### Task: "[Example task]"
**Skill**: `/skill-name` (if applicable)
**Docs**: `docs/category/`
**Code**: `src/path/to/code.ts`
**Pattern**: [Brief description of approach]

---

## 💡 Tips for AI-Assisted Development

1. **Always check docs first** - Documentation is organized by category in `docs/`
2. **Use skills for domain expertise** - Invoke relevant skills for specialized help
3. **Follow existing patterns** - Check similar features before creating new patterns
4. **Respect brand voice** - Use `/act-brand-alignment` for any user-facing content
5. **Test thoroughly** - [Project-specific testing guidelines]
6. **Document as you go** - Add to appropriate `docs/` category

---

## 🌾 ACT Ecosystem

This project is part of the ACT Regenerative Innovation Ecosystem:

**Ecosystem Overview**: https://github.com/Acurioustractor
**Unified Project Board**: https://github.com/users/Acurioustractor/projects/1

**Related Projects**:
- **ACT Main**: ACT Regenerative Studio
- **Empathy Ledger**: Ethical storytelling platform
- **JusticeHub**: Open-source justice network
- **The Harvest**: Community hub and heritage preservation
- **More**: https://github.com/Acurioustractor

---

**Last Updated**: [YYYY-MM-DD]
**Maintained By**: [Team/Person Name]
**Questions?** Check `.claude/SKILLS_GUIDE.md` or create an issue!
