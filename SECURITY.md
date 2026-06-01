# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| 1.2.x   | ✅ Yes |
| 1.1.x   | ✅ Yes |
| 1.0.x   | ⚠️ Critical fixes only |
| < 1.0   | ❌ No |

## Reporting a Vulnerability

If you discover a security vulnerability in AchievementForge, please report it **privately** — do not open a public issue.

### How to Report

**Option 1 — GitHub Private Vulnerability Reporting (Preferred)**
Use GitHub's [private vulnerability reporting](../../security/advisories/new) feature.

**Option 2 — Email**
Send details to: `security@yourdomain.com`

Include:
- Type of issue (e.g. XSS, data exposure, dependency vulnerability)
- File paths related to the issue
- Steps to reproduce
- Proof of concept (if possible)
- Potential impact

### Response Timeline

| Stage | Timeline |
|-------|----------|
| Acknowledgement | Within 48 hours |
| Initial assessment | Within 7 days |
| Fix or mitigation | Within 30 days |
| Public disclosure | After fix is released |

We appreciate responsible disclosure and will credit reporters in the changelog (if desired).

## Security Considerations

AchievementForge is a **static website** with no backend, no database, and no user data collection. It uses:

- No server-side processing
- No authentication or sessions
- No external API calls (planned features will use GitHub's public API only)
- `localStorage` only for theme preference (no personal data)

The attack surface is minimal by design.
