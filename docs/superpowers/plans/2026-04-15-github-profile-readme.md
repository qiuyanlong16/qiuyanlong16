# GitHub Profile README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a visually rich, dark-themed GitHub Profile README with animated widgets, stats dashboards, project showcase, and social links for `qiuyanlong16/qiuyanlong16`.

**Architecture:** Single `README.md` file at repo root, composed of embedded SVG images from public widget endpoints. No build process, no external hosting — all images are served dynamically from GitHub-hosted SVG endpoints.

**Tech Stack:** Markdown, SVG images (github-readme-stats, readme-typing-svg, github-profile-summary-cards, shields.io badges, Komarev visitor counter).

---

## File Structure

| File | Action | Responsibility |
|------|--------|----------------|
| `README.md` | Create | The entire profile — all 6 sections as one file |
| `.github/ISSUE_TEMPLATE/` | (optional) | Future-proofing, skip unless requested |

---

### Task 1: Header Section

**Files:**
- Create: `README.md` (new file, write lines 1–20)

This task creates the README from scratch with the header section:
- Welcome heading with name and role
- Animated typing SVG with rotating intro text lines
- Developer-themed header GIF banner
- Profile info badge row

```markdown
## README.md — Header Section

Add this content at the top of the file:

```markdown
### Hi there 👋

<!-- Typing SVG by DenverCoder1 - https://git.io/typing-svg -->
<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com/?lines=Frontend+%26+Software+Developer;Building+things+for+the+web+and+beyond;TypeScript+%7C+Rust+%7C+Python+%7C+C%23;Open+Source+Enthusiast&font=Fira+Code&center=true&width=500&height=50&duration=3500&pause=1000&color=58A6FF" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <img src="https://media.giphy.com/media/iY8CRBdQXODJSCERIr/giphy.gif" alt="Coding Animation" width="600" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/-Open%20Source-3DA639?style=flat-square&logo=open-source-initiative&logoColor=white" />
  <img src="https://img.shields.io/badge/-Frontend_Developer-61DAFB?style=flat-square&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/-Building_Cool_Stuff-FF6F61?style=flat-square" />
</p>
```
```

- [ ] **Step 1: Create README.md with header section**

Write the header markdown above into `README.md`.

- [ ] **Step 2: Verify the file was created**

Run: `cat README.md`
Expected: Markdown content with heading, typing SVG, GIF, and badges.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add profile header with typing SVG and badges"
```

---

### Task 2: Stats & Activity Dashboard

**Files:**
- Modify: `README.md` (append lines 22–50)

This task adds the stats dashboard section with GitHub stats cards and language charts.

```markdown
## README.md — Stats Section

Append this content after the header section:

```markdown
---

### 📊 Stats & Activity

<div align="center">
  <img width="49%" src="https://github-readme-stats.vercel.app/api?username=qiuyanlong16&show_icons=true&theme=dracula&hide_border=true&include_all_commits=true" alt="GitHub Stats" />
  <img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=qiuyanlong16&layout=donut-vertical&theme=dracula&hide_border=true&langs_count=8" alt="Top Languages" />
</div>

<div align="center">
  <img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=qiuyanlong16&theme=dracula" alt="Profile Details" />
  <img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=qiuyanlong16&theme=dracula" alt="Stats" />
</div>
```
```

- [ ] **Step 1: Append stats section to README.md**

Add the stats markdown block above after the header section (after the `---` divider).

- [ ] **Step 2: Verify the append**

Run: `tail -30 README.md`
Expected: Stats section with 4 widget images (stats card, top langs, profile details, stats summary).

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add stats and activity dashboard widgets"
```

---

### Task 3: Tech Stack Section

**Files:**
- Modify: `README.md` (append lines 52–70)

This task adds the technology showcase with animated skill icons and categorized badges.

```markdown
## README.md — Tech Stack Section

Append this content after the stats section:

```markdown
---

### 🛠️ Tech Stack

<div align="center">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Rust-DEA584?style=for-the-badge&logo=rust&logoColor=black" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white" />
</div>

<div align="center">
  <img src="https://skillicons.dev/icons?i=ts,nodejs,rust,python,cs,react,vue,nextjs,webpack,git,docker,linux&theme=dark" alt="Tech Stack Icons" />
</div>

<div align="center">
  <img src="https://img.shields.io/badge/Frontend-React_/_Vue_/_Next.js-61DAFB?style=flat-square" />
  <img src="https://img.shields.io/badge/Backend-Node.js_/_Rust_/_Python-339933?style=flat-square" />
  <img src="https://img.shields.io/badge/Tools-Docker_/_Git_/_Linux-2496ED?style=flat-square" />
</div>
```
```

- [ ] **Step 1: Append tech stack section to README.md**

Add the tech stack markdown block above after the stats section.

