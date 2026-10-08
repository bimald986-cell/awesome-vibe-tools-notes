# Awesome Vibe Tools Notes

Personal reference for tools spotted in TikToks (Oct 2026). How & when to use them.

## 1. OpenCut — Free Open-Source CapCut Alternative

**Repo (forked):** https://github.com/bimald986-cell/OpenCut  
**Original:** https://github.com/OpenCut-app/OpenCut (~93k stars)  
**Live:** https://opencut.app (classic version)  
**License:** MIT

### What it is
Browser-based (and upcoming desktop/mobile) video editor. Fully free, no subscriptions, no paywalled features, no watermarks, privacy-first (videos stay on device).

### Current status
Being rewritten from the ground up (Rust core + one codebase for web/desktop/mobile). Classic version is usable today. Rewrite brings:
- Editor API
- Plugin-first architecture
- **MCP server** so AI agents can edit videos for you
- Headless mode for batch rendering / automation
- Scripting tab inside the editor

### When to use
- You hate CapCut subscriptions / price hikes
- Quick social-media style edits in the browser
- Future: tell an AI agent "make a 30s TikTok from these clips" and let it run unattended
- Batch process dozens of variants without opening the UI

### How to start
1. Go to https://opencut.app and try the beta
2. Watch the GitHub for the rewrite (new.opencut.app)
3. Star / fork the repo to track MCP + headless features

---

## 2. Haikei — Free SVG Background / Shape Generator

**Site:** https://haikei.app  
**No signup, completely free for basic use**

### What it is
Web tool that generates unique SVG design assets in seconds: blobs, waves, gradients, circle scatter, low-poly grids, layered peaks, etc. Export as SVG or PNG.

### When to use
- Need a nice background for a landing page, presentation, social post, or UI mockup
- Want organic / modern abstract shapes without opening Illustrator or Figma from scratch
- Rapid prototyping of visual styles

### How to use
1. Open haikei.app → Start designing
2. Pick a generator
3. Tweak colors, complexity, canvas size
4. Hit the dice to randomize
5. Download SVG (best for code) or PNG

Pro plan is "coming soon" but the free tier is already very usable.

---

## 3. Manus.im — AI Full-Stack Website / App Builder

**Site:** https://manus.im  
**Credits-based (comment "Manus" on the TikTok for free credits from creators)**

### What it is
Conversational AI that builds **real** full-stack apps (frontend + backend + database + auth + SEO + analytics) from plain English. Not just static pages — actual working SaaS-style apps.

### When to use
- You want a working prototype or production-ready site/app without writing code
- Need backend logic, user accounts, payments (Stripe), etc.
- Want built-in analytics and SEO out of the box
- "Vibe coding" entire products

### How to use
1. Go to manus.im
2. Describe what you want in natural language
3. Iterate via chat
4. Deploy with one command

Great complement to the UI component libraries below.

---

## 4. Cult UI — Fun / Personality-Rich Components

**Site:** https://cult-ui.com  
**Repo (forked):** https://github.com/bimald986-cell/cult-ui  
**Original:** https://github.com/nolly-studio/cult-ui  
**License:** MIT (shadcn registry style)

### What it is
150+ animated, niche React components built for shadcn/ui + Tailwind + Motion. Focus on *interactions* (expanding panels, 3D carousels, popover forms, floating panels) rather than just pretty surfaces.

### When to use
- Your landing page or app needs personality and delightful micro-interactions
- You already use (or plan to use) shadcn/ui
- You want copy-paste components you fully own

### How to use
```bash
npx shadcn@latest add @cult-ui/shift-card
# or register the registry once in components.json
```

---

## 5. Magic UI — Animated Components for "Funded" Looking Landing Pages

**Site:** https://magicui.design  
**Repo (forked):** https://github.com/bimald986-cell/magicui  
**Original:** https://github.com/magicuidesign/magicui (~22.5k stars)  
**License:** MIT

### What it is
150+ free open-source animated React components (marquees, beams, meteors, glowing borders, device mocks, text effects, etc.). Perfect companion for shadcn/ui. Makes a landing page look like a funded startup.

### When to use
- Building marketing / landing pages that need polish and motion
- Want glowing borders, beams, marquees, typing effects, etc. ready to copy-paste
- Pair with Cult UI for more interactive pieces

### How to use
Same shadcn-style install:
```bash
npx shadcn@latest add @magicui/...
```
There is also an MCP server so AI editors can search & install components for you.

---

## 6. Sol-Advisor — Codex Orchestration Plugin

**Repo (forked):** https://github.com/bimald986-cell/sol-advisor  
**Original:** https://github.com/DannyMac180/sol-advisor (~2.6k stars)  
**License:** MIT

### What it is
Codex-native (OpenAI Codex CLI / ChatGPT desktop) plugin for capability-routed software delivery.  
Primary model (Sol / High) plans, routes, verifies and accepts.  
Can delegate implementation to Luna / Max or Terra lanes.  
Keeps architecture & acceptance in the strong model so your best model isn’t wasted on every small piece.

### When to use
- You work heavily with Codex / GPT-5.x family
- You want structured agent workflows (orchestrator + implementers + reviewer)
- Building non-trivial features and want the strongest model to stay in charge of planning & QA

### How to install (from original README)
```bash
codex plugin marketplace add DannyMac180/sol-advisor --ref main
codex plugin add sol-advisor@sol-advisor
# then run the companion agent installer if using native lane
```

Prompt pattern:
> Use $sol-advisor:orchestration to build this feature and verify it. Declare the selective route before task tools.

---

## Quick Decision Guide

| Need | Tool |
|------|------|
| Free CapCut replacement + future AI video agents | **OpenCut** |
| Pretty SVG backgrounds / blobs / waves | **Haikei** |
| Full-stack app from a prompt | **Manus.im** |
| Personality-rich interactive UI components | **Cult UI** |
| Polished animated landing-page components | **Magic UI** |
| Structured multi-agent coding with Codex | **Sol-Advisor** |

---

*Forked the open-source repos into this account so we can track them easily. Notes last updated: 2026-10-08.*
