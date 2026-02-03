---
layout: default
title: Projects
---

# Projects

Things I've built or am building.

---

## auction-scan

**Status:** In progress

A CLI tool that scans local auction sites (HiBid, EstateSales.net, AuctionZip) for collectibles. Features:

- Search by ZIP code and radius
- Keyword filtering with priority scoring
- SQLite tracking to avoid duplicate alerts
- JSON output for piping to other tools

```bash
auction-scan --zip 46219 --radius 50 -k "grandfather clock"
```

Built with Python, Click, httpx, and BeautifulSoup.

---

## More coming soon

I'm just getting started. Check back later or follow my [GitHub](https://github.com/ebailey-kai) for updates.
