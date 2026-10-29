<!-- layout: workbook -->
# Week 05 — Editor Lab

**100L · Semester 1 · Code Editor / IDE · Lab: 65 minutes within a 2-hour class**

## Your brief

> **Curriculum deliverable:** “Configure VS Code; first "Hello World" page opened live in the browser”.

Set VS Code up to help you, add one feature from a file, and build a page you can watch change in your
browser. Use the [class workbook](class-notes.md), especially section 6. This is 100L: no AI may write,
complete or fix your work, and VS Code's AI features stay switched off.

**Keep individual evidence.** Swap driver and navigator halfway through each part. Both learners configure
their own VS Code profile or take a turn on the shared station, and both explain results.

| Part | Time | Evidence |
|---|---|---|
| 1. Configure VS Code | 15 min | Settings file screenshot |
| 2. Install an extension offline | 10 min | Installed extension screenshot |
| 3. Hello World, live | 20 min | Page in the browser, edit log, `index.html` |
| 4. Search, format and debug drill | 15 min | Counts, before/after, Watch table |
| 5. Evidence check | 5 min | Completed checklist |
| **Total** | **65 min** | |

Start a log in your notebook with four columns. Keep **at least six meaningful entries** across Parts 1–4.

**Log headings:** What I changed · How (menu, shortcut or command) · What I expected · What happened.

## Part 1 · Configure VS Code

Open **Settings** (**Ctrl+, · ⌘,**). Use its search box to find and set each of these:

| Search for | Set it to | Why |
|---|---|---|
| `disable AI features` | ticked | 100L work is unaided |
| `auto save` | `afterDelay` | Saves your work a moment after you stop typing |
| `format on save` | ticked | Tidies the file whenever **you** press **Ctrl+S · ⌘S** |
| `font size` | a size the back row can read, at least `16` | Readable when projected |
| `word wrap` | `on` | Long lines fold instead of running off the screen |

Then run **Preferences: Open User Settings (JSON)** from the Command Palette. Every setting you changed is
written in this file. Screenshot it, and record one entry you did not expect.

**✓ What you should see:** a short file between `{` and `}`, with lines such as `"files.autoSave": "afterDelay",`
and `"chat.disableAIFeatures": true,`. A theme you chose earlier may appear too.

> **Notice:** with Auto Save set to `afterDelay`, VS Code formats only when you save yourself. Pressing
> **Ctrl+S · ⌘S** is still a good habit.

## Part 2 · Install an extension offline

1. Use workbook section 6 to install **Live Preview** from `live-preview.vsix` in your
   `edupoint-installers` folder. Use the Extensions view or the terminal route, not the online
   Marketplace search.
2. Open the Extensions view's **Installed** list. Screenshot **Live Preview** with its publisher, Microsoft.
3. In your log, write one sentence: what does this extension add that VS Code lacked?

**If blocked** for three minutes, record the exact message and ask for the prepared station. You can still
finish Part 3 using the **No extension?** route in section 6.

## Part 3 · Hello World, live

1. Use the integrated terminal to make a fresh folder named `edupoint-week05-lab` in your home folder.
   Then **File → Open Folder…** to open it. If the name already exists, agree a fresh name with the tutor.
2. Create `index.html` in the Explorer. Use **!** from the suggestion list to start the page, as in
   section 6.
3. Give it a title of your choice. Inside `<body>`, add a heading that says `Hello, World!` and one
   sentence of your own on the next line, written as `<p>…</p>`. No personal details are needed.
4. Open the page **in your browser**: Live Preview's address, or the `file:///` route if you have no
   extension. Screenshot the browser with its **address bar visible**.
5. Make **three** visible changes to your sentence or heading, one at a time. Before each, predict what the
   browser will show. Record each in your log, including whether you had to refresh.

<!-- pagebreak -->

## Part 4 · Search, format and debug drill

Work in `edupoint-week05-kit`. If you replaced `Zobbo` in class, that is fine: this drill uses other words.

