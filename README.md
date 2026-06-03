<div align="center">
  <img src="./logo.svg" alt="env-var-manager" width="120" />
  <h1>Env Variable Manager</h1>
  <p>Encrypted environment variable manager using AES-GCM encryption via Web Crypto API. Manage dev/staging/prod .env files securely in the browser.</p>

  ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
  ![License: MIT](https://img.shields.io/badge/license-MIT-blue?style=flat)
  ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat)
</div>

---

## Overview

Encrypted environment variable manager using AES-GCM encryption via Web Crypto API. Manage dev/staging/prod .env files securely in the browser.

Built as a single-file HTML application — no build tools, no frameworks, no external dependencies. Just open `index.html` in any modern browser.

## Features

- AES-GCM encryption via Web Crypto API (PBKDF2 key derivation)
- Passphrase-protected access — nothing stored in plaintext
- Three environments: Development, Staging, Production
- Copy individual values to clipboard
- Side-by-side environment diff viewer
- Zero external dependencies — single HTML file

## Quick Start

1. Clone the repository
2. Open `index.html` in your browser
3. Enter a passphrase to unlock (first time creates a new vault)
4. Start adding environment variables

```bash
git clone https://github.com/soumendrak/env-var-manager.git
cd env-var-manager
open index.html
```

## Project Structure

```
env-var-manager/
├── index.html    # The complete application
├── LICENSE       # MIT License
└── README.md     # This file
```

## Security

- Uses AES-256-GCM encryption via the browser's native Web Crypto API
- Encryption key derived from passphrase using PBKDF2 (200,000 iterations, SHA-256)
- Encrypted data stored in localStorage
- Nothing transmitted over the network — all crypto happens locally

## Dark Theme

All projects in this suite share a consistent dark theme:

| Token | Color | Usage |
|-------|-------|-------|
| `--bg` | `#0f0f1a` | Page background |
| `--surface` | `#1a1a2e` | Cards, headers, panels |
| `--accent` | `#ff6b35` | Buttons, highlights, borders |
| `--text` | `#e0e0e0` | Body text |

## Contributing

Contributions welcome! Open an issue or submit a PR.

## License

MIT © [Soumendra Kumar Sahoo](https://github.com/soumendrak)
