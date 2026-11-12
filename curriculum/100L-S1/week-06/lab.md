<!-- layout: workbook -->
# Week 06 — The Job: Your Own Page

**100L · Semester 1 · HTML I — Structure · Lab: 65 minutes within a 2-hour class**

## Your brief

> **Curriculum deliverable:** “Start the Personal Portfolio: structure only”.

> **Mama Titi** · 2:30 pm
>
> Ehen! Now that is a menu. Funmi showed her coursemates, and they keep asking who made it and what else
> you have built. What should she tell them?

Build the first version of your **portfolio**: one page about you and your work, written in HTML,
**structure only**. Use the [class workbook](class-notes.md): Beats 1–3 and "The job" explain each element,
and Appendix B–G has every click, path and command. This is 100L: no AI may write, complete or fix your
work, and VS Code's AI features stay switched off.

**Your page is your own.** Pairs may talk through plans and test each other's pages, but each learner
writes their own `index.html` with their own words, on their own machine or a shared-station turn.

| Part | Time | Evidence |
|---|---|---|
| 1. Plan on paper | 10 min | A photo of your outline and tree |
| 2. Skeleton | 10 min | `index.html` with a complete `head` |
| 3. Fill the structure | 25 min | Your page in the browser |
| 4. Test it like a stranger | 15 min | Four test results in your log |
| 5. Evidence check | 5 min | Completed checklist |
| **Total** | **65 min** | |

Keep a log in your notebook with four columns. Keep **at least six meaningful entries** across Parts 2–4.

**Log headings:** What I changed · Why · What I expected · What happened.

## Part 1 · Plan on paper

1. Write your page's **outline**: the `h1`, then three or more `h2` section titles in order. Under each,
   write what goes there: a paragraph, a list, the image, the table.
2. Draw your page as a **tree**, like the diagrams in the workbook: `body` at the top, each element
   hanging from the one it sits inside.
3. Decide which section gets an `id` for a jump link, and which two or more elements will share a
   `class` because they belong together.

Photograph the page for your evidence.

## Part 2 · Skeleton

1. In your **home folder**, make a folder named `portfolio`, with a folder named `images` inside it.
   **Keep this folder all semester.** It grows each week, and in week 11 it goes on GitHub.
2. Open `portfolio` in VS Code. Create `index.html` and start it with **!** *(Appendix B)*.
3. Give the page a `<title>` with the name you want readers to see, such as `Ada · Portfolio`. Check that
   the `head` keeps `<meta charset="UTF-8">` and the `html` element keeps `lang="en"`.
4. Copy your image into `images`, renamed in lowercase with no spaces. Copy your week 5 page into
   `portfolio` and name it `hello.html`. If you have no week 5 page, make a short `hello.html` with **!**
   and one heading.
5. Preview `index.html` in your browser *(Appendix A)*.

## Part 3 · Fill the structure

Your page must contain all of these. Write every sentence yourself.

| Requirement | Detail |
|---|---|
| Headings | One `h1`; at least three `h2` sections in a sensible order; no skipped levels |
| Paragraphs | At least two `p` elements in your own words |
| Lists | One `ul` and one `ol`, each with three or more `li`. Use `ol` only where the order matters |
| Image | One `img` from your `images` folder with a relative `src` and an `alt` that describes it |
| Table | One `table` with a header row of `th` cells and at least three rows of `td` cells, such as what you have learnt each week |
| Links | One to a page on the web, one relative link to `hello.html`, and one jump link to an `id` on this page |
| `id` and `class` | Every `id` is unique; at least two elements share a `class` |

**Structure only.** No colours, fonts or layout: no `style` attribute, no `<style>` element and no
`border` attribute. Those arrive in week 8.

**Privacy.** Use the name you want employers to see. Leave out phone numbers, your home address, your
matric number and anyone else's details.

<!-- pagebreak -->

## Part 4 · Test it like a stranger

Run each test, then record the result in your log.

1. **Move test.** Copy the whole `portfolio` folder somewhere else: a USB stick, or your Desktop. Open
   `index.html` from the copy. Do the image and the link to `hello.html` still work? Delete the copy
   afterwards. If anything broke, a path points outside the folder: fix it and test again.
2. **`alt` test.** Change one letter in your image's `src` and save. Does the `alt` text tell a stranger
   what the image showed? Screenshot it, then change the letter back.
