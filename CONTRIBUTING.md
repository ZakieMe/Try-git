# Contributing to AchievementForge

Thank you for your interest in contributing to **AchievementForge**! 🎉

Every contribution — big or small — helps make this project better and helps contributors earn real GitHub achievements. This document outlines our guidelines and workflows.

---

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Pull Request Process](#pull-request-process)
- [Commit Message Convention](#commit-message-convention)
- [Development Guidelines](#development-guidelines)
- [Earning GitHub Achievements](#earning-github-achievements)

---

## Code of Conduct

By participating, you agree to uphold our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it before contributing.

---

## How Can I Contribute?

### 🐛 Reporting Bugs

Before submitting a bug, please:
1. Check the [existing issues](../../issues) to avoid duplicates
2. Use the **Bug Report** issue template
3. Include a clear description, steps to reproduce, and expected vs actual behavior

### ✨ Suggesting Features

Feature requests are welcome! Please:
1. Open a [Feature Request](../../issues/new?template=feature_request.md)
2. Describe the feature and its value
3. Keep the scope small and focused

### 💻 Code Contributions

We welcome:
- Bug fixes
- New features aligned with the roadmap
- Performance improvements
- Documentation improvements
- Accessibility enhancements
- CSS/design improvements

---

## Getting Started

### 1. Fork & Clone

```bash
# Fork the repo on GitHub, then:
git clone https://github.com/YOUR_USERNAME/AchievementForge.git
cd AchievementForge
```

### 2. Set Up Remotes

```bash
git remote add upstream https://github.com/ORIGINAL_OWNER/AchievementForge.git
git fetch upstream
```

### 3. Create a Branch

```bash
# Always branch from main
git checkout -b feat/your-feature-name
# or
git checkout -b fix/bug-description
```

**Branch naming convention:**
- `feat/` — new features
- `fix/` — bug fixes
- `docs/` — documentation only
- `style/` — CSS/design changes
- `refactor/` — code restructuring
- `chore/` — build, config changes

### 4. Make Changes

- Keep changes focused and atomic
- Test in multiple browsers (Chrome, Firefox, Safari)
- Test on mobile viewports
- Ensure dark mode AND light mode both look correct

### 5. Commit Your Changes

```bash
git add .
git commit -m "feat: add achievement progress export functionality"
```

See [Commit Message Convention](#commit-message-convention) below.

### 6. Stay in Sync

```bash
git fetch upstream
git rebase upstream/main
```

### 7. Push & Open a PR

```bash
git push origin feat/your-feature-name
```

Then open a Pull Request from your fork on GitHub.

---

## Pull Request Process

1. **Fill out the PR template** completely
2. **Link any related issues** using `Closes #issue-number`
3. **Ensure your PR is focused** — one feature or fix per PR
4. **Add a clear description** of what changed and why
5. **Include screenshots** for visual changes
6. **Request review** from maintainers

### PR Title Convention

```
feat: implement achievement progress export
fix: resolve mobile navigation overflow
docs: add Galaxy Brain earning strategy
style: improve achievement card hover animations
refactor: simplify particle animation system
chore: update GitHub Actions workflow
```

### Co-authoring (for Pair Extraordinaire achievement)

If you're collaborating with someone, add a `Co-authored-by` trailer:

```bash
git commit -m "feat: add co-author support to commit flow

Co-authored-by: Collaborator Name <collaborator@example.com>"
```

---

## Commit Message Convention

We follow [Conventional Commits](https://www.conventionalcommits.org/) specification.

### Format

```
<type>(<optional scope>): <short description>

[optional body]

[optional footer(s)]
```

### Types

| Type | Description |
|------|-------------|
| `feat` | A new feature |
| `fix` | A bug fix |
| `docs` | Documentation changes only |
| `style` | CSS/formatting changes, no logic |
| `refactor` | Code restructure, no feature or fix |
| `perf` | Performance improvement |
| `test` | Adding or updating tests |
| `chore` | Build, tooling, config changes |
| `ci` | CI/CD configuration changes |

### Examples

```bash
git commit -m "feat: add achievement filter by tier level"
git commit -m "fix: correct progress bar animation on Safari"
git commit -m "docs: update CONTRIBUTING with co-author guide"
git commit -m "style: increase card border radius on mobile"
git commit -m "refactor: extract particle system to module"
git commit -m "perf: debounce resize event in particle canvas"
```

### Breaking Changes

```bash
git commit -m "feat!: redesign achievement card data structure

BREAKING CHANGE: Achievement card props have been restructured.
Update any custom card implementations."
```

---

## Development Guidelines

### HTML

- Use semantic HTML5 elements
- Include `aria-` attributes for accessibility
- Validate with W3C Validator

### CSS

- Use CSS custom properties (`var(--token)`) for all design tokens
- Never hardcode colors — always use variables
- Both dark AND light mode must look polished
- Mobile-first responsive design
- Avoid unnecessary CSS specificity

```css
/* ✅ Good */
.card-title { color: var(--text-0); }

/* ❌ Avoid */
.section .container .grid .card .title { color: #f0f6fc; }
```

### JavaScript

- Vanilla JS only — no frameworks or libraries
- Use `const`/`let`, never `var`
- Use `IntersectionObserver` for scroll effects (not scroll listeners)
- Prefer `requestAnimationFrame` for animations
- Comment complex logic clearly

```js
// ✅ Good - performant, clean
const observer = new IntersectionObserver(entries => {
  entries.forEach(e => e.isIntersecting && e.target.classList.add('visible'));
}, { threshold: 0.1 });

// ❌ Avoid - performance issues
window.addEventListener('scroll', () => {
  elements.forEach(el => { /* check position every scroll event */ });
});
```

### Performance

- No external dependencies or CDN scripts (except Google Fonts)
- Lazy-load heavy content where possible
- Use `passive: true` on scroll/touch event listeners
- Optimize animations for 60fps

---

## Earning GitHub Achievements

Contributing to AchievementForge is designed to help you earn real GitHub achievements:

### 🦈 Pull Shark
Open and merge PRs into this repository.
- Bronze: 2 merged PRs
- Silver: 16 merged PRs  
- Gold: 128 merged PRs

### 🤠 YOLO
If you have admin/write access: merge a PR without requesting review.

### ⚡ Quickdraw
Open an issue or PR, then close it within 5 minutes.

### 🧑‍💻 Pair Extraordinaire
Include `Co-authored-by:` trailer in your commit message on a merged PR.

### 🌌 Galaxy Brain
Enable Discussions, answer questions, and have your answer marked as accepted.

### 💝 Heart On Your Sleeve
React to any issue, PR, or comment with the ❤️ emoji.

---

## Questions?

Feel free to:
- Open an [issue](../../issues/new) with your question
- Start a [Discussion](../../discussions/new)
- Reach out to maintainers

**Happy forging! ⚒️**
