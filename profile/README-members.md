<div align="center">

<img src="https://raw.githubusercontent.com/all-aboard-ohio/aao-lab-homepage/main/src/assets/AAOLAB_White_Logo.svg" alt="AAO Data Lab" height="64" />

# All Aboard Ohio Data Lab — Member Guide

**Welcome to the team. This document is for active org members and contributors.**

[![Live Site](https://img.shields.io/badge/lab.allaboardohio.org-012345?style=for-the-badge&logoColor=white)](https://lab.allaboardohio.org)
[![Slack](https://img.shields.io/badge/Slack-Dev_Workspace-B72717?style=for-the-badge&logo=slack&logoColor=white)](https://join.slack.com/t/all-aboard-ohio/shared_invite/zt-3wgj180pu-eWAJoGn4_6~y9YHR9Lq3qA)

</div>

---

## Quick Links

| Resource | Link |
|---|---|
| Live site | [lab.allaboardohio.org](https://lab.allaboardohio.org) |
| All Aboard Ohio main site | [allaboardohio.org](https://allaboardohio.org) |
| Contributor docs | [aao-lab-docs](https://github.com/all-aboard-ohio/aao-lab-docs) |
| Homepage source | [aao-lab-homepage](https://github.com/all-aboard-ohio/aao-lab-homepage) |
| Web component library | [aao-lab-components](https://github.com/all-aboard-ohio/aao-lab-components) |
| Slack workspace | [Join here](https://join.slack.com/t/all-aboard-ohio/shared_invite/zt-3wgj180pu-eWAJoGn4_6~y9YHR9Lq3qA) |
| Project board | [GitHub Projects](https://github.com/orgs/all-aboard-ohio/projects) |

---

## What We're Working On

### Active Projects

| Repository | Status | Purpose |
|---|---|---|
| [aao-lab-homepage](https://github.com/all-aboard-ohio/aao-lab-homepage) | ✅ Live (PR open) | React + Vite homepage |
| [aao-lab-components](https://github.com/all-aboard-ohio/aao-lab-components) | ✅ Live on CDN | Shared `<aao-site-header>` + `<aao-notification>` web components |
| [aao-lab-docs](https://github.com/all-aboard-ohio/aao-lab-docs) | ✅ Active | Contributor documentation, auto-rendered on homepage |

### Tools In Development

| Tool | Description | Looking For |
|---|---|---|
| Economic Impact Calculator | Model jobs, GDP uplift, and tax revenue from rail investment | Data analysts, React developers |
| Proposed Route Mapper | Ohio rail corridor explorer with ridership catchment areas | GIS/mapping developers, data engineers |
| Rail News Digest | Curated daily digest of Ohio rail news and legislative updates | API developers, researchers |

Want to pick up a tool? Find the tracking issue on the [project board](https://github.com/orgs/all-aboard-ohio/projects) or ask in `#dev-general` on Slack.

---

## How the Organization Works

### Decision Making

- **Tools and features**: Scoped in GitHub Issues with clear acceptance criteria. Maintainers triage and label. Contributors claim and build.
- **Architecture decisions**: Discussed in `#dev-general` on Slack before implementation. Significant decisions are documented in `aao-lab-docs/architecture.md`.
- **Content and policy framing**: Coordinated with AAO leadership via `#announcements` on Slack.

### Roles

| Role | Responsibilities |
|---|---|
| **Contributor** | Pick up issues, submit PRs, review peer PRs |
| **Maintainer** | Triage issues, review/merge PRs, guide contributors, make architecture calls |
| **Program Lead** | Coordinate across disciplines, manage milestones, liaison with AAO leadership |

Maintainer status is earned — if you have 5+ quality contributions and want to step up, say so in `#dev-general`.

---

## Slack Channels

| Channel | Purpose |
|---|---|
| `#general` | Org-wide announcements and introductions |
| `#dev-general` | Developer conversation, architecture, code questions |
| `#dev-resources` | API keys, dataset access, environment help |
| `#projects` | Per-project coordination threads |
| `#education` | Students, professors, and capstone coordination |
| `#announcements` | Updates from AAO leadership and maintainers |
| `#policy` | Legislative tracking, policy analysis, framing discussions |

---

## Technical Standards (Required on Every Project)

Every publicly facing AAO Data Lab tool must include:

```html
<!-- In index.html -->
<script type="module" src="https://all-aboard-ohio.github.io/aao-lab-components/aao-banner.js"></script>
```

```jsx
// In root layout component
<aao-site-header mode="compact" dev-url="https://lab.allaboardohio.org"></aao-site-header>
<aao-notification
  config-url="https://raw.githubusercontent.com/all-aboard-ohio/aao-lab-components/main/banner.json"
></aao-notification>
```

**Privacy:** No personal data collection, no third-party analytics trackers, ever.

**Accessibility:** WCAG 2.1 AA minimum. Run axe DevTools before every PR.

**Full standards:** [requirements.md](https://github.com/all-aboard-ohio/aao-lab-docs/blob/main/requirements.md)

---

## Brand Reference

| Token | Hex | Use |
|---|---|---|
| `aao-dark-blue` | `#012345` | Primary backgrounds, headings |
| `aao-dark-red` | `#B72717` | Accents, CTAs |
| `aao-light-blue` | `#388CBB` | Links, hover states, highlights |
| `aao-beige` | `#FBF3E3` | Alternate section backgrounds |

Fonts: **Poppins** (`font-heading`) for all headings, **Montserrat** (`font-body`) for everything else.

Full guide: [style-guide.md](https://github.com/all-aboard-ohio/aao-lab-docs/blob/main/style-guide.md)

---

## How to Contribute

1. **Find an issue** labeled `good first issue` or ask in `#dev-general` for a recommendation
2. **Comment to claim it** — wait for a maintainer to assign it before starting
3. **Branch off `main`** using the naming convention: `feature/`, `fix/`, `docs/`, `data/`, `chore/`
4. **Open a PR** with the template filled in and `Closes #<issue-number>` in the description
5. **Respond to feedback** within 5 business days — maintainers aim for the same turnaround

Commit format: `feat|fix|docs|style|refactor|test|chore|data(<scope>): <description>`

Full guide: [contributing.md](https://github.com/all-aboard-ohio/aao-lab-docs/blob/main/contributing.md)

---

## Our Disciplines

Great work here requires every one of these:

| Discipline | What You Build |
|---|---|
| **Software Developers** | Web apps, APIs, maps, data pipelines — React, Python, Node |
| **Data Analysts / Engineers** | Cleaned datasets, Jupyter notebooks, economic models, ETL |
| **UI/UX Designers** | Component specs, Figma designs, accessibility audits |
| **Policy Analysts** | Legislative context, source review, policy framing guides |
| **Researchers** | Literature reviews, comparable programs, citations |
| **Project Managers** | Issue scoping, milestones, cross-discipline coordination |
| **Technical Writers** | Docs, READMEs, onboarding guides |

---

## Our Mission

We build tools that make the case for investing in passenger rail and connected public transit — with rigorous economic analysis and visualizations that anyone can understand and share. Rail is the spine, but the system includes local transit, bike infrastructure, and station-area development. We design for reuse beyond Ohio — any advocate in any corridor should be able to use what we build.

Full context: [mission-ethos.md](https://github.com/all-aboard-ohio/aao-lab-docs/blob/main/mission-ethos.md)

---

<div align="center">

Questions? Ask in `#dev-general` on Slack · [lab.allaboardohio.org](https://lab.allaboardohio.org) · [allaboardohio.org](https://allaboardohio.org)

</div>
