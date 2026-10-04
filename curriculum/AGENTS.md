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
      class-notes.md        projected in class; students practise along; tutor section at the end
      lab.md                student-facing: the lab and deliverable, with tutor notes at the end
```

- Create one folder per week, named `week-NN` with two digits.
- Each week has exactly the three files above. Add another file only if the week really needs one,
  such as a printable handout.
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

- **Session structure.** Each session is one block of about 3 to 3.5 hours:

  | Part | Time |
  |---|---|
  | Warm-up | 10–15 min |
  | Concept | 45–60 min |
  | Lab | 90–120 min |
  | Show & tell | 15 min |
  | Ship | 10 min |

  Session plans must fit these timings. Keep the concept part short; the lab takes most of the time.
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

The tutor projects these notes. Students read a short explanation, then do it on their own device while
the tutor demonstrates. A student who missed the session must be able to work through the notes alone.

- "How to use these notes", then the learning outcomes, written as things a student "can do"
- Numbered concept sections. In each one, keep the explanation to about two minutes of reading, then
  use this pattern:
  - **▶ Try it**: numbered steps. Mark each with what it needs: **(phone)**, **(laptop)**, **(paper)**,
    or **(watch)** for the tutor's screen only.
  - **✓ What you should see**: the expected result, so a student working alone can tell it worked.
  - **? Check**: one question, with the answer hidden in a
    `<details><summary>Answer</summary>…</details>` block.
- Key words (a glossary), common questions (also in `<details>` blocks), and Read more
- **For tutors**, last: the session plan with timings, a prep checklist including offline fallbacks,
  and tips for running each demo

If a section takes longer to read than to try, it is too long. The concept time is for doing, not
reading off the screen.

**`lab.md`** (for students first, tutors at the end)
- The deliverable, quoted from the curriculum document
- Parts with times and formats
- Clear requirements
- Optional extras
- Submission instructions
- A rubric that totals 10 points
- Tutor notes: the kit to prepare, how to run the activities, and answer keys

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
