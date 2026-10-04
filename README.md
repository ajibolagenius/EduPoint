# EduPoint × Trinity University — Full Stack & Mobile Application Development

The programme repository for **Full Stack & Mobile Application Development**, delivered by
[EduPoint](https://www.linkedin.com/company/edupoint-limited/) at **Trinity University, Yaba, Lagos**
under the **EduPoint Future Skills Academy** partnership.

Shared with students and tutors: it holds the curriculum and the per-semester class notes,
pre-reads, lab specs and rubrics as they are written.

## How Students Join

Students select **EduPoint Future Skills Academy** as their skill-acquisition option when they
register courses on the Trinity University student portal. The programme is credit-bearing and runs
alongside the academic degree.

1. Log in to the Trinity University student portal.
2. Open **Course Registration**.
3. Scroll to the **Skill Acquisition / Vocational Course** section and choose EduPoint.

## At a Glance

| Item | Detail |
|---|---|
| **Institution** | Trinity University, Yaba, Lagos |
| **Programme** | Full Stack & Mobile Application Development — unified track |
| **Structure** | 4 levels (100L–400L) × 2 semesters, 12 weeks each |
| **Session format** | One session per week, ~3–3.5 hours: warm-up, live-coded concept, lab, show & tell, ship |
| **Track fork** | End of 200L S1 — Track A Full Stack (PHP + MySQL) or Track B Mobile (React Native + Expo) |
| **Status** | Credit-bearing, registered via the Trinity student portal |
| **First classes** | Week of 2026-10-08 |
| **Lead tutor** | Ajibola Akelebe — Professional Trainer, Software Development |

One shared spine for the first eighteen months, then two specialisations, each ending in a defended
capstone. Joining above 100L is possible through a self-paced bridging pack and a diagnostic.

## The Four Years

| Level | Semester | Focus | Status | Weeks |
|---|---|---|---|---|
| 100L | 1 | Web Foundations & Developer Mindset | Shared | 12 |
| 100L | 2 | Programming with JavaScript | Shared | 12 |
| 200L | 1 | React Foundations | Shared — fork at week 12 | 12 |
| 200L | 2 | Track Introduction | Full Stack or Mobile | 12 |
| 300L | 1 | Track Deepening | Full Stack or Mobile | 12 |
| 300L | 2 | Specialisation & Real-World Practice | Full Stack or Mobile | 12 |
| 400L | 1 | Production & Delivery Engineering | Shared teaching, track-adapted labs | 12 |
| 400L | 2 | AI Engineering, Capstone & Employability | Track capstone | 12 |

Eight semesters, four years, one shared first eighteen months.

**Outcome.** A graduate can independently design, build, test and deploy a production-grade web or
mobile application on a PHP or Python/FastAPI backend, has shipped an AI-backed feature, and can
evidence all of it with a public portfolio of real deployed work — not a certificate alone.

## What You Work On

Every session ends with working code committed to Git. The running projects build across semesters:

- **100L** — a personal portfolio site, then a JavaScript app consuming a real API
- **200L** — a multi-screen React application; Track A adds a PHP/MySQL backend, Track B a working
  app on your own phone via Expo
- **300L** — a documented, secured REST API (Track A) or a native-featured, performant mobile app
  (Track B), each in real-world practice projects
- **400L** — Docker, CI/CD and cloud delivery, then a defended capstone shipping one AI-backed
  feature of your own

## What You Need

| Requirement | Detail |
|---|---|
| **Laptop** | Minimum 4 GB RAM / 20 GB free; 8 GB and 50 GB recommended. Windows 10, macOS 11 or current Linux |
| **Phone** | Any Android or iOS device from 200L — mobile labs run through Expo Go, no emulator needed |
| **Software** | VS Code, Git, Chrome, Node.js LTS — all free. Installers are provided offline in week 1 |
| **Accounts** | GitHub (created in week 2); Expo from 200L; deployment on free tiers |
| **Copilot / AI assistants** | Staged by design: not used at 100L, introduced and critiqued at 200L, expected as professional practice from 300L |

## How You Are Assessed

Consistent every semester, so progress is comparable across both tracks:

| Component | Weight | Basis |
|---|---|---|
| Weekly submissions | 10% | Merged pull requests each week |
| Mid-semester practical | 15% | Timed, individual build against a spec |
| Project milestones | 15% | Scheduled deliverables against a published rubric |
| Final practical examination | 35% | Timed, individual build |
| Project demonstration & defence | 25% | Live demo plus individual questioning |

Git history is the evidence trail throughout: a project without a credible commit history across the
semester does not pass, regardless of its final state.

## Where Coursework Lives

Your code, submissions and weekly starting points live in the **class GitHub organisation**, not in
this repository. A **checkpoint repository is tagged at the start of every week** (`week-05-start`,
…) — if you miss a session or break your code, pull the tag and rejoin immediately. This repository
is the curriculum and the teaching materials.

## Repository Layout

```
curriculum/     Per-semester class notes, pre-reads, lab specs & rubrics (100L-S1 … 400L-S2, per track)
README.md       This document
```

- Semester folder structure and conventions: `curriculum/README.md`.
- Full curriculum document, orientation deck and document tooling are maintained locally by the
  tutor team and distributed to students through the class repository — they are not part of this
  repository.

## For Tutors

Content is authored per semester under `curriculum/<LEVEL>-S<n>/<TRACK>/`, one subfolder per week
once materials grow. Class notes, pre-reads, lab specs and rubrics belong to the semester folder
they are taught in; the weekly checkpoint tags are made in the class repository, not here.