- [ ] **Step 2: Verify the append**

Run: `tail -25 README.md`
Expected: Tech stack section with shield.io badges and skillicons.dev icon grid.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add tech stack icons and skill badges"
```

---

### Task 4: Project Showcase

**Files:**
- Modify: `README.md` (append lines 72–100)

This task adds the project showcase section with repo pins for each project.

```markdown
## README.md — Projects Section

Append this content after the tech stack section:

```markdown
---

### 🚀 Featured Projects

<div align="center">
  <a href="https://github.com/qiuyanlong16/openclaw-manager">
    <img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=qiuyanlong16&repo=openclaw-manager&theme=dracula&show_owner=true&border_radius=10" alt="openclaw-manager" />
  </a>
  <a href="https://github.com/qiuyanlong16/hermes-mutil-agent-devops-admin">
    <img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=qiuyanlong16&repo=hermes-mutil-agent-devops-admin&theme=dracula&show_owner=true&border_radius=10" alt="hermes-mutil-agent-devops-admin" />
  </a>
</div>

<div align="center">
  <a href="https://github.com/qiuyanlong16/raspberry_by_smart_speaker">
    <img width="48%" src="https://github-readme-stats.vercel.app/api/pin/?username=qiuyanlong16&repo=raspberry_by_smart_speaker&theme=dracula&show_owner=true&border_radius=10" alt="raspberry_by_smart_speaker" />
  </a>
</div>
```
```

- [ ] **Step 1: Append projects section to README.md**

Add the project showcase markdown block above after the tech stack section.

- [ ] **Step 2: Verify the append**

Run: `tail -25 README.md`
Expected: Featured projects section with 3 repo pin cards as clickable links.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add featured projects showcase"
```

---

### Task 5: Visual Extras

**Files:**
- Modify: `README.md` (append lines 102–125)

This task adds themed visual dividers, contribution graphs, and activity widgets between sections.

```markdown
## README.md — Visual Extras Section

Append this content after the projects section:

```markdown
---

### 📈 Contribution Activity

<div align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=qiuyanlong16&theme=dracula" alt="Commit Languages" />
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=qiuyanlong16&theme=react-dark&line=58A6FF&point=58A6FF&area=true&hide_border=true" alt="Activity Graph" />
</div>

<p align="center">
  <img src="https://media.giphy.com/media/du3J3cXyzhj75IOgvA/giphy.gif" alt="Rocket Animation" width="400" />
</p>
```
```

- [ ] **Step 1: Append visual extras section to README.md**

Add the visual extras markdown block above after the projects section.

- [ ] **Step 2: Verify the append**

Run: `tail -25 README.md`
Expected: Contribution activity section with language chart, activity graph, and rocket animation GIF.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add contribution activity graphs and visual extras"
```

---

### Task 6: Footer & Social Links

**Files:**
- Modify: `README.md` (append lines 127–end)

This task adds the footer with social links, visitor counter, and closing message.

```markdown
## README.md — Footer Section

Append this content at the end of the file:

```markdown
---

### 🌐 Connect With Me

<div align="center">
  <a href="https://x.com/GlobalEye_X">
    <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter" />
  </a>
  <a href="mailto:qiuyanlong2016@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://qiuyanlong16.github.io/hermes-vs-openclaw/">
    <img src="https://img.shields.io/badge/Blog-000000?style=for-the-badge&logo=github&logoColor=white" alt="Blog" />
  </a>
</div>

---

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=qiuyanlong16&label=Profile+Views&color=58A6FF&style=flat-square" alt="Profile Views" />
</div>

<p align="center">
  <strong>Thanks for stopping by! Happy coding! 🚀</strong>
</p>
```
```

- [ ] **Step 1: Append footer section to README.md**

Add the footer markdown block above at the end of the file.

- [ ] **Step 2: Verify the complete file**

Run: `cat README.md`
Expected: Full profile README with all 6 sections (header, stats, tech stack, projects, visual extras, footer).

- [ ] **Step 3: Count total lines**

Run: `wc -l README.md`
Expected: 130–160 lines.

- [ ] **Step 4: Commit**

```bash
git add README.md
git commit -m "feat: add footer with social links and visitor counter"
```

---

### Task 7: Final Review & Push

**Files:**
- Modify: `README.md` (no changes, final review)

- [ ] **Step 1: Review the complete README**

Run: `cat README.md`
Check: All sections render correctly in markdown. All image URLs use `qiuyanlong16` as the username. All links are valid.

- [ ] **Step 2: Verify git status is clean**

Run: `git status`
Expected: clean working tree, all commits on main branch.

- [ ] **Step 3: View commit history**

Run: `git log --oneline`
Expected: 6 feature commits, one per task.

- [ ] **Step 4: Push to remote (when user is ready)**

```bash
git push -u origin main
```
