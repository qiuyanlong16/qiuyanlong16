# GitHub Profile README Design

**Date:** 2026-04-15
**Author:** qiuyanlong16
**Goal:** Create a visually rich, dark-themed GitHub Profile README for the `qiuyanlong16/qiuyanlong16` repository.

---

## 1. Overview

A single `README.md` file at the root of the `qiuyanlong16/qiuyanlong16` GitHub repository. The profile will be English-language, dark-themed, and heavily visual — inspired by the "Code Mode" aesthetic from the [awesome-github-profile-readme](https://github.com/abhisheknaiidu/awesome-github-profile-readme) repository.

All visual elements use dynamically generated SVGs from public GitHub-hosted endpoints. No external hosting, no build step. The README is a single markdown file with embedded images.

---

## 2. Profile Info (to be filled in README)

| Field | Value |
|-------|-------|
| Name | qiuyanlong16 |
| Role | Frontend & Software Developer |
| Languages | TypeScript, Node.js, Rust, Python, C# |
| Projects | openclaw-manager, hermes-mutil-agent-devops-admin, raspberry_by_smart_speaker |
| Social | Twitter/X: https://x.com/GlobalEye_X, Email: qiuyanlong2016@gmail.com, Blog: https://qiuyanlong16.github.io/hermes-vs-openclaw/ |

---

## 3. Section Architecture

The README is organized top-to-bottom as follows:

### 3.1 Header

- **Welcome Banner**: Greeting text with name and role
- **Animated Typing SVG**: `readme-typing-svg` showing rotating intro text
- **Header GIF**: A coding/developer themed animated banner image

### 3.2 Stats & Activity Dashboard

- **GitHub Stats Card**: Total repos, commits, PRs, stars
- **Top Languages Card**: Bar chart of language usage
- **Coding Activity Pie Chart**: WakaTime-style time breakdown
- **Contribution Activity Graph**: Line chart of commit frequency

### 3.3 Tech Stack & Skills

- **Animated Tech Icon Grid**: Glowing icons for TS, Node.js, Rust, Python, C#
- **Skill Badges**: Categorized badges for Frontend, Backend, Tools

### 3.4 Project Showcase

- Three project cards with title, description, language badge, and links
- One project gets "featured" treatment with a larger banner

### 3.5 Visual Extras

- Themed SVG dividers (rocket/space themed) between sections
- Achievement/trophy badges
- Activity heatmap
- Animated tech stack banner

### 3.6 Footer

- Social links (Twitter/X, Email, Blog) as styled badges
- Visitor count badge
- Closing "Let's connect!" message

---

## 4. Widget & Asset Sources

| Widget | Purpose | Endpoint/Source |
|--------|---------|-----------------|
| `github-readme-stats` | Stats card, top langs, streak | `https://github-readme-stats.vercel.app/api?username=qiuyanlong16` |
| `github-profile-summary-cards` | Contribution overview | `https://github-profile-summary-cards.vercel.app/api/cards` |
| `readme-typing-svg` | Animated header text | `https://readme-typing-svg.demolab.com/` |
| Tech icons | Skill/tech stack icons | Inline SVGs or shields.io badges |
| Visitor badge | Profile view counter | `https://komarev.com/ghpvc/?username=qiuyanlong16` |
| Themed GIFs | Dividers, header | Giphy repos / public image URLs |

---

## 5. Implementation Notes

- Single file: `README.md` at repo root
- No build process — everything is embedded images
- All widget URLs reference `qiuyanlong16` as the GitHub username
- Dark theme is enforced via `?theme=dark` query params on widgets
- Project descriptions are placeholders until user fills them in
- Social links are hardcoded from collected info above
