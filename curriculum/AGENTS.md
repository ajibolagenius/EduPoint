# AGENTS.md

Guidance for AI coding agents working in this repository (Claude Code, Copilot, Cursor, Codex and
similar). Human contributors should follow the same rules.

## What this repository is

This repository holds the curriculum and teaching materials for the **Full Stack & Mobile Application
Development** programme, a four-year, unified-track course:

- **100L to 200L S1:** a shared foundation, ending with React.
- **From 200L S2:** students fork into **Track A, Full Stack** (PHP + MySQL) or **Track B, Mobile**
  (React Native + Expo).

This repository is **public** and is read by tutors and students alike. It holds teaching materials only.
Student code, submissions and the weekly checkpoint tags live in the class GitHub organisation, not here.

See the root [`README.md`](../README.md) for the programme overview and [`curriculum/README.md`](README.md)
for the semester folder map.

## Who you are working for

Find out which of these applies before you act:

- **A tutor writing materials.** Follow [Writing teaching materials](#writing-teaching-materials).
- **A student studying.** Follow [Working with students](#working-with-students). The programme's AI
  policy limits what you may do.

If you can't tell, ask.

---

## Repository layout

```
curriculum/
  README.md                 semester map and conventions
  100L-S1/ … 200L-S1/       shared semesters
  200L-S2/ … 300L-S2/       split into Full-Stack/ and Mobile/
  400L-S1/                  shared teaching, track-adapted labs
  400L-S2/                  split into Full-Stack/ and Mobile/
    story.md                the semester's running example (100L S1: Mama Titi's Kitchen)
    week-07/
      pre-read.md           student-facing: the week's foundations, read before the session
      class-notes.md        student-facing: the full module-by-module notes, for class and revision
      class-notes.html      required presentation the tutor teaches from, built from the notes
      assets/               images the notes need, only when a real screenshot teaches something
    assignments/
      assignment-NN.md      student-facing: the week's graded take-home, carrying its deliverable
```

- Create one folder per week, named `week-NN` with two digits.
- From 100L S1 Week 07, a week has **four materials and nothing else**: `pre-read.md`,
  `class-notes.md`, `class-notes.html` and one `assignments/assignment-NN.md`. Don't write a
  `lab.md`, a practice kit, tutor notes or story episodes for new weeks.
- **Always render PDFs** of `pre-read.md`, `class-notes.md` and the assignment, and keep them beside
  their Markdown: `node tools/md2pdf.mjs <file.md>` from the repository root. Re-render after every
  Markdown edit. All three use the assignment PDF theme (green title band, tinted metadata strip),
  so each must start with its `#` title followed by a bold metadata line. Students download them for offline reading; the assignment PDF goes on Google Classroom.
- Weeks 01–06 keep files from earlier formats (labs, practice kits, PDFs, tutor notes). Leave them
  as they are, and don't copy their layouts forward.
- Empty folders contain a `.gitkeep` file. Delete it when the folder gets real content.

## The source of truth

The **curriculum document** defines every semester: its weekly themes, content, labs and deliverables,
the structure of a session, and the assessment model. The tutor team maintains it and shares it
privately; **it is not committed to this repository.**

- Before writing a week, read that week's row in the curriculum document. If you don't have the
  document, ask the tutor for the week's theme, content and deliverable.
- **Never invent** a week's topic, deliverable, deadline or grading weight.
- Never commit the curriculum document, or any file or folder listed in `.gitignore`.

---

## Writing teaching materials

### Write original material

- Base each week on the curriculum document and the reference sites below.
- Write fresh explanations, analogies and activities. **Do not reuse or adapt old drafts or legacy
  material** unless the tutor asks you to.
- Link to external sources rather than copying them. Paraphrase, and quote only short pieces with
  credit.
- Credit sources at the end of each file under a **Sources** or **References** heading.
- Put a Mermaid diagram beside every concept with structure or flow; keep its source editable in
  Markdown. Add a raster image (such as a real interface screenshot) only when it teaches something
  words and diagrams can't. Give it meaningful alt text, a caption, source and licence, and store it
  in the week's `assets/` folder for offline use.

### Reference sites

| Site | Use it for |
|---|---|
| [MDN, Learn web development](https://developer.mozilla.org/en-US/docs/Learn_web_development) | The authoritative reference for HTML, CSS, JavaScript, HTTP and how the web works |
| [The Valley of Code](https://thevalleyofcode.com/) | Short, one-concept lessons. Many now redirect to flaviocopes.com; link to the final URL. |
| [Flavio Copes, free courses](https://flaviocopes.com/courses/) | Structured courses: HTTP, DNS, HTML, CSS, Git, Node.js, SQL and more |
| [JavaScript.info](https://javascript.info/) | JavaScript in depth, from 100L S2 |

### Check before you commit

- **Open every link** you add and confirm it loads, for example with
  `curl -sL -o /dev/null -w "%{http_code}"`. Use the URL the page ends up at after any redirects.
  Course sites move pages often, and a redirect to a generic tag page counts as a broken link.
- **Check every fact** against a source: dates, port numbers, status codes, commands, shortcuts.
- **Run every command** you put in front of students, or confirm what it outputs.

### Fit how the programme runs

- **Session structure.** Every class is **2 hours (120 minutes)**, as confirmed by the lead tutor
  on 2026-10-26. This supersedes the longer timings in curriculum §2 and earlier weekly plans:

  | Part | Time | From Week 07, taught from |
  |---|---|---|
  | Warm-up | 10 min | A recap or prediction from the deck |
  | Guided modules | 25 min | The modules, live-coded, with a room vote per module |
  | Hands-on exercises | 65 min | The notes' Levels 1–3 |
  | Show & tell | 10 min | Learners show Level 3 work |
  | Ship | 10 min | Save work and start the assignment |

  Session plans must total exactly 120 minutes, including transitions, saving and submission.
  Pre-reading, the assignment and optional extensions are outside class time. Interleave short
  demonstrations with student attempts, expected results and checks; hands-on work takes most of the
  session. Before Git is taught, Ship means saving files and submitting evidence. Shorten older plans
  before reusing them.
- **Teach only what students know so far.** Don't use a tool, language or concept before the week
  that introduces it. For example, in 100L S1 the terminal arrives in week 4, VS Code in week 5, HTML in
  week 6 and Git in week 11. When a reading mentions a tool students haven't met yet, tell them to skip
  that part.
- **Plan for poor connectivity.** Students may have no laptop or no data. Give a no-internet fallback
  for anything that depends on the network, and prefer activities that work offline.
- **Submissions.** Assignments are posted and collected on **Google Classroom**. Once Git has been
  taught, weekly submissions are merged pull requests, linked from Classroom. Before that, the
  assignment must say exactly what to submit and how to name the files.
- **Grading weights** are fixed by the curriculum document:

  | Component | Weight |
  |---|---|
  | Weekly submissions | 10% |
  | Mid-semester practical | 15% |
  | Milestones | 15% |
  | Final practical | 35% |
  | Demo & defence | 25% |

  Never change these in an assignment's rubric.

### What each file contains

From 100L S1 Week 07 (decided by the lead tutor on 2026-11-14), every week uses the **module
structure** below, modelled on the tutor team's full-stack class notes. The notes teach the concept
fully; the deck teaches it live; the assignment is where students prove it.

| File | Read by | What it is |
|---|---|---|
| `pre-read.md` | students, before class | The week's foundations in the same structure, 30–45 minutes |
| `class-notes.md` | students | The full module-by-module notes, for class and revision |
| `class-notes.html` | the room | The presentation the tutor teaches from, built from the notes |
| `assignments/assignment-NN.md` | students | The graded take-home that carries the week's curriculum deliverable |

**`class-notes.md`** — this outline, in this order:

1. `# Week NN: <Curriculum theme>`, then a bold line with the level, semester, week and "Class
   notes" (the PDF shows it as a strip under the title), then two or three short paragraphs: what
   students can already do, what is still missing, and what this week adds. A `---` rule follows.
2. `## Pedagogical Roadmap`: one Mermaid `flowchart TD`, a node per module, each listing its three or
   four subtopics as `•` bullets.
3. `## Module N: <Title>`, usually five or six, covering the curriculum row's content in teaching
   order. Inside each module:
   - Numbered subsections, `### 1. <Subtopic>`. Name the analogy in the heading where there is one,
     such as "(The Paper Form Analogy)". Explain the idea before naming it.
   - The **mental model** in a `> [!NOTE]` callout that starts `**The Mental Model:**`.
   - Tables to compare things, Mermaid for structure and flow, and short commented code blocks.
     Mark wrong and right code with 🔴 and 🟢 comments.
   - GitHub callouts, each with one job: `[!NOTE]` mental models, `[!TIP]` shortcuts and good habits,
     `[!IMPORTANT]` rules students must not miss, `[!WARNING]` mistakes that break work,
     `[!CAUTION]` safety, security or data-loss risks.
   - `### 🏋️ Try It Now (Drill N)` wherever students should act before the next module: numbered
     steps and the real output or screen to expect.
4. `## Module N: Rookie Traps & Debugging Guide`: a table of *what you see* · *what happened* ·
   *how to fix it*, quoting real error messages and real browser behaviour.
5. `## 🎯 Week NN Hands-on Classroom Exercises`: `### Level 1`, `### Level 2`, `### Level 3`, from
   guided drill to independent build. Level 3 starts the week's curriculum deliverable; the
   assignment finishes and submits it.
6. `## 📚 Curated Deep-Dive References`: five to eight bullets, `* [Site: Page](url) — why to open it.`
   Then `### Sources`: the curriculum row, anything paraphrased, and the date links were checked.

- **Running example.** Code samples share one running example across the semester (100L S1:
  Mama Titi's Kitchen; see [`100L-S1/story.md`](100L-S1/story.md)). It is example data, not a story:
  no cold opens, beats, cliffhangers or dialogue.
- **Length:** roughly 500–850 lines of Markdown. The notes may explain more than the room hears.
- **Student-only.** Never add a "For tutors" section, a run sheet or the answer to graded work.
- Answers to drills may sit in `<details><summary>Answer</summary>…</details>` blocks.

**`pre-read.md`** — the same structure, shorter (30–45 minutes):

1. `# Week NN Pre-read: <Theme>`: the session in two or three sentences, the time needed and what to
   bring. A `---` rule follows.
2. `## Pedagogical Roadmap`: the class notes' roadmap, with the modules the pre-read covers marked.
3. Two or three `## Module N:` sections covering only the foundations. Each has a `[!NOTE]` mental
   model, one small example and a `### Read with a question` reading: the link, where to stop, and
   one question to keep in mind.
4. `## 🏋️ Warm-up Drill`: one short task before class, on paper or a laptop.
5. `## No Internet?`: an offline summary of each reading.
6. `## ✅ Ready Check` and `## 📚 References`.

**`assignments/assignment-NN.md`** — one per week from 100L S1 Week 06, numbered in the order set:

1. `# Assignment NN: <Title>`, a line with the level, week, theme, points and suggested time, then
   two or three paragraphs on what students build and why. A `---` rule follows.
2. `## Mission Roadmap`: a Mermaid flowchart of the tasks.
3. `## Before You Start`: the AI policy and individual-work rule in a `> [!IMPORTANT]` callout, then
   the folder and file names.
4. `## Task N: <Title> · P points`: requirements as a table or numbered steps, the evidence to keep,
   and callouts where a trap is likely. The week's curriculum deliverable, quoted, is one task.
5. `## Rookie Traps to Avoid`, `## Submit` (file names, Google Classroom, a no-internet route),
   `## Marking · 10 points` (a rubric that totals 10) and `## 📚 References`.

- Never include a worked solution or model answer. Assignment tutor notes are no longer written; the
  rubric is the marking guide.
- When asked, draft the Google Classroom post as well: title, instructions under about 1,500
  characters (Classroom formats only bold, italic, underline and bullets), points, due date, topic and
  rubric rows. Don't commit it. The tutor sets the due date.

**`class-notes.html`** (required whenever class notes are authored or revised)

- Always write and maintain an HTML presentation alongside `class-notes.md`. Markdown is the editable
  source. Keep the HTML's concepts, code, outcomes and session timings in step with it; the HTML is a
  designed teaching experience, not an unstyled Markdown dump.
- From 100L S1 Week 07, the deck follows the notes' modules: a title slide, the 120-minute route,
  the roadmap, then for each module an **Idea** slide (the mental model with one diagram or short code
  sample) and an **Act** slide (a room vote the tutor reveals, or a live editor the room predicts
  from). Never more than one idea slide before the room has to act. Then the rookie traps, the
  exercise levels with the timer, show & ship (pointing to the assignment), a reference slide and
  sources. Prefer diagrams and live renders to text walls.
- Build it from the previous week's deck engine with the scripts in `tools/deck-src/week-NN/`
  (copy the latest week's folder, then swap the slides, CSS and JS parts).
- Keep it student-only: no presenter notes, because the repository is public. Do not publish worked
  solutions to graded tasks. Label simulations and sample outputs clearly; browser activity must never
  be presented as evidence of a real device command or installation.
- Embed the full Markdown notes as the deck's reading copy, with diagrams rendered to inline SVG and
  callouts styled.
- Use the lab theme from the Week 04 presentation: monochrome paper and ink, the system monospace
  stack throughout, big rounded flat controls, and four accents that each keep one job (violet acts,
  coral draws attention, sun marks output and highlights, lime marks live state). Reuse its `:root`
  tokens and "Lab theme" rules rather than inventing colours. No full-bleed dark slides. Clear
  hierarchy, generous space and readable contrast. Use purposeful motion to explain relationships
  and state changes.
  Honour `prefers-reduced-motion` and provide a visible motion toggle.
- Make the core presentation work offline when opened directly as a file: inline CSS and JavaScript,
  embedded images only where truly needed, no runtime CDN or network dependency. Use system font
  stacks; do not embed font files — embedded base64 fonts multiply the file size for little gain.
  Preserve visual attribution. Provide keyboard and on-screen navigation, a section index, visible
  focus, and accessible controls.
- Include the phone-remote hook from the Week 04 presentation (its final script block and the
  "Phone remote" style rules) so `tools/deck-server.mjs` can drive the deck from a phone on the same
  Wi-Fi. Mark any control outside the slides that the phone should reach with `data-remote`.
  The hook must stay silent when the file is opened as `file://`.
- Verify every slide and core interaction in a real browser before delivery, including a projector
  viewport and a phone viewport. Check for clipping/overlap, keyboard use, reduced motion, shell
  variants, offline operation and JavaScript errors. Link the HTML from `curriculum/README.md`.

### This repository is public: answer keys

- Answers to **ungraded** drills and exercises may sit in `<details>` blocks in the class notes.
- **Never** commit worked solutions, model answers or answer keys for **graded** work: weekly
  deliverables, practicals, the final exam or capstone criteria. Keep those in the tutors' private
  channels.
- Never include student names, matric numbers, grades or other personal data. Example names and IDs
  must be obviously made up.

### Examples and placeholders

- For domains, use names reserved for examples (`example.com`, `*.example`) or names that are
  obviously made up. Don't use a real organisation's domain to stand in for something it isn't.
- For IP addresses, use the documentation ranges: `192.0.2.0/24`, `198.51.100.0/24`, `203.0.113.0/24`.
- Local context is welcome and helps students: naira (₦), USSD, the hostel Wi-Fi, the student portal.

### Writing style

- Use plain English and short sentences. Many readers are first-year students and some read English as
  a second language.
- Explain an idea before naming it. Define every technical term the first time it appears.
- Prefer tables, numbered steps and small diagrams to long paragraphs. Write diagrams in Mermaid, which
  GitHub renders.
- Address students as "you". Tutor notes speak to the tutor.
- Refer to people as "they" unless you know otherwise.

---

## Working with students

The programme introduces AI assistants in stages, and this policy applies to you whenever you help a
student:

| Level | Policy | What you do |
|---|---|---|
| **100L** | **Unaided.** Students build their own skills first. | Do not write, complete or fix a student's exercise, assignment, deliverable or practical, either in code or in prose. You may explain a concept, point to the matching reading in this repository or a reference site, ask guiding questions, and explain what an error message *means*. |
| **200L** | **Introduced and critiqued.** | You may suggest code, but the student must be able to explain it. Encourage them to check and question what you produce, and say when you are unsure. |
| **300L+** | **Expected professional practice.** | Help as you would a junior colleague, and still explain your reasoning. |

Assessment is based on Git history and on live, individual questioning. Work a student cannot explain
counts against them. If the student's level is unclear, assume the **strictest** policy that could apply,
or ask.

---

## Commits

- Use Conventional Commit prefixes, as in the existing history:
  - `docs:` for teaching materials and READMEs
  - `chore:` for structure and housekeeping
- Write commit messages in the imperative, and name the semester and week, for example
  `docs: add 100L-S1 week 07 pre-read, class notes, deck and assignment 04`.
- Commit only what the change needs. Don't stage files from ignored folders.
