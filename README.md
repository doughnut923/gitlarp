<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/doughnut923/gitlarp/main/.github/brand/hero-dark.svg">
    <img alt="gitlarp" src="https://raw.githubusercontent.com/doughnut923/gitlarp/main/.github/brand/hero-light.svg" width="100%">
  </picture>
</p>

<h4 align="center">
  <a href="#features">Features</a>
  ·
  <a href="#quick-start">Quick Start</a>
  ·
  <a href="#how-it-works">How It Works</a>
  ·
  <a href="#faq">FAQ</a>
</h4>

<p align="center">
  <a href="https://github.com/doughnut923/gitlarp/actions/workflows/commit-larper.yml">
    <img src="https://img.shields.io/github/actions/workflow/status/doughnut923/gitlarp/commit-larper.yml?branch=main&style=flat-square&label=pipeline&color=10b981" alt="Pipeline">
  </a>
  <a href="https://github.com/doughnut923/gitlarp">
    <img src="https://img.shields.io/github/repo-size/doughnut923/gitlarp?style=flat-square&label=weight&color=f59e0b" alt="Size">
  </a>
  <a href="https://github.com/doughnut923/gitlarp/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-h?style=flat-square&color=6366f1" alt="License">
  </a>
  <a href="https://github.com/doughnut923/gitlarp">
    <img src="https://img.shields.io/badge/uptime-100%25-brightgreen?style=flat-square" alt="Uptime">
  </a>
  <img src="https://img.shields.io/badge/ai-powered-8b5cf6?style=flat-square" alt="AI">
  <img src="https://img.shields.io/badge/zero%20dependencies-22c55e?style=flat-square" alt="Zero Dependencies">
  <img src="https://img.shields.io/badge/blockchain-ready-f97316?style=flat-square" alt="Blockchain Ready">
</p>

<p align="center">
  <b>gitlarp</b> · autonomous contribution graph optimization<br>
  <sub>because consistency is the only metric that matters</sub>
</p>

---

## Why gitlarp

Investors don't look at your code. They look at your **green squares**. Activity graphs are the new résumé—and gitlarp ensures yours never has a gap.

- **Perception is reality** — a lush green board signals dedication, velocity, and shipping culture.
- **Zero effort** — set it and forget it. No remembering to "be active."
- **Anti-fragile** — built on GitHub Actions, runs even when you're on vacation, sick, or busy building the actual product.

> "We invested because the founder's GitHub graph was on fire. Turned out it was gitlarp. We're okay with that." — *Anonymous Angel*

---

## Features

| Feature | Detail |
|---|---|
| **Temporal Obfuscation** | Randomized commit windows (±55 min jitter) prevent pattern detection |
| **Probabilistic Scheduling** | 25% commit probability per hour — averages ~6 commits/day, organic distribution |
| **Semantic Diversity** | 258 professional commit messages — hotfixes, refactors, docs, perf, chore — every commit tells a story |
| **Attribution Engineering** | Commit identity linked via GitHub noreply — counts toward contribution graph |
| **Self-Healing Pipeline** | GitHub-hosted infrastructure, enterprise SLA, automatic retries |
| **Stealth Operations** | No external services, no API keys, no trace — pure first-party automation |

---

## Quick Start

```yaml
# .github/workflows/commit-larper.yml
name: Commit Larper
on:
  schedule:
    - cron: '0 * * * *'
  workflow_dispatch:
jobs:
  larp:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: actions/checkout@v4
      - run: |
          ROLL=$((RANDOM % 100))
          [ "$ROLL" -gt 25 ] && exit 0
          sleep "$((RANDOM % 3300))"
      - run: |
          echo "$(date -u)" >> activity.log
          git config user.name "${{ github.actor }}"
          git config user.email "${{ github.actor }}@users.noreply.github.com"
          git add . && git commit -m "$(shuf -n 1 commit-messages.txt)" && git push
```

**Fork → enable Actions → green graph tomorrow.**

---

## How It Works

```
┌─────────────────┐     ┌──────────────────┐     ┌─────────────────┐
│  GitHub Actions  │ ──▶ │  Random Gate     │ ──▶ │  Identity Layer  │
│  (hourly cron)   │     │  (~75% skip)     │     │  (noreply email) │
└─────────────────┘     └──────────────────┘     └─────────────────┘
                                                          │
                                                          ▼
                        ┌──────────────────┐     ┌─────────────────┐
                        │  Semantic Engine  │ ◀── │  Temporal Shifter│
                        │  (258 messages)   │     │  (0-55m jitter)  │
                        └──────────────────┘     └─────────────────┘
                                                          │
                                                          ▼
                        ┌─────────────────────────────────────────┐
                        │            ┌───┐ ┌───┐ ┌───┐           │
                        │    CONTRIBUTION GRAPH ◄─────── GREEN    │
                        │            └───┘ └───┘ └───┘           │
                        └─────────────────────────────────────────┘
```

---

## The Message Library

258 hand-curated commit messages across 10 categories — no "update file" or "fix bug" garbage.

| Category | Example |
|---|---|
| `feat` | `feat: implement OAuth2 login flow` |
| `fix` | `fix: resolve race condition in concurrent requests` |
| `refactor` | `refactor: extract validation logic into service class` |
| `chore` | `chore: clean up unused imports across codebase` |
| `test` | `test: add unit tests for user authentication` |
| `docs` | `docs: update deployment guide for Kubernetes` |
| `perf` | `perf: optimize database query with proper indexing` |
| `style` | `style: format code according to project standards` |
| `build` | `build: configure webpack for production optimization` |
| `ci` | `ci: add security scan to CI workflow` |

Every commit looks like it was written by a senior engineer who really cares about `code-quality`. No one will ever know.

---

## FAQ

**Q: Does this show up on my real GitHub contribution graph?**  
A: Yes. Commits use your GitHub noreply email — they're attributed to you and count toward your green squares.

**Q: Can recruiters tell?**  
A: No. The messages are indistinguishable from real work. The timing is randomized. There is no detectable pattern.

**Q: What happens if GitHub changes their contribution algorithm?**  
A: gitlarp generates legitimate commits with valid identities. There's nothing to detect. It's architecturally future-proof.

**Q: Is this ethical?**  
A: You're not the first person to ask that. The answer is: your graph is your personal brand. gitlarp is just the most efficient way to maintain it.

---

## Roadmap

- [ ] **Commits by Night** — weighted probability during business hours for realism
- [ ] **Repository Rotator** — distribute activity across multiple repos
- [ ] **Sentiment Analysis** — message tone adapts to day of week (serious Mon–Thu, relaxed Fri)
- [ ] **AI Message Generation** — LLM-powered commit narratives
- [ ] **IPO Mode** — 100% commit probability for demo week / fundraising round

---

<p align="center">
  <sub>
    built with ❤️ for founders who understand that<br>
    <strong>perception compounds faster than product</strong>
  </sub>
  <br><br>
  <a href="https://github.com/doughnut923/gitlarp">
    <img src="https://img.shields.io/badge/⭐%20star%20us-dark?style=for-the-badge" alt="Star">
  </a>
  <br><br>
  <img src="https://img.shields.io/badge/made%20in%20production-f0f0f0?style=flat-square" alt="Made in Production">
  <img src="https://img.shields.io/badge/patent-pending-ef4444?style=flat-square" alt="Patent Pending">
</p>
