# Contributing to [PROJECT NAME]

> **Welcome!** We're glad you're interested in contributing to the ACT ecosystem.

---

## 🌾 Code of Conduct

This project follows the [ACT Code of Conduct](https://github.com/Acurioustractor/.github/blob/main/CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

**In brief**:
- Be respectful and inclusive
- Listen deeply before responding
- Focus on solutions, not blame
- Center community benefit over individual gain
- Honor Indigenous knowledge and sovereignty

---

## 🚀 Quick Start for Contributors

### 1. Fork and Clone

```bash
# Fork the repository on GitHub, then:
git clone https://github.com/YOUR_USERNAME/[REPO_NAME].git
cd [REPO_NAME]

# Add upstream remote
git remote add upstream https://github.com/Acurioustractor/[REPO_NAME].git
```

---

### 2. Run Setup

```bash
# Run the setup script
./scripts/setup.sh

# Or manually:
npm install
cp .env.example .env.local
# Edit .env.local with your credentials
```

---

### 3. Create a Branch

Use descriptive branch names following this pattern:

```bash
# Feature branches
git checkout -b feature/your-feature-name

# Bug fixes
git checkout -b fix/bug-description

# Documentation
git checkout -b docs/what-youre-documenting

# Chores (refactoring, deps, etc)
git checkout -b chore/task-description
```

---

## 📋 Development Workflow

### Before You Start

1. **Check existing issues** - See if someone's already working on it
2. **Create or comment on issue** - Discuss approach before major work
3. **Read architecture docs** - Check `docs/architecture/` for patterns
4. **Use Claude skills** - Invoke `/act-brand-alignment` for content, etc.

---

### While You Work

1. **Follow existing patterns** - Check similar features first
2. **Write tests** - [Add project-specific testing requirements]
3. **Document as you go** - Update relevant `docs/` files
4. **Keep commits atomic** - One logical change per commit
5. **Run checks locally**:
   ```bash
   npm run lint
   npm run type-check
   npm test
   npm run build
   ```

---

### Before You Submit PR

1. **Update from upstream**:
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```

2. **Squash if needed** - Clean up commit history if it's messy

3. **Run full test suite**:
   ```bash
   npm run lint
   npm run type-check
   npm test
   npm run build
   ```

4. **Update documentation** - Ensure docs reflect your changes

---

## 📝 Commit Message Conventions

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation only
- `style:` - Code style (formatting, semicolons, etc)
- `refactor:` - Code change that neither fixes bug nor adds feature
- `perf:` - Performance improvement
- `test:` - Adding or updating tests
- `chore:` - Build process, dependencies, tooling

### Examples

```bash
# Simple feature
git commit -m "feat: add dark mode toggle to settings"

# Bug fix with scope
git commit -m "fix(auth): resolve OAuth redirect loop"

# Breaking change
git commit -m "feat!: migrate to new API endpoint

BREAKING CHANGE: The old /api/v1/users endpoint has been removed.
Use /api/v2/users instead."

# With body
git commit -m "docs: update Gmail OAuth setup guide

Added troubleshooting section for common redirect_uri errors.
Clarified callback URL configuration in Google Console."
```

---

## 🎯 Pull Request Process

### 1. Create PR

- Use the PR template (auto-populated)
- Link related issues (Fixes #123, Closes #456)
- Fill out all checklist items
- Add screenshots/videos for UI changes

### 2. PR Title Format

Follow same convention as commits:

```
feat: add user profile page
fix(auth): resolve session timeout bug
docs: update contribution guidelines
```

### 3. ACT Quality Checklist

Every PR must check these boxes:

**Code Quality**
- [ ] Code follows project style and conventions
- [ ] No console logs or debugging code
- [ ] Error handling is appropriate
- [ ] Types are properly defined (TypeScript)

**Testing**
- [ ] Tests added/updated for new functionality
- [ ] All tests pass locally
- [ ] Manual testing completed

**Documentation**
- [ ] README updated (if needed)
- [ ] CLAUDE.md updated (if needed)
- [ ] Code comments added for complex logic
- [ ] API docs updated (if applicable)

**LCAA Alignment**
- [ ] **Listen**: Does this honor community voice and context?
- [ ] **Curiosity**: Have we tested assumptions and explored alternatives?
- [ ] **Action**: Is this building tangible solutions alongside communities?
- [ ] **Art**: Does this challenge status quo and translate change into culture?

**Security & Performance**
- [ ] No exposed secrets or credentials
- [ ] No performance regressions
- [ ] Accessibility considered (if UI)

---

### 4. Code Review

- Address all feedback
- Be respectful and collaborative
- Ask questions if feedback is unclear
- Push new commits (don't force push during review)

---

### 5. Merge

Once approved:
- Maintainer will merge (usually squash merge)
- Delete your branch after merge
- Celebrate!

---

## 🎨 LCAA Methodology in Practice

All contributions should align with ACT's LCAA method:

### Listen
- Have you deeply listened to the problem context?
- Does this solution honor community voice?
- Have you considered historical and cultural context?

### Curiosity
- Have you explored alternative approaches?
- Did you prototype and test rigorously?
- Are you solving root causes, not just symptoms?

### Action
- Is this building tangible solutions?
- Are you working alongside communities, not for them?
- Does this create immediate value?

### Art
- Does this challenge extractive status quo?
- Can this translate change into culture?
- Is there beauty in the solution?

**Use this lens for all contributions** - from code architecture to documentation tone.

---

## 🏷️ Issue Labels Guide

When creating or working on issues, use these labels:

### Priority
- `priority: critical` - Urgent, blocking work
- `priority: high` - Important, should be next
- `priority: medium` - Normal priority
- `priority: low` - Nice to have

### Type
- `type: bug` - Something isn't working
- `type: feature` - New functionality
- `type: chore` - Maintenance work
- `type: docs` - Documentation
- `type: security` - Security issue

### LCAA Phase
- `lcaa: listen` - Research, discovery, community listening
- `lcaa: curiosity` - Prototyping, experimentation
- `lcaa: action` - Building, implementation
- `lcaa: art` - Creative expression, cultural translation

### Status
- `status: blocked` - Waiting on something
- `status: in progress` - Actively being worked on
- `status: ready for review` - PR submitted
- `status: needs discussion` - Needs team input

---

## 🧪 Testing Guidelines

[Add project-specific testing requirements]

**Example**:
```bash
# Run all tests
npm test

# Watch mode during development
npm test -- --watch

# Coverage report
npm test -- --coverage
```

---

## 📦 Adding Dependencies

**Before adding a new dependency**:
1. Check if existing dependency can solve the problem
2. Evaluate bundle size impact (use [bundlephobia](https://bundlephobia.com/))
3. Check license compatibility (prefer MIT, Apache 2.0)
4. Consider maintenance status (actively maintained?)
5. Discuss in issue first for major dependencies

**Adding dependency**:
```bash
npm install package-name
# or for dev dependencies
npm install -D package-name

# Document why in commit message
git commit -m "chore: add [package] for [reason]"
```

---

## 🎨 Style Guide

### Code Style
- Follow existing code style (linter will enforce)
- Use TypeScript for type safety
- Prefer functional components (React)
- Use descriptive variable names
- Comment complex logic

### Documentation Style
- Use clear, concise language
- Include code examples
- Add links to related docs
- Use ACT voice (see CLAUDE.md)

### Commit Style
- Follow Conventional Commits (see above)
- Keep commits focused and atomic
- Write clear commit messages

---

## 🚦 What to Contribute

### Good First Issues
Look for `good first issue` label - these are beginner-friendly!

### Areas We Need Help
- [ ] [List specific areas where contributions are welcome]
- [ ] Documentation improvements
- [ ] Test coverage
- [ ] Bug fixes
- [ ] Performance optimizations

### Before Starting Major Work
- Create or comment on an issue
- Discuss approach with maintainers
- Get buy-in before investing significant time

---

## 🤝 Getting Help

### Documentation
- Start with [docs/quick-starts/quick-start.md](./docs/quick-starts/quick-start.md)
- Check [CLAUDE.md](./CLAUDE.md) for project context
- Browse [docs/](./docs/) for detailed guides

### Claude Skills
```bash
# Use AI assistance
/act-brand-alignment  # For content and voice
# [Add other relevant skills]
```

### Community
- Ask questions in issues
- Join ACT ecosystem discussions
- Reach out to maintainers

---

## 🙏 Thank You

Every contribution, no matter how small, helps build infrastructure for a post-extractive economy.

**Your work matters. Together we're cultivating solutions.**

---

## 📄 License

By contributing, you agree that your contributions will be licensed under the same license as this project (see [LICENSE](./LICENSE)).

---

**Last Updated**: [YYYY-MM-DD]
**Questions?** Create an issue or reach out to maintainers!
