# Quick Start Guide

> **Get [PROJECT NAME] running in minutes**
> This guide walks you through first-time setup and basic usage.

---

## 📋 Prerequisites

Before you begin, ensure you have:

- **Node.js** (v18+) - [Download](https://nodejs.org/)
- **npm** or **yarn** - Included with Node.js
- **Git** - [Download](https://git-scm.com/)
- **[Any other requirements]** - e.g., Docker, PostgreSQL, etc.

### Check Prerequisites

```bash
# Check Node.js version
node --version
# Should show v18.0.0 or higher

# Check npm version
npm --version

# Check git
git --version
```

---

## 🚀 Installation

### 1. Clone the Repository

```bash
# Clone the repo
git clone https://github.com/Acurioustractor/[REPO_NAME].git
cd [REPO_NAME]
```

---

### 2. Run Setup Script

The setup script will:
- Install dependencies
- Create environment file
- Link Claude skills
- Set up database (if applicable)

```bash
# Make script executable (if needed)
chmod +x scripts/setup.sh

# Run setup
./scripts/setup.sh
```

**Or set up manually**:

```bash
# Install dependencies
npm install

# Copy environment template
cp .env.example .env.local

# Edit with your values
nano .env.local  # or use your preferred editor
```

---

### 3. Configure Environment Variables

Edit `.env.local` with your actual values:

```bash
# Required variables (example)
DATABASE_URL=postgresql://user:password@localhost:5432/dbname
API_KEY=your_api_key_here
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

See [Environment Setup Guide](./env-setup.md) for detailed configuration.

---

### 4. Start Development Server

```bash
# Start the dev server
npm run dev
```

The application should now be running at:
- **Web**: http://localhost:3000 (or configured port)
- **API**: http://localhost:3000/api (if applicable)

---

## ✅ Verify Installation

### 1. Run Health Check

```bash
# Check project health
./scripts/health-check.sh
```

This validates:
- Dependencies installed correctly
- Environment configured
- Database connected (if applicable)
- All required files present

---

### 2. Run Tests (if available)

```bash
# Run test suite
npm test

# Run with coverage
npm test -- --coverage
```

---

## 🎯 First Steps

### Explore the Application

1. **Homepage**: Navigate to http://localhost:3000
2. **[Feature 1]**: [Description and where to find it]
3. **[Feature 2]**: [Description and where to find it]

---

### Project Structure

```
/
├── src/              # Source code
│   ├── app/          # Pages and routes (Next.js)
│   ├── components/   # React components
│   ├── lib/          # Utilities and helpers
│   └── types/        # TypeScript types
├── docs/             # Documentation (you are here!)
├── scripts/          # Utility scripts
├── .claude/          # Claude AI skills
└── public/           # Static assets
```

See [Architecture Overview](../architecture/overview.md) for detailed structure.

---

### Common Commands

```bash
# Development
npm run dev           # Start dev server
npm run build         # Build for production
npm run start         # Start production server

# Code Quality
npm run lint          # Lint code
npm run type-check    # TypeScript type checking
npm test              # Run tests

# Database (if applicable)
npm run db:migrate    # Run migrations
npm run db:seed       # Seed database
npm run db:types      # Generate TypeScript types

# Utilities
./scripts/health-check.sh  # Check project health
```

---

## 🤖 Using Claude AI Assistance

This project includes Claude Code skills for AI-assisted development.

### Available Skills

```bash
# Brand alignment and content
/act-brand-alignment

# [Add other skills relevant to this project]
```

### Learn More
- [CLAUDE.md](../../CLAUDE.md) - Project context for Claude
- [.claude/SKILLS_GUIDE.md](../../.claude/SKILLS_GUIDE.md) - Skills documentation

---

## 📚 Next Steps

### For Developers

1. **Read Documentation**
   - [Architecture Overview](../architecture/overview.md)
   - [Development Setup](../development/setup.md)
   - [Coding Standards](../development/coding-standards.md)

2. **Explore Features**
   - [Feature Documentation](../features/)
   - Try making a small change
   - Run tests to verify

3. **Make Your First Contribution**
   - Find a "good first issue"
   - Read [CONTRIBUTING.md](../../CONTRIBUTING.md)
   - Submit a PR!

---

### For Users

1. **Learn the Interface**
   - [User Guide](../user-guide/) (if applicable)
   - Try core features
   - Explore settings

2. **Customize**
   - Configure preferences
   - Set up integrations
   - Personalize workspace

---

## 🐛 Troubleshooting

### Common Issues

#### Dependencies Won't Install
```bash
# Clear npm cache
npm cache clean --force

# Delete node_modules and reinstall
rm -rf node_modules package-lock.json
npm install
```

#### Port Already in Use
```bash
# Find process using port 3000
lsof -i :3000

# Kill the process
kill -9 <PID>

# Or use a different port
PORT=3001 npm run dev
```

#### Environment Variables Not Loading
- Ensure `.env.local` exists (not `.env`)
- Check file name is exact (case-sensitive)
- Restart dev server after changes
- For Next.js: prefix public vars with `NEXT_PUBLIC_`

#### Database Connection Errors
- Verify DATABASE_URL is correct
- Ensure database server is running
- Check credentials and permissions
- Try running migrations: `npm run db:migrate`

---

### Still Stuck?

1. **Check Documentation**: [docs/](../)
2. **Run Health Check**: `./scripts/health-check.sh`
3. **Search Issues**: [GitHub Issues](https://github.com/Acurioustractor/[REPO_NAME]/issues)
4. **Ask for Help**: Create a new issue

---

## 🌾 ACT Ecosystem

This project is part of the ACT Regenerative Innovation Ecosystem.

### LCAA Method
- **Listen** - Deep listening to community and place
- **Curiosity** - Prototype boldly, test rigorously
- **Action** - Build tangible solutions
- **Art** - Translate change into culture

### Related Projects
- [ACT Main](https://github.com/Acurioustractor/act-regenerative-studio)
- [Empathy Ledger](https://github.com/Acurioustractor/empathy-ledger-v2)
- [JusticeHub](https://github.com/Acurioustractor/justicehub-platform)

---

## 📖 Additional Resources

- [Environment Setup](./env-setup.md) - Detailed environment configuration
- [Deployment Guide](./deploy.md) - Deploy to production
- [API Documentation](../architecture/api-design.md) - API reference
- [Contributing Guide](../../CONTRIBUTING.md) - How to contribute

---

## 🙋 Getting Help

- **Documentation**: Check [docs/README.md](../README.md)
- **Issues**: [GitHub Issues](https://github.com/Acurioustractor/[REPO_NAME]/issues)
- **Discussions**: [GitHub Discussions](https://github.com/Acurioustractor/[REPO_NAME]/discussions)

---

**Last Updated**: [YYYY-MM-DD]
**Questions?** Create an issue or reach out to maintainers!

🌾 Happy building! 🌾
