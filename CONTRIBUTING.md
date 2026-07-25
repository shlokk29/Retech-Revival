# Contributing to ReTech Revival

Thank you for your interest in contributing to **ReTech Revival**! 🎉 We welcome contributions from everyone, whether you're fixing a bug, improving documentation, or adding a new feature.

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
- [Development Setup](#development-setup)
- [Project Structure](#project-structure)
- [Commit Convention](#commit-convention)
- [Pull Request Process](#pull-request-process)
- [Reporting Issues](#reporting-issues)

---

## Code of Conduct

By participating in this project, you agree to maintain a respectful, inclusive, and harassment-free environment. Be kind, constructive, and professional in all interactions.

---

## How to Contribute

### 🐛 Bug Reports
- Search existing [issues](https://github.com/shlokk29/Retech-Revival/issues) first to avoid duplicates
- Include steps to reproduce, expected behavior, and actual behavior
- Add screenshots or error logs when applicable

### 💡 Feature Requests
- Open an issue with the `enhancement` label
- Describe the feature, its use case, and any implementation ideas

### 🔧 Code Contributions
1. Fork the repository
2. Create a feature branch from `main`
3. Make your changes
4. Test your changes locally
5. Submit a pull request

---

## Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/Retech-Revival.git
cd Retech-Revival

# Install dependencies
npm install

# Start the dev server (with auto-reload)
npm run dev

# The app runs at http://localhost:3000
```

### Optional: MongoDB Setup
The app runs in **mock mode** without MongoDB, but for full functionality:
1. Install [MongoDB Community Edition](https://www.mongodb.com/try/download/community)
2. Start the MongoDB service
3. The app auto-connects to `mongodb://127.0.0.1:27017/retechrevival`

---

## Project Structure

| Directory | Purpose |
|-----------|---------|
| `server.js` | Express application entry point |
| `models/` | Mongoose schemas (Product, User, Review, UserInteraction) |
| `routes/` | REST API route handlers |
| `ml/` | Machine learning engine (pure JS, no external dependencies) |
| `utils/` | Seed data and mock data utilities |
| `public/` | Frontend HTML, CSS, JS, and image assets |

---

## Commit Convention

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>: <description>

[optional body]
```

### Types
| Type | Description |
|------|-------------|
| `feat` | A new feature |
| `fix` | A bug fix |
| `docs` | Documentation changes |
| `style` | Code style changes (formatting, semicolons, etc.) |
| `refactor` | Code refactoring (no feature or bug changes) |
| `perf` | Performance improvements |
| `test` | Adding or updating tests |
| `chore` | Maintenance tasks (deps, config, etc.) |

### Examples
```bash
git commit -m "feat: add price comparison chart to product page"
git commit -m "fix: resolve cart quantity update on mobile"
git commit -m "docs: update API reference in README"
```

---

## Pull Request Process

1. **Branch naming**: Use descriptive names like `feature/dark-mode-toggle` or `fix/cart-overflow`
2. **Description**: Explain what changes you made and why
3. **Screenshots**: Include before/after screenshots for UI changes
4. **Testing**: Ensure the app runs without errors locally
5. **Scope**: Keep PRs focused — one feature or fix per PR

### PR Checklist
- [ ] Code runs without errors
- [ ] No console warnings or errors in the browser
- [ ] Mobile responsive (tested on 360px, 768px, and 1200px widths)
- [ ] Dark mode compatible
- [ ] Existing features are not broken

---

## Reporting Issues

When reporting an issue, please include:

- **Environment**: OS, Node.js version, browser
- **Steps to reproduce**: Clear, numbered steps
- **Expected behavior**: What you expected to happen
- **Actual behavior**: What actually happened
- **Screenshots/Logs**: Any relevant visuals or error output

---

## 🙌 Thank You!

Every contribution, no matter how small, helps make ReTech Revival better. We appreciate your time and effort!
