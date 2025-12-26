# ACT Project Template

> **Standard template for all ACT ecosystem projects**
> Includes workflows, documentation structure, Claude skills integration, and ACT conventions

---

## 🎯 What This Is

This template provides a standardized structure for all [ACT (A Curious Tractor)](https://github.com/Acurioustractor) projects, ensuring:

- ✅ Consistent project structure
- ✅ Standard GitHub workflows (test, deploy, security, auto-label)
- ✅ Professional documentation organization
- ✅ Claude Code AI assistance ready
- ✅ LCAA methodology embedded
- ✅ Professional issue/PR templates

---

## 🚀 Quick Start

### 1. Use This Template

Click "Use this template" button on GitHub, or:

```bash
# Clone this template
git clone https://github.com/Acurioustractor/act-project-template.git my-new-project
cd my-new-project

# Remove git history
rm -rf .git
git init
git add .
git commit -m "feat: initialize from ACT project template"

# Create new repo and push
gh repo create Acurioustractor/my-new-project --public --source=. --push
```

---

### 2. Run Setup Script

```bash
./scripts/setup.sh
```

This will:
- Install dependencies
- Copy environment template
- Link global Claude skills
- Initialize database (if applicable)

---

### 3. Customize

Update these files for your project:

- [ ] **README.md** - Replace with your project details
- [ ] **CLAUDE.md** - Update with your project context
- [ ] **package.json** - Update name, description
- [ ] **.env.example** - Add your environment variables
- [ ] **docs/** - Add your project documentation
- [ ] **.claude/skills/local/** - Create project-specific skills

---

## 📁 What's Included

### `.github/` - GitHub Configuration
- **workflows/** - 5 standard workflows (test, deploy, security, auto-label, type-sync)
- **ISSUE_TEMPLATE/** - Bug, Feature, Task, Epic templates
- **PULL_REQUEST_TEMPLATE.md** - ACT Quality Checklist
- **labeler.yml** - Auto-labeling configuration
- **CODEOWNERS** - Auto-reviewer assignment

### `.claude/` - AI Assistant Configuration
- **skills/global/** - Symlink to global ACT skills
- **skills/local/** - Project-specific skills
- **SKILLS_GUIDE.md** - Available skills documentation

### `docs/` - Documentation Structure
- **quick-starts/** - Getting started guides
- **architecture/** - System design docs
- **features/** - Feature documentation
- **integrations/** - Integration guides
- **development/** - Dev environment setup
- **strategy/** - Roadmaps and vision

### `scripts/` - Automation Scripts
- **setup.sh** - One-command project setup
- **health-check.sh** - Project health diagnostics

### Standard Files
- **CLAUDE.md** - AI assistant context
- **CONTRIBUTING.md** - Contribution guidelines
- **README.md** - Project overview
- **.env.example** - Environment variable template
- **.gitignore** - Standard ignores

---

## 🤖 Claude Skills

This template includes integration with global ACT skills:

**Global Skills** (available in all ACT projects):
- `/act-brand-alignment` - ACT voice, LCAA methodology, content creation
- `/ghl-crm-advisor` - GoHighLevel CRM strategy
- `/act-github-pm` - GitHub project management help
- `/act-deployment-helper` - Deployment troubleshooting
- `/act-security-advisor` - Security best practices

**To activate**:
```bash
# Link global skills (done by setup.sh)
ln -s ~/act-global-skills .claude/skills/global
```

---

## 📋 Standard Workflows

### 1. `test.yml` - CI/CD Testing
**Triggers**: PR, Push to main/develop
**Jobs**:
- Lint & Type Check
- Build
- Tests
- Security Audit

### 2. `deploy.yml` - Auto-Deployment
**Triggers**: Push to main
**Jobs**:
- Deploy to Vercel/Production
- Notify Team

### 3. `security-scan.yml` - Security Scanning
**Triggers**: Weekly (Monday 9 AM), PR (package changes)
**Jobs**:
- Dependency Audit
- Secret Scanning
- CodeQL Analysis

### 4. `auto-label.yml` - Auto-Labeling
**Triggers**: PR/Issue open or edit
**Jobs**:
- Label based on files changed
- Label based on PR size
- Label based on branch name

### 5. `type-sync.yml` - Type Synchronization
**Triggers**: Push to main (types changed)
**Jobs**:
- Sync types across ACT repos
- Create PRs with updates

---

## 🏷️ Standard Labels

All ACT projects use these 37 labels:

**Categories**:
- **Priority**: Critical, High, Medium, Low
- **Type**: Bug, Feature, Chore, Documentation, Security, Refactor
- **Project**: ACT Main, Empathy Ledger, JusticeHub, Harvest, etc.
- **Effort**: 1h, 3h, 1d, 3d, 1w, 2w
- **Status**: Blocked, In Progress, Ready for Review, Needs Discussion
- **LCAA**: Listen, Curiosity, Action, Art
- **Special**: Good First Issue, Help Wanted, Breaking Change

Deploy labels to your repo:
```bash
node ~/act-global-scripts/setup-github-labels.mjs --repo your-repo-name
```

---

## 🎨 ACT Methodology (LCAA)

All ACT projects follow the **LCAA Method**:

- **Listen** → Deep listening to place, people, community voice
- **Curiosity** → Think deeply, prototype boldly, test rigorously
- **Action** → Build tangible solutions alongside communities
- **Art** → Translate change into culture, challenge status quo

### In Practice:
- Issues tagged with LCAA phase labels
- PR template includes LCAA alignment checklist
- Documentation organized by LCAA phases
- Workflows support each phase

---

## 📚 Documentation

See the [docs/](./docs/) folder for:

- [Quick Start Guide](./docs/quick-starts/quick-start.md)
- [Architecture Overview](./docs/architecture/overview.md)
- [Development Setup](./docs/development/setup.md)
- [Contributing Guide](./CONTRIBUTING.md)

---

## 🔧 Customization Guide

### For Web Apps (Next.js, React)
- Keep `src/` folder
- Update `package.json` with your dependencies
- Add `.env.example` with your variables
- Update `deploy.yml` with your deployment config

### For Backend Services (Node.js, API)
- Use `src/` for source code
- Update workflows as needed
- Add database migration scripts
- Document API endpoints

### For Libraries/Packages
- Remove `deploy.yml` (not needed)
- Keep `test.yml` for CI
- Add `publish.yml` for npm publishing
- Focus on API documentation

---

## 🌾 ACT Ecosystem

This template is part of the ACT Regenerative Innovation Ecosystem:

- **ACT Main**: https://github.com/Acurioustractor/act-regenerative-studio
- **Empathy Ledger**: https://github.com/Acurioustractor/empathy-ledger-v2
- **JusticeHub**: https://github.com/Acurioustractor/justicehub-platform
- **The Harvest**: https://github.com/Acurioustractor/theharvest
- **More**: https://github.com/Acurioustractor

**Unified visibility**: https://github.com/users/Acurioustractor/projects/1

---

## 📞 Support

- **Issues**: Create an issue in this repo
- **Documentation**: Check [docs/](./docs/)
- **Claude Skills**: Run `./.claude/skills-menu.sh`
- **Community**: Join ACT ecosystem discussions

---

## 📄 License

AGPL-3.0 - See [LICENSE](./LICENSE) for details

---

**🌾 Building infrastructure for a post-extractive economy 🌾**

**Last Updated**: 2025-12-26
**Version**: 1.0.0
**Maintained By**: ACT Ecosystem Team
