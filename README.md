# EduPoint × Trinity University — Full Stack & Mobile Software Development

Programme repository for the **EduPoint Professional Skills Development Programme** delivered at
**Trinity University, Yaba, Lagos** (Faculty of Science and Technology), under the **EduPoint Future
Skills Academy** partnership. Students register it on the Trinity portal as their skill-acquisition
option; it is credit-bearing and runs alongside their academic degree.

## The Partnership

EduPoint partners with Trinity University to give students practical, industry-relevant skills that
complement their academic education — hands-on building, certifications, and a public portfolio of
deployed work rather than a certificate alone.

This repository holds the **Full Stack Software Development** track (S/N 3), taught as a unified
track that forks into **Full-Stack (Track A)** and **Mobile (Track B)** from 200 Level.

## At a Glance

| Item | Detail |
|---|---|
| **Institution** | Trinity University, Yaba, Lagos — Faculty of Science and Technology |
| **Programme** | Full Stack Software Development (unified; Full-Stack and Mobile tracks) |
| **Structure** | 4 levels (100L–400L) × 2 semesters = 8 modules, 12 weeks each |
| **Contact** | 2 sessions/week × 2–3 hours (~60 hours/semester) |
| **Cohort** | 30–100 students, progressing together; on-ramp for joiners above 100L |
| **Status** | Credit-bearing, registered via the Trinity student portal |
| **Delivery starts** | Physical classes from the week of 2026-10-08 |
| **Trainer** | Ajibola Akelebe — Professional Trainer, Full Stack Software Development |

**Programme outcome.** A graduate of the four-year track can independently design, build, test, and
deploy a production-grade application in two backend languages, has shipped a mobile app and an
AI-backed feature, and can evidence all of it with a public portfolio built over eight semesters.

## Repository Layout

```
curriculum/     Per-semester lecture notes & teaching materials (100L-S1 … 400L-S2, per track)
docs/           Canonical curriculum, tools & requirements memo, faculty matrix
presentation/   Virtual presentation deck (deployed to fullstack-edu.surge.sh)
tools/          md2pdf — renders Markdown docs to PDF
```

- Source of truth for the curriculum: `docs/Unified_Full_Stack_and_Mobile_Curriculum.pdf`
  (`docs/CURRICULUM_[LEGACY].md` is the superseded single-track version).
- Structure and conventions of the semester folders: `curriculum/README.md`.
- Facility, tooling, and licence decisions requested of EduPoint: `docs/TOOLS-AND-REQUIREMENTS.md`.

## Docs → PDF

```bash
cd tools
npm install
npm run pdf          # node md2pdf.mjs
```

Uses `puppeteer-core` with a locally installed Chrome; no browser is downloaded.

## Notes

- Assessment and checkpoint repositories live in the class GitHub organisation, not here; the
  checkpoint repo is tagged weekly (`week-05-start`, …).
- All software in year one is free (VS Code, Git, Node.js, GitHub); distribution and connectivity
  requirements are set out in the tools memo.
