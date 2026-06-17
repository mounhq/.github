<div align="center">

<img src="https://raw.githubusercontent.com/mcnulabs/.github/main/profile/nabla.svg" alt="∇" width="120" />

# ∇ MCNU Labs

**Follow the gradient.**

Small, self-hosted tools — privacy-first, dark by default, no telemetry you didn't ask for.
One identity across every surface: the pixel **∇** is the monogram, the cyan→violet **gradient** is the thesis.

[![site](https://img.shields.io/badge/mcnu.ro-22D3EE?style=flat-square&labelColor=0A0E1A&color=22D3EE)](https://mcnu.ro)
[![self-hosted](https://img.shields.io/badge/self--hosted-A78BFA?style=flat-square&labelColor=0A0E1A&color=A78BFA)](https://github.com/mcnulabs)
[![license MIT](https://img.shields.io/badge/license-MIT-A78BFA?style=flat-square&labelColor=0A0E1A&color=A78BFA)](#license)

</div>

---

## ∇ What we build

MCNU Labs is a family of small, focused, **self-hostable** web services. Each one does a single
job well, ships **dark-first**, and refuses to track you: no cookies, no fingerprinting, no
IP storage, no consent banners. One tiny script or one SQLite file — not a platform.

The whole family shares one **design system** so every property looks like it belongs to the
same world: cyan + violet on a near-black ink background, the Press Start 2P pixel face for
labels, Inter for everything readable, JetBrains Mono for code.

## ∇ The family

| | Service | What it does | Live |
|---|---|---|---|
| **📊** | [**mcnu-analytics**](https://github.com/mcnulabs/mcnu-analytics) | Privacy-first web analytics. No cookies, no fingerprinting, no IP storage, no consent banner. One tiny script, one SQLite file. | — |
| **🔗** | [**mcnu-go**](https://github.com/mcnulabs/mcnu-go) | Self-hosted URL shortener with privacy-first click analytics. Auto codes or custom aliases, per-link stats. | [l.mcnu.ro](https://l.mcnu.ro) |
| **📋** | [**mcnu-paste**](https://github.com/mcnulabs/mcnu-paste) | Self-hosted pastebin. Syntax highlight, expiry, burn-after-read, raw + download. You write, anyone reads via link. | [p.mcnu.ro](https://p.mcnu.ro) |
| **⌘** | [**mcnu-snippets**](https://github.com/mcnulabs/mcnu-snippets) | Private command/snippet library. Instant search, tags, and placeholders filled at copy time. | [s.mcnu.ro](https://s.mcnu.ro) |
| **📝** | [**mcnu-md**](https://github.com/mcnulabs/mcnu-md) | Anything → Markdown. PDF, Word, Excel, PowerPoint, HTML, CSV → clean Markdown. No sign-up, nothing stored. | [md.mcnu.ro](https://md.mcnu.ro) |
| **🛰️** | [**mcnu-console**](https://github.com/mcnulabs/mcnu-console) | Private hub for every MCNU service. One login, one page: live status + key numbers. | — |
| **🚀** | [**mcnu-deploy**](https://github.com/mcnulabs/mcnu-deploy) | One command to deploy any MCNU service safely: rsync → perms → validate → backup → restart → health-check. | — |
| **💾** | [**mcnu-backup**](https://github.com/mcnulabs/mcnu-backup) | Daily, encrypted, off-site backups of every service's secrets and databases. gpg AES256 → B2 → rotated, with a tested restore. | — |
| **🎨** | [**mcnu-design-system**](https://github.com/mcnulabs/mcnu-design-system) | The shared identity: tokens, components, and the living styleguide every property is built on. | — |

## ∇ The four laws

Everything we ship obeys the same rules — that's why it all feels like one thing:

1. **Nabla primary, candy secondary.** Cyan `#22D3EE` + violet `#A78BFA` on dark for anything rigorous. Candy `#FF2E63` only for social / swag / recruiting.
2. **Dark-first.** We ship dark. Light mode is an opt-in for print and docs; semantic tokens remap automatically.
3. **The pixel face is for labels only.** Press Start 2P sets the monogram, eyebrows, and short labels — never body. Inter is everything readable; JetBrains Mono is code/data.
4. **Accessibility floor.** Visible focus ring on every interactive element, AA contrast, full keyboard reach, `prefers-reduced-motion` respected.

## ∇ The palette

<div align="center">

| | Token | Hex | Role |
|---|---|---|---|
| ![](https://img.shields.io/badge/-22D3EE?style=flat-square&color=22D3EE) | `--mc-cyan` | `#22D3EE` | Primary accent — rigour |
| ![](https://img.shields.io/badge/-A78BFA?style=flat-square&color=A78BFA) | `--mc-violet` | `#A78BFA` | Secondary accent |
| ![](https://img.shields.io/badge/-FF2E63?style=flat-square&color=FF2E63) | `--mc-candy` | `#FF2E63` | Comms only — social/swag |
| ![](https://img.shields.io/badge/-0A0E1A?style=flat-square&color=0A0E1A) | `--mc-ink` | `#0A0E1A` | Background |
| ![](https://img.shields.io/badge/-E6ECF7?style=flat-square&color=E6ECF7) | `--mc-text` | `#E6ECF7` | Primary text |

**The gradient** — `linear-gradient(135deg, #22D3EE, #A78BFA)` — is the one thing to be remembered on a surface. Never wallpaper.

</div>

## ∇ Self-hosting, the MCNU way

Every service is a small Node app backed by SQLite — clone, configure `.env`, run.
Deployments are reproducible and boring on purpose:

```
mcnu-deploy  →  rsync → fix perms → ensure .data → validate .env
             →  npm ci (only if deps changed) → backup → restart → health-check
```

Want the shared look on your own page? Pull in the tokens and components from the design system:

```html
<link rel="stylesheet" href="/brand/tokens.css">  <!-- single source of truth, import first -->
<link rel="stylesheet" href="/brand/mcnu.css">     <!-- .mc-* components, import second -->
```

## ∇ License

Open source under the **MIT** license — see each repository for details.

<div align="center">

<br>

**∇ follow the gradient ∇**

</div>