3. **Jump test.** Click your jump link. Screenshot the browser with the address bar showing the `#`.
4. **Outline test.** Your partner reads **only your headings** aloud, top to bottom. Does it sound like a
   contents list? Write down one thing your partner suggested.

**If you are online (optional):** paste your code into the W3C checker's
[Validate by direct input](https://validator.w3.org/#validate_by_input) tab and record how many errors it
reports. Fix what you understand.

## Part 5 · Evidence check

Check your evidence against the list below. Circle one element you can explain without your notes.
Submission gets its own ten minutes after show & tell.

## Show, explain, submit

**Show & tell · 10 minutes after the lab.** Three learners show their page in the browser, click their
jump link and explain one choice: why an `ol`, why that `alt` text, or why that table.

**Ship · final 10 minutes of class.** Git arrives in week 11. Use the submission destination the tutor
announces. Do not upload student work to this public teaching-materials repository. The tutor confirms
the due date through the class channel.

### Submit one evidence pack per learner

- Your `portfolio` folder, zipped whole so the image travels with it *(Appendix G)*.
- Screenshots: your page in the browser with the address bar visible, your table, the `alt` test and the
  jump test.
- A photo of your Part 1 outline and tree.
- Your log, with at least six meaningful entries, including the four test results.

**Naming:** `week-06-<surname>-<firstname>-portfolio.zip` for the folder,
`week-06-<surname>-<firstname>-<n>.png` (or `.jpg`) for screenshots and photos, numbered from 1. Keep
your working `portfolio` folder unchanged: you build on it next week.

**No internet:** save the pack locally and give it to the tutor by USB or local transfer, or hand in the
paper log for collection. The tutor records receipt; delayed connectivity must not erase your work.

## Marking · 10 points

| Criterion | Points | Evidence for full marks |
|---|---|---|
| Page skeleton | 2 | `DOCTYPE`, `html` with `lang`, `head` with `meta charset` and your own `title`, content inside `body` |
| Headings and text | 2 | One `h1`, three or more `h2` in order, two own paragraphs, a `ul` and an `ol` each used for the right reason |
| Image and links | 2 | An image with a relative `src` and a meaningful `alt`; working web, relative and jump links |
| Table, `id` and `class` | 2 | A table with a header row and three or more data rows; unique `id`s; a shared `class` |
| Testing and explanation | 2 | Plan, four test results and log; can explain any element on the page in their own words |
| **Total** | **10** | |

The weekly-submission category remains **10% of the semester**, not 10% per lab. Styling is not marked
and earns nothing; remove it before submitting. Equipment blockers are recorded for follow-up, not
treated as a completed task or an automatic failure. Affected criteria stay pending until the learner
demonstrates them on a suitable station.

### Optional extras · after the core work, no extra marks

- Add a second page, such as `projects.html`, with a link to it from `index.html` and a link back.
- Add a contents list at the top of your page: a `ul` of jump links, one per section.
- Find three websites you use and say which parts of each would be a table, a list or a heading.

<!-- pagebreak -->

## For tutors

### Run sheet · exactly 120 minutes

| Elapsed time | Minutes | What to run |
|---|---|---|
| 00:00–00:10 | 10 | Cold open: read the two messages; pairs predict A–D on paper and mark T/L/S; room vote; open `menu.html` in the browser |
| 00:10–00:19 | 9 | Beat 1: element anatomy and the skeleton tree; heading-size myth vote; learners tag headings, paragraph and three lists; delete one `</h2>` |
| 00:19–00:27 | 8 | Beat 2: attributes and relative paths; learners add the broken `img`, fix the path, add the link; the copy-only-`menu.html` test |
| 00:27–00:35 | 8 | Beat 3: row-by-row tables; layout myth; learners replace the menu `ul` with the table from `prices.txt` |
| 00:35–01:40 | 65 | Lab Parts 1–5: 10 + 10 + 25 + 15 + 5 minutes, opening with the `id`/`class` briefing from "The job" |
| 01:40–01:50 | 10 | Three short demos; ask a non-driver to explain one element |
| 01:50–02:00 | 10 | Each learner zips, names and submits; collect offline work |

Each beat runs Problem → Idea → Try. Read the story problem aloud in under a minute, teach the idea with its
diagram in two to three minutes, then stop talking: learners spend the rest of the beat typing. Name the
myth before the try. Zoom VS Code (**Ctrl+= · ⌘=**) and the browser so the back row can read both. Ask
"What do you expect to see?" before every refresh.

### How to deliver the beats live

- **Cold open.** Don't open the file in a browser until the vote is in. The reveal works best on the
  projector: show the deck's live render, then have learners open their own copy.
- **Beat 1.** Type the first `<h1>` yourself, save and refresh, then stop. Learners do the rest. The
  deliberate `</h2>` deletion in step 6 is the beat's payoff: let them see the damage before you explain.
- **Beat 2.** Insist on the wrong `src` first. A learner who has seen the `alt` text standing in remembers
  why `alt` matters and why paths start from the page's folder.
- **Beat 3.** Build the header row together, then let pairs race through the data rows. Learners who finish
  early count their `tr`, `th` and `td` elements for the check.

### Prepare before students arrive

- Read the story bible, `curriculum/100L-S1/story.md`, so names and the cliffhanger stay consistent.
- Print the pre-read, workbook and lab; save the PDFs and image assets locally. No web access is needed
  during the core lesson.
- Copy the repository's `practice-kit` folder to every machine as `edupoint-week06-kit` in the home
  folder. Keep a clean copy on USB: learners change `menu.html` throughout the beats.
- Check that Live Preview from week 5 still works on each station; the `file:///` route in workbook
  Appendix A is the fallback.
- Bring a USB stick for Part 4's move test, or let learners use the Desktop.
- Preflight on one Windows machine in PowerShell and CMD, and one macOS or Linux machine, with networking
  disconnected: open `menu.html`, build the table, and zip a test folder with both the clicks and the
  terminal route in Appendix G.
- The CampusChop link in Beat 2 is meant to fail: `.example` names are reserved and never resolve. The
  optional validator in Part 4 is the only step that needs the internet.
- Check that the class submission destination accepts `.zip` files, and announce the deadline through the
  normal class channel. No new deadline or assessment weight is introduced by these notes.

### Protect practice time

Cap an individual blockage at three minutes: record it, move the learner to a prepared station and
arrange follow-up. Learners without Live Preview use the `file:///` route and refresh by hand. Check for
AI features at the start of the lab, not after. Watch for learners copying the menu page's structure
word for word into the portfolio: the elements may match, but the sections and sentences must be their
own.

### Ungraded answer keys

These cover the workbook's guided checks only.

- Cold open: **B**, one long paragraph. Four titles (shop name and three sections), eight list items, three
  steps and one sentence.
- Beat 1: "How to order" is an `ol` because the steps happen in order. Deleting the `</h2>` after "Why
  students eat here" turns that section's three bullet points into heading text; the damage ends at the
  next `<h2>`.
- Beat 2: `src="jollof.jpg"` shows the broken-image icon and the `alt` text; `images/jollof.jpg` works.
  A copy of `menu.html` alone loses the photo. Renaming `images` to `photos` needs `src="photos/jollof.jpg"`.
- Beat 3: **6** `tr`, **3** `th`, **15** `td`.
- The job: `href="#Skills"` doesn't match `id="skills"`, because capitals count.

There is no public worked solution for the graded lab. Keep any marking key in the tutors' private
materials. Do not accept a partner's page as an individual's evidence.

### Prompts for feedback

- "Read me your headings only. Is that the outline of your page?"
- "Why is this list numbered? What would change if the items swapped places?"
- "Close your eyes: I'll read your `alt` text. Do I know what the picture shows?"
- "Your folder moves to a USB stick. Which of your paths still work, and why?"
- "Why is this an `id` and that a `class`?"

### Completion and follow-up

Keep the full class to **120 minutes**: 10 warm-up + 25 guided practice + this 65-minute lab +
10 show & tell + 10 Ship. Record equipment blockers and arrange an individual catch-up. Do not silently
add a mandatory second class block. Announce the actual submission deadline; these materials
intentionally do not invent one.

<!-- pagebreak -->

## Sources

- Local curriculum §4, week 6 (quoted deliverable) and §11 (assessment weights).
- [Class workbook](class-notes.md), especially Beats 1–3, "The job" and Appendix A–G.
- MDN contributors: [Basic HTML syntax](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/Basic_HTML_syntax),
  [HTML images](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/HTML_images),
  [Creating links](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/Creating_links),
  [HTML table basics](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/HTML_table_basics).
  W3C: [Markup Validation Service](https://validator.w3.org/#validate_by_input). Links checked 12
  November 2026.
