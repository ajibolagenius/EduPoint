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
    week-01/
      pre-read.md           student-facing: read before the session
      class-notes.md        student-only notes, projected in class; students practise along
      class-notes.html      required interactive presentation of the same student-only notes
      lab.md                student-facing: the lab and deliverable, with tutor notes at the end
    assignments/
      assignment-NN.md      student-facing: take-home work spanning several weeks
      assignment-NN-tutor-notes.md   for tutors: purpose, checks, feedback prompts; never the answer key
```

- Create one folder per week, named `week-NN` with two digits.
- Each week has the three Markdown sources above and a required `class-notes.html` presentation.
  Add other files only if the week really needs them, such as matching PDFs or a printable handout.
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
- From Week 04, include relevant raster images (for example, real interface screenshots) and
  Mermaid diagrams beside the concepts they explain. Give images meaningful alt text, a caption,
  source and licence; store them under the week's `assets/` folder for offline use. Each visual
  should support a question or activity. Keep Mermaid source editable in Markdown and render it
  in the PDF. Follow the workbook layout conventions in `curriculum/README.md`.

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

  | Part | Time |
  |---|---|
  | Warm-up | 10 min |
  | Guided concept and student practice | 25 min |
  | Lab | 65 min |
  | Show & tell | 10 min |
  | Ship | 10 min |

  Session plans must total exactly 120 minutes, including transitions, saving and submission.
  Pre-reading and optional extensions are outside class time. Interleave short demonstrations with
  student attempts, expected results and checks; the lab takes most of the session. Before Git is
  taught, Ship means saving files and submitting evidence. Shorten older plans before reusing them.
- **Teach only what students know so far.** Don't use a tool, language or concept before the week
  that introduces it. For example, in 100L S1 the terminal arrives in week 4, VS Code in week 5, HTML in
  week 6 and Git in week 11. When a reading mentions a tool students haven't met yet, tell them to skip
  that part.
- **Plan for poor connectivity.** Students may have no laptop or no data. Give a no-internet fallback
  for anything that depends on the network, and prefer activities that work offline.
- **Submissions.** Weekly submissions are merged pull requests once Git has been taught. Before that,
  the lab must say exactly how to submit and how to name the files.
- **Grading weights** are fixed by the curriculum document:

  | Component | Weight |
  |---|---|
  | Weekly submissions | 10% |
  | Mid-semester practical | 15% |
  | Milestones | 15% |
  | Final practical | 35% |
  | Demo & defence | 25% |

  Never change these in a lab's rubric.

### What each file contains

**`pre-read.md`** (for students, about 30–45 minutes of work)
- What the session is about, in two or three sentences
- Short readings, in order, each with one question to keep in mind
- Anything to do before reading, and what to bring
- A note on what to do if the student has no internet

**`class-notes.md`** (for students; projected in class, and used for revision and catch-up)

The tutor projects these student-only notes. **Class notes are a workbook, not a lecture:** the
student acts first and reads the explanation of what just happened second. A student who missed the
session must be able to work through the notes alone.

- "How to use these notes" in one short paragraph, then the learning outcomes.
- **Write each outcome as something the tutor can see happening on a device** — *find, create, move,
  diagnose, launch* — not *explain* or *describe*. Where understanding is the point, bolt it to an
  action: "open two sites, compare the address bars, then explain what differs."
- Numbered concept sections, each in this order:
  - **▶ Try it** first: numbered steps, marked **(laptop)**, **(phone)**, **(paper)** or **(watch)**.
    Nothing is explained until the student has done something concrete.
  - **✓ What you should see**: paste the **real output or screen** the student gets — a terminal
    block, a panel, a dialog — so they compare it instead of guessing whether they broke something.
  - **What you just saw**: at most three lines that now name and define the concept the student has
    met. Theory belongs here, and this is the last place a reader reaches it.
  - **? Check**: one question, with the answer hidden in a
    `<details><summary>Answer</summary>…</details>` block.
- **Doing must outweigh reading.** If a section takes longer to read than to try, cut the prose, never
  the activity. Prefer a short real transcript to a paragraph describing it.
- **Cap passive time.** At most one **(watch)** step per session. Where the room has too few machines,
  turn it into a **(phone)** task or a shared-keyboard turn. **(paper)** is a parallel route for a
  student with no device, not a substitute for a keyboard turn when one is available.
- Key words (a glossary), common questions (also in `<details>` blocks), and Read more. Keep Read more
  to links a student should really open; put full attribution in a short Sources list.
- **Never include a "For tutors" section or tutor-only guidance in class notes or their PDF.**
  Put the session run sheet, preparation checklist, demo tips and private teaching logistics in
  the lab's final tutor section. Students may still have a short agenda showing their own activities.

**`lab.md`** (for students first, tutors at the end)
- The deliverable, quoted from the curriculum document
- Parts with times and formats
- Clear requirements
- Optional extras
- Submission instructions
- A rubric that totals 10 points
- Tutor notes: the kit to prepare, how to run the activities, and answer keys

**`class-notes.html`** (required whenever class notes are authored or revised)

- Always write and maintain an HTML presentation alongside `class-notes.md`. This starts with
  100L S1 Week 04; earlier weeks need conversion when their notes are next revised. Markdown remains
  the editable workbook source. Keep the HTML's concepts, commands, outcomes and session timings in
  step with it; HTML is a designed teaching experience, not an unstyled Markdown dump.
- Keep it student-only and hands-on first. Include meaningful interactions with feedback, such as
  navigable diagrams, prediction/reveal steps, safe simulations or ungraded knowledge checks.
  Do not publish worked solutions to graded tasks. Label simulations and sample outputs clearly;
  browser activity must never be presented as evidence of a real device command or installation.
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

- Answer keys for **ungraded** in-class activities may go in the tutor notes.
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
| **100L** | **Unaided.** Students build their own skills first. | Do not write, complete or fix a student's lab, deliverable or practical, either in code or in prose. You may explain a concept, point to the matching reading in this repository or a reference site, ask guiding questions, and explain what an error message *means*. |
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
  `docs: add 100L-S1 week 02 pre-read, class notes and lab`.
- Commit only what the change needs. Don't stage files from ignored folders.
