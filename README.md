# Wayhours

> Independent travel discovery & planning platform — **[wayhours.com](https://wayhours.com)**
> Information-only (no bookings): curated destination guides, editable itineraries, and verified entry requirements.

---

## About

Wayhours helps travelers research destinations and organize trips through curated content and interactive tools.

- **Destination Guides** — 38 guides across 17 countries (Tokyo, Bali, Singapore, Dubai, …)
- **Trip Planner** — editable day-by-day itineraries by destination, duration, and budget
- **Travel Guides** — 37 practical articles (packing, visas, costs, layover strategies)
- **Community Forum** — traveler discussions and seasonal trade-offs
- **Know Before You Go** — verified entry requirements and fees with official-source citations

**Primary sections:** Destinations · Trip Planner · Travel Guides · Community · Reviews

---

## SEO & GEO Playbook

Action checklist to grow organic traffic and get cited by AI answer engines (ChatGPT, Perplexity, Google AI Overviews, Claude).

### 1. Technical SEO (foundations)

- [ ] **Server-render / statically generate pages** so crawlers and AI bots see real HTML, not an empty JS shell *(highest-leverage item)*
- [ ] `sitemap.xml` (auto-generated) + `robots.txt`
- [ ] Canonical tags and clean, descriptive URLs (`/tokyo/3-day-itinerary`)
- [ ] Optimized images with descriptive `alt` text + lazy loading
- [ ] Pass Core Web Vitals (LCP, CLS, INP); minimize client-side JS
- [ ] Visible "Updated <Month Year>" date on every page (freshness signal)

### 2. Structured data (schema.org JSON-LD)

- [ ] `TouristDestination` + `TouristTrip` — destinations & itineraries
- [ ] `Article` with `author`, `datePublished`, `dateModified` — blogs
- [ ] `FAQPage` — "Know Before You Go" entry requirements
- [ ] `BreadcrumbList`, `Organization`, `ItemList` — hubs & navigation

### 3. Content & architecture

- [ ] **Topic-cluster model:** country hub → destination pillar → itineraries + articles, strongly interlinked
- [ ] Target long-tail intent: *"3 days in Tokyo itinerary"*, *"Bali on a budget 7 days"*, *"Dubai 8-hour layover"*
- [ ] Lead every page with a direct 2–3 sentence answer (extractable)
- [ ] E-E-A-T: author bios, and keep citing official sources with dates

### 4. GEO — get cited by AI answer engines

- [ ] **Allow AI crawlers** in `robots.txt`: `GPTBot`, `ClaudeBot`, `PerplexityBot`, `Google-Extended`, `CCBot`
- [ ] Add **`/llms.txt`** — a markdown index of your best pages for LLMs
- [ ] Use FAQ sections, tables (visa fees, costs, best time to visit), and specific numbers — AI engines lift structured facts
- [ ] Cite sources with dates (a primary GEO trust signal)
- [ ] Establish entity clarity: consistent brand name, `Organization` schema, and a Wikidata/Wikipedia presence

### 5. Off-page / authority

- [ ] Digital PR & backlinks (travel listicles, "best itinerary sites")
- [ ] RSS feed for syndication
- [ ] Google Business Profile + consistent social presence

---

## Content structure (recommended)

Store blogs and itineraries as Markdown with frontmatter so a build step can generate HTML, sitemap, RSS, and structured data:

```
content/
├── destinations/   # tokyo.md, bali.md ...
├── itineraries/    # tokyo-3-days.md, bali-budget-7-days.md
└── articles/       # packing-guide.md, dubai-layover.md
```

Example frontmatter:

```yaml
---
title: "3 Days in Tokyo: The Perfect First-Timer Itinerary"
description: "A day-by-day Tokyo itinerary covering must-see districts, costs, and transit tips."
destination: Tokyo
country: Japan
duration: 3
budget: mid-range
author: Wayhours Editorial
datePublished: 2026-11-14
dateModified: 2026-11-14
sources:
  - https://www.japan.travel/
---
```

---

## Links

- Website: https://wayhours.com
- Contribute: travel-writing submissions welcome via the site's contributor platform