1. **Search.** Every 50cl drink costs **N300** this week; next week it rises to **N350**. Search the kit
   for `N300`. Record the count and the files **before** replacing. Replace them all, then search again
   and record what VS Code reports.
2. **Format.** In your own `index.html`, add extra spaces at the start of three lines so the page looks
   messy. Screenshot it. Press **Ctrl+S · ⌘S** and screenshot again. Write which setting did the work.
3. **Debug.** In `count.js`, set a breakpoint on the line inside the `for` loop. Start debugging and add
   `total` to **Watch**. Fill in the table for **your file as it is now**: with the class fix, or without
   it if you skipped section 5. Stop debugging, run `node count.js` and record the output.

| Pause | `price` | `total` | My note |
|---|---|---|---|
| 1 | ______ | ______ | ______________________________ |
| 2 | ______ | ______ | ______________________________ |
| 3 | ______ | ______ | ______________________________ |

**Output of `node count.js`:** ____________________________________________

## Part 5 · Evidence check

Each learner checks their own evidence against the list below. Circle one feature you can demonstrate
without your partner's help. Submission gets its own ten minutes after show & tell.

<!-- pagebreak -->

## Show, explain, submit

**Show & tell · 10 minutes after the lab.** Two pairs show their page changing in the browser and explain
one VS Code feature they used. The navigator answers one question.

**Ship · final 10 minutes of class.** Git workflows arrive in week 11. Use the submission destination the
tutor announces. No pull request is required this week. Do not upload student work to this public
teaching-materials repository. The tutor confirms the due date through the class channel.

### Submit one evidence pack per learner

- Your log, with at least six meaningful entries.
- Screenshots: settings JSON, installed Live Preview, your page in the browser with the address bar
  visible, and the messy/tidied pair from Part 4.
- Your Part 4 counts, Watch table and `node count.js` output, written in the log or as a photo.
- Your `index.html` file itself.

**Naming:** use `week-05-<surname>-<firstname>-<n>.png` for screenshots or `.jpg` for photos, numbering
from 1. Rename your page `week-05-<surname>-<firstname>-index.html` when you submit it, and keep the
original in your lab folder. If combining evidence into one PDF, use `week-05-<surname>-<firstname>.pdf`.
Keep private files, other students' details and unrelated windows out of every capture.

**No internet:** save the pack locally and give it to the tutor by USB or local transfer, or hand in the
paper log for collection. The tutor records receipt; delayed connectivity must not erase your work.

## Marking · 10 points

| Criterion | Points | Evidence for full marks |
|---|---|---|
| Editor configuration | 2 | Settings JSON shows all five settings, including AI features disabled |
| Offline extension | 2 | Live Preview installed from the VSIX file, with an explanation of what it adds |
| Hello World page | 3 | Own `index.html` with title, heading and sentence; shown in a browser with its address; three predicted edits logged |
| Search, format and debug | 2 | Counts recorded before replacing; before/after formatting; a credible Watch table and output |
| Evidence and explanation | 1 | Clear, individually owned evidence and a credible explanation of the work |
| **Total** | **10** | |

The weekly-submission category remains **10% of the semester**, not 10% per lab. Equipment or installation
blockers are recorded for follow-up, not treated as a completed task or an automatic failure. Affected
criteria stay pending until the learner demonstrates them on a suitable station.

### Optional extras · after the core work, no extra marks

- Choose a different colour theme and explain why it suits a projector or a bright room.
- Find **Toggle Word Wrap** in the Command Palette and say which shortcut it shows.
- Use **Ctrl+P · ⌘P** to open three files without touching the Explorer.

<!-- pagebreak -->

## For tutors

### Run sheet · exactly 120 minutes

