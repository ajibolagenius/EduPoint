# Curriculum — Class Notes & Teaching Materials

Per-semester working directories for the Full Stack & Mobile unified track.
The full curriculum document is distributed by the tutor team (via the class repository); these
folders hold the materials written for each semester.

## Structure

| Folder | Semester | Covers | Curriculum section |
|---|---|---|---|
| `100L-S1/` | 100 Level S1 | Web Foundations & Developer Mindset (shared) | §4 |
| `100L-S2/` | 100 Level S2 | Programming with JavaScript (shared) | §5 |
| `200L-S1/` | 200 Level S1 | React Foundations — the shared bridge (fork at week 12) | §6, §7 |
| `200L-S2/Full-Stack/` | 200 Level S2 | Track A intro: Core PHP, MySQL | §8.1 |
| `200L-S2/Mobile/` | 200 Level S2 | Track B intro: React Native + Expo | §9.1 |
| `300L-S1/Full-Stack/` | 300 Level S1 | Track A deepening: REST API, auth, full-stack integration | §8.2 |
| `300L-S1/Mobile/` | 300 Level S1 | Track B deepening: auth, native features, performance | §9.2 |
| `300L-S2/Full-Stack/` | 300 Level S2 | Track A real-world practice; School Management System v1 | §8.3 |
| `300L-S2/Mobile/` | 300 Level S2 | Track B real-world practice; student-chosen app v1 | §9.3 |
| `400L-S1/` | 400 Level S1 | Production & Delivery Engineering — Python primer, Docker, CI/CD, cloud (shared teaching, track-adapted labs) | §10.1 |
| `400L-S2/Full-Stack/` | 400 Level S2 | AI engineering + capstone (School Management System, AI-backed, defended) | §10.2 |
| `400L-S2/Mobile/` | 400 Level S2 | AI engineering + capstone (student-chosen app, AI-backed, shipped build) | §10.2 |

## Conventions

- Every class session is **2 hours (120 minutes)**. The standard split is 10 minutes warm-up,
  25 guided practice, 65 lab, 10 show & tell and 10 save/submit. Pre-reading is separate.
  Confirmed 2026-10-26; supersedes the original curriculum's longer session model. Earlier weekly
  plans retain their original timings and must be shortened before reuse.
- One subfolder per week (`week-01/`, `week-02/`, …). Each week holds `pre-read.md`,
  `class-notes.md`, `class-notes.html` and `lab.md` as they are written. **Always write an interactive
  HTML presentation when creating or revising class notes.** This begins with 100L S1 Week 04;
  convert earlier weeks when next revised. Keep Markdown and HTML aligned.
- Pre-reads, class notes, lab specs, and rubrics live under the semester folder they belong to.
- The checkpoint repository is tagged weekly (`week-05-start`, …) in the class GitHub repo, not here.
- Physical classes start the week of 2026-10-08; the orientation deck is shared separately.

## Week 04 onward: materials and presentation formats

100L S1 Week 04: [Before class](100L-S1/week-04/pre-read.md) ·
[Class workbook](100L-S1/week-04/class-notes.md) ·
[Interactive class presentation](100L-S1/week-04/class-notes.html) ·
[Practical lab](100L-S1/week-04/lab.md).

100L S1 Week 05: [Before class](100L-S1/week-05/pre-read.md) ·
[Class workbook](100L-S1/week-05/class-notes.md) ·
[Interactive class presentation](100L-S1/week-05/class-notes.html) ·
[Practical lab](100L-S1/week-05/lab.md) ·
[Practice kit](100L-S1/week-05/practice-kit/).
Matching PDFs sit beside each Markdown file.

### HTML class presentations

Download `class-notes.html` and open it in a modern browser; GitHub's file view shows the source.
The Week 04 presentation embeds its images, uses system fonts, and works offline as a single file.
Keep the matching lab/pre-read PDFs beside it to use the optional workbook links offline. Use the
on-screen controls, arrow keys or swipe to navigate, and **Contents** to jump to a topic. Choose your
shell once; command examples follow that choice. **Motion** can be switched off at any time.
The timer stays visible on every slide: click its time to edit minutes and seconds, or choose a
120-minute class, 65-minute lab or 10-minute activity preset. Start, pause and reset are always
available. Its duration and running/paused state persist in this browser's localStorage, including
across reloads; a running timer keeps counting while the file is closed. If browser storage is
blocked, the presentation reports that it cannot save the timer.

To present from the room's laptop and drive the slides from a phone on the same Wi-Fi, run
`node tools/deck-server.mjs curriculum/100L-S1/week-04` from the repository root. It prints a deck
URL for the laptop and a `/remote` URL for the phone. The phone gets Next/Previous buttons, a slide
list and a touch pad that moves a laser dot on the laptop. The deck itself is unchanged: the remote
only works while the server runs, and the file still opens offline as before.

Every future HTML version must be clean, interactive and motion-backed, using the Week 04 lab
theme — monochrome with four purposeful accents, system monospace type rather than embedded font
files, big rounded controls and no full-bleed dark slides. Interactions must teach: predict, try, inspect and explain. Browser
simulations are practice, not proof of device work. Keep the two-hour session, student-only content,
source credits and the Markdown workbook's scope. Include keyboard navigation, a topic index,
reduced-motion support, the phone-remote hook and offline assets. Check every slide and core
interaction in a real browser at projector and phone sizes before delivery. Full authoring
requirements are in [AGENTS.md](AGENTS.md).

From Week 04, use the workbook layout: a session map, short activity pages, clearly labelled
operating-system commands (including both Windows PowerShell and Command Prompt), expected results,
checkpoints and writing space. **Each section is hands-on first: the student acts, sees the real output,
then reads at most three lines naming what happened.** Show pasted tool output rather than describing
it, and keep doing time above reading time. Full rules are in [`AGENTS.md`](AGENTS.md). Class notes and
their PDFs are student-only: put tutor guidance at the
end of the lab, never in class notes. Answers remain collapsible in Markdown and appear as labelled self-check boxes in print.
Use `<!-- layout: workbook -->` at the start of a source and `<!-- pagebreak -->` between planned
pages. The tutor's local renderer is `node tools/md2pdf.mjs curriculum/100L-S1/week-04` from the
repository root. The workbook theme uses local fonts and needs no internet to render these notes.
