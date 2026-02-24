# Meta Ads Performance Marketing Academy

A complete, production-ready educational website covering Meta (Facebook & Instagram) Ads from beginner to advanced.

## Features

- 18 full content sections covering all aspects of Meta Ads
- Sidebar navigation with section grouping
- Internal search bar (searches across all topics)
- AI Chatbot assistant with 15+ topic knowledge base
- Expandable troubleshooting diagnostics
- Fully responsive (mobile, tablet, desktop)
- Dark theme, modern design
- Zero dependencies — single HTML file, works anywhere

## Pages / Sections

| Section | Content |
|---|---|
| Home | Overview and learning paths |
| Start Here | Orientation, tools, account setup checklist |
| Meta Ads Basics | Campaign structure, objectives, auction, learning phase, ABO/CBO, placements |
| Campaign Creation | Step-by-step campaign setup, UTMs, naming convention |
| Audience Targeting | Interest, broad, custom, lookalike audiences, frequency |
| Creatives & Ad Copy | Hooks, AIDA/PAS, video structure, UGC, creative testing |
| Optimization & Metrics | CPM, CTR, CPA, ROAS, CVR — full diagnosis for each |
| Scaling Strategies | Vertical/horizontal scaling, CBO structure, creative calendar |
| Retargeting Strategies | Funnel levels, retargeting windows, DPA setup |
| Tracking & Analytics | Meta Pixel, standard events, iOS 14 impact |
| GTM Full Guide | Tags, triggers, variables, click tracking, data layer, forms |
| GA4 Full Guide | Setup, enhanced measurement, funnels, debug view |
| Conversion API | CAPI setup, deduplication, GTM server-side |
| Advanced Meta Ads | ASC, DCO, advanced bidding, attribution windows, first-party data |
| Troubleshooting Center | 7 diagnostic scenarios with step-by-step solutions |
| Real World Scenarios | E-commerce, local business, SaaS, scaling case studies |
| Resources | Official links, tools, formulas reference |
| About | How to use the academy |

## Running Locally

Just open `index.html` in your browser — no server required:

```bash
# Option 1: Direct file open
open index.html

# Option 2: Simple Python server
python3 -m http.server 3000
# Then visit http://localhost:3000
```

## Deploying to Vercel

1. Push this folder to a GitHub repository
2. Go to vercel.com → New Project → Import your GitHub repo
3. No configuration needed — Vercel detects it as a static site
4. Click Deploy

## Deploying to Netlify

1. Push to GitHub, or drag the folder to netlify.com/drop
2. For GitHub: New Site → Import from Git → Select repo
3. Build command: leave empty
4. Publish directory: `.` (root)
5. Click Deploy

## File Structure

```
meta-ads-academy/
├── index.html    ← Entire website (HTML + CSS + JS)
└── README.md     ← This file
```

The entire site is a single `index.html` file. All CSS and JavaScript are embedded inline — no external dependencies except Google Fonts (loaded via CDN). The site works offline if Google Fonts CDN is unavailable (falls back to system fonts).

## Customization

- **Colors:** Edit CSS variables at the top of the `<style>` block (`:root { }`)
- **Content:** Each page is a `<div class="page" id="page-[name]">` — edit directly in HTML
- **Chatbot knowledge:** Add to the `knowledgeBase` array in the `<script>` block
- **Search index:** Add entries to the `searchIndex` array
- **Navigation:** Edit the `<nav id="sidebar">` section