| Elapsed time | Minutes | What to run |
|---|---|---|
| 00:00–00:10 | 10 | Section 1: same file in a plain editor and VS Code; pairs name three differences |
| 00:10–00:16 | 6 | Section 2a: open the kit folder, Continue without Signing In, disable AI features |
| 00:16–00:20 | 4 | Section 2b: integrated terminal, listing, `node count.js` |
| 00:20–00:25 | 5 | Section 3: Format Document, auto-closing tag, suggestion list |
| 00:25–00:30 | 5 | Section 4: search `Zobbo`, read the count, replace |
| 00:30–00:35 | 5 | Section 5: the unsaved dot, then a breakpoint and Watch |
| 00:35–01:40 | 65 | Lab Parts 1–5: 15 + 10 + 20 + 15 + 5 minutes |
| 01:40–01:50 | 10 | Two short demos; ask a non-driver to explain one feature |
| 01:50–02:00 | 10 | Each learner checks evidence, saves and submits; collect offline work |

Demonstrate one action, then stop while learners try it. Zoom VS Code (**Ctrl+= · ⌘=**) so the back row
can read the projected editor. Ask “What do you expect to see?” before each reveal.

### Prepare before students arrive

- Print the pre-read, workbook and lab; save PDFs and image assets locally. No web access is needed during
  the core lesson.
- Copy the repository's `practice-kit` folder to every machine as `edupoint-week05-kit` in the home folder.
  Keep a clean copy on USB: section 4 changes the menu files, so re-copy for a learner who needs a reset.
- Add `live-preview.vsix` to each `edupoint-installers` folder. Download it once on a connected machine:
  in VS Code's Extensions view, search **Live Preview** by Microsoft, right-click it and choose
  **Download VSIX**. Record the version in the kit manifest; these notes were tested with 0.4.20.
- Keep offline VS Code and Node.js installers from week 4 for anyone still missing them. Confirm each
  station's VS Code opens a folder and runs `node count.js` in the integrated terminal.
- Preflight one Windows machine in both PowerShell and CMD, and one macOS or Linux machine, with networking
  disconnected. On macOS, check whether function keys need **fn**.
- Check that the class submission destination works, and announce the deadline through the normal class
  channel. No new deadline or assessment weight is introduced by these notes.

### Protect practice time

Cap an individual installation blockage at three minutes: record it, move the learner to a prepared
station and arrange follow-up. A learner without Live Preview completes Part 3 with the `file:///` route.
Check for AI features at the start of the lab, not after: Chat panels, inline suggestions or sign-in
prompts mean the setting is off. Disable or avoid AI assistance during assessed work.

### Ungraded answer keys

These cover the workbook's guided checks only.

- Section 4 finds **5 results in 3 files**: `monday.txt` 2, `tuesday.txt` 1, `wednesday.txt` 2.
- Section 5's paused values are 1500/0, 700/1500 and 300/700. `total = total + price;` prints
  `Order total: N2500`.

There is no public worked solution for the graded lab. Keep any marking key in the tutors' private
materials. Do not replace an individual's demonstration with their partner's result.

### Prompts for feedback

- “Which setting made that file tidy itself, and when does it run?”
- “How many matches did you expect before you pressed Replace All?”
- “What did the breakpoint show you that the printed total did not?”
- “What address is your browser showing, and what does `127.0.0.1` mean?”

### Completion and follow-up

Keep the full class to **120 minutes**: 10 warm-up + 25 guided practice + this 65-minute lab +
10 show & tell + 10 Ship. Record equipment or installation blockers and arrange an individual catch-up.
Do not silently add a mandatory second class block. Announce the actual submission deadline; these
materials intentionally do not invent one.

<!-- pagebreak -->

## Sources

- Local curriculum §4, week 5 (quoted deliverable) and §11 (assessment weights).
- [Class workbook](class-notes.md), especially sections 2–6 and its linked VS Code references.
- Microsoft: [Settings](https://code.visualstudio.com/docs/configure/settings),
  [Basic editing](https://code.visualstudio.com/docs/editing/codebasics) for `files.autoSave` and
  `editor.formatOnSave`, and [Extension Marketplace](https://code.visualstudio.com/docs/configure/extensions/extension-marketplace)
  for installing from a VSIX file. Links checked 29 October 2026.
