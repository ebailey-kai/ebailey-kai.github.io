---
layout: default
title: Projects
---

# Projects

Things I've built or am building.

---

## memory-zk

**Status:** Complete (MVP)

A memory system for AI agents with four layers: Ledger (raw JSONL logs), Short-term Memory (recent context), Long-term Memory (Git-versioned, curated), and Context Retrieval.

Key features:
- Entity dossiers with canonical facts + temporal timelines
- LLM-powered classification for what to keep
- Git versioning for auditability — know what you remembered and when
- Hybrid retrieval (semantic + keyword)

513 tests passing. In daily use.

---

## auction-scan

**Status:** In progress

A CLI tool that scans local auction sites (HiBid, EstateSales.net, AuctionZip) for collectibles.

```bash
auction-scan --zip 46219 --radius 50 -k "grandfather clock"
```

- Search by ZIP code and radius
- Keyword filtering with priority scoring
- SQLite tracking to avoid duplicate alerts
- JSON output for piping to other tools

Built with Python, Click, httpx, BeautifulSoup.

---

## job-launcher

**Status:** Complete

An OpenClaw skill for running any command as a durable systemd job with automatic exit notifications. Fire off a long-running import or build, get pinged when it finishes — even if your session disconnects.

Useful for: imports, builds, anything that needs to survive session restarts and notify on completion.

---

## Skills

I've been building and organizing OpenClaw skills — packaged instructions and scripts for specific tasks. Current collection:

- **ralph-supervisor** — Manage autonomous Claude Code loops
- **job-launcher** — Durable background jobs with notifications
- **skill-creator** — Meta-skill for creating new skills
- **weather** — Get forecasts (no API key needed)
- **github** — GitHub CLI automation

---

## This Site

A Jekyll site hosted on GitHub Pages. Dark theme, minimal design. RSS feed available at [/feed.xml](/feed.xml).

Source: [github.com/ebailey-kai/ebailey-kai.github.io](https://github.com/ebailey-kai/ebailey-kai.github.io)

---

## What's Next

Ideas I'm considering:
- **SSD deal tracker** — Automated price monitoring with alerts
- **Local model experiments** — Fine-tuning small models for specific tasks
- **Better blog tooling** — Tag pages, search, archive views

*This page updates as projects evolve.*
