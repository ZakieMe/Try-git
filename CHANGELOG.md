# Changelog

All notable changes to **AchievementForge** will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

### Added
- GitHub Discussions integration for Galaxy Brain achievement
- Contributor spotlight section
- Discord community server link

### Planned
- GitHub API live stats integration
- Personal achievement tracker
- Achievement progress export to JSON

---

## [1.2.0] — 2024-11-15

### Added
- Roadmap section with 5-phase project phases
- Phase card status indicators (completed, in-progress, planned)
- `SECURITY.md` security policy document

### Changed
- Improved scroll reveal animation performance using IntersectionObserver
- Achievement card layout refinement on tablet breakpoints

### Fixed
- Filter tab active state not clearing on fast double-click
- Timeline connector line gradient misalignment on Firefox

---

## [1.1.0] — 2024-09-20

### Added
- Achievement filter tabs (All, Earned, In Progress, Available, Legacy)
- Animated progress bars for tiered achievements (Pull Shark, Starstruck, etc.)
- Tier chip badges (Bronze / Silver / Gold) with completion indicators
- Timeline section with 10 development milestones
- `Co-authored-by` commit strategy documentation

### Changed
- Hero particle canvas rewritten for better performance and mobile support
- Stats counters now animate only when scrolled into view
- Dark mode toggle now persists preference across sessions via localStorage

### Fixed
- Hero canvas overflow causing horizontal scroll on mobile
- Stat counter animation not triggering on iOS Safari

---

## [1.0.0] — 2024-08-01

### Added
- Initial public release of AchievementForge
- Hero section with animated particle canvas and grid background
- Achievement showcase grid for all 11 GitHub achievements
- Stats strip with animated counters (Achievements, Stars, PRs, Contributors)
- Dark mode (default) with light mode toggle
- Responsive layout for mobile, tablet, and desktop
- Professional navigation with scroll-aware border
- CTA section and footer
- `README.md` with full documentation
- `CONTRIBUTING.md` with detailed guide
- `CODE_OF_CONDUCT.md` (Contributor Covenant v2.1)
- MIT License

### Achievement Data Included
- 🦈 Pull Shark (Bronze / Silver / Gold tiers)
- 🤠 YOLO
- ⚡ Quickdraw
- 🧑‍💻 Pair Extraordinaire (Bronze / Silver / Gold tiers)
- 🌌 Galaxy Brain (Bronze / Silver / Gold tiers)
- ⭐ Starstruck (Bronze / Silver / Gold tiers)
- 💝 Heart On Your Sleeve
- 🧙 Open Sourcerer (Bronze / Silver / Gold tiers)
- 💖 Public Sponsor
- 🌐 Arctic Code Vault Contributor (Legacy)
- 🚁 Mars 2020 Helicopter Contributor (Legacy)

---

## [0.3.0] — 2024-07-10

### Added
- Achievement card component with shimmer effect for earned cards
- Dark/light mode CSS custom properties system
- Google Fonts integration (Rajdhani, JetBrains Mono, Nunito Sans)
- Floating emoji animation on achievement card icons

### Changed
- Refactored CSS to use design tokens throughout
- Improved card hover states with color-matched glow effects

---

## [0.2.0] — 2024-06-22

### Added
- Hero section with canvas particle animation
- Responsive navigation with theme toggle button
- Stats section with 4 stat cards

### Fixed
- Canvas particle overflow on small screens

---

## [0.1.0] — 2024-06-05

### Added
- Initial repository creation
- Basic HTML scaffold
- `README.md` placeholder
- MIT License
- `.gitignore`

---

[Unreleased]: https://github.com/yourusername/AchievementForge/compare/v1.2.0...HEAD
[1.2.0]: https://github.com/yourusername/AchievementForge/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/yourusername/AchievementForge/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/yourusername/AchievementForge/compare/v0.3.0...v1.0.0
[0.3.0]: https://github.com/yourusername/AchievementForge/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/yourusername/AchievementForge/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/yourusername/AchievementForge/releases/tag/v0.1.0
