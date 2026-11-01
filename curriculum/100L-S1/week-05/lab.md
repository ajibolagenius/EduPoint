<!-- layout: workbook -->
# Week 05 — The Job: Show Her the Page

**100L · Semester 1 · Code Editor / IDE · Lab: 65 minutes within a 2-hour class**

## Your brief

> **Curriculum deliverable:** “Configure VS Code; first "Hello World" page opened live in the browser”.

> **Mama Titi** · 11:15 am
>
> Funmi says the total is correct now. Thank you o! But I don't understand code. Show me something I
> can see in a browser.

Set VS Code up the way a working developer would, add one feature from a file, and build a page you can
watch change in your browser. Use the [class workbook](class-notes.md): "The job" explains the ideas and
Appendix A–G has every click. This is 100L: no AI may write, complete or fix your work, and VS Code's
AI features stay switched off.

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

1. Use workbook Appendix E to install **Live Preview** from `live-preview.vsix` in your
   `edupoint-installers` folder. Use the Extensions view or the terminal route, not the online
   Marketplace search.
2. Open the Extensions view's **Installed** list. Screenshot **Live Preview** with its publisher, Microsoft.
3. In your log, write one sentence: what does this extension add that VS Code lacked?

**If blocked** for three minutes, record the exact message and ask for the prepared station. You can still
finish Part 3 using the **No extension?** route in Appendix G.

## Part 3 · Hello World, live

1. Use the integrated terminal to make a fresh folder named `edupoint-week05-lab` in your home folder.
   Then **File → Open Folder…** to open it. If the name already exists, agree a fresh name with the tutor.
2. Create `index.html` in the Explorer. Use **!** from the suggestion list to start the page, as in
   Appendix F.
3. Give it a title of your choice. Inside `<body>`, add a heading that says `Hello, World!` and one
   sentence of your own on the next line, written as `<p>…</p>`. No personal details are needed.
4. Open the page **in your browser**: Live Preview's address, or the `file:///` route if you have no
   extension. Screenshot the browser with its **address bar visible**.
5. Make **three** visible changes to your sentence or heading, one at a time. Before each, predict what the
   browser will show. Record each in your log, including whether you had to refresh.

<!-- pagebreak -->

## Part 4 · Search, format and debug drill

Work in `edupoint-week05-kit`. If you replaced `Zobbo` in class, that is fine: this drill uses other words.

1. **Search.** Mama Titi is raising the price of zobo from **N300** to **N350** next week. Search the
   kit for `N300`. Record the count and the files **before** replacing. Replace them all, then search again
   and record what VS Code reports.
2. **Format.** In your own `index.html`, add extra spaces at the start of three lines so the page looks
   messy. Screenshot it. Press **Ctrl+S · ⌘S** and screenshot again. Write which setting did the work.
3. **Debug.** In `count.js`, set a breakpoint on the line inside the `for` loop. Start debugging and add
   `total` to **Watch**. Fill in the table for **your file as it is now**: with the class fix, or without
   it if you skipped Beat 3. Stop debugging, run `node count.js` and record the output.

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
| 00:00–00:10 | 10 | Cold open: read Mama Titi's message aloud; pairs add up the order and predict why Word broke the file; room vote |
| 00:10–00:18 | 8 | Beat 1: three kinds of tool; plain editor vs VS Code; open the kit folder, disable AI features, Format Document, auto-closing tag |
| 00:18–00:26 | 8 | Beat 2: room predicts the `rice` count, then searches; search `Zobbo`, read the preview, replace |
| 00:26–00:35 | 9 | Beat 3: integrated terminal, `node count.js`, breakpoint and Watch; the unsaved fix, then save |
| 00:35–01:40 | 65 | Lab Parts 1–5: 15 + 10 + 20 + 15 + 5 minutes |
| 01:40–01:50 | 10 | Two short demos; ask a non-driver to explain one feature |
| 01:50–02:00 | 10 | Each learner checks evidence, saves and submits; collect offline work |

Each beat runs Problem → Idea → Try. Read the story problem aloud in under a minute, teach the idea
with its diagram in two to three minutes, then stop talking: learners spend the rest of the beat
trying. Name the myth out loud before the try; it is what learners will otherwise believe.
Demonstrate one action, then stop while learners try it. Zoom VS Code (**Ctrl+= · ⌘=**) so the back row
can read the projected editor. Ask “What do you expect to see?” before each reveal.

### Prepare before students arrive

- Read the 100L S1 story bible, `curriculum/100L-S1/story.md`, so the characters and the cliffhanger
  stay consistent with later weeks.
- Print the pre-read, workbook and lab; save PDFs and image assets locally. No web access is needed during
  the core lesson.
- Copy the repository's `practice-kit` folder to every machine as `edupoint-week05-kit` in the home folder.
  Keep a clean copy on USB: Beat 2 changes the menu files, so re-copy for a learner who needs a reset.
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

- Cold open: the order should total **₦2,500**. Word saves its own format and curly quotes, not plain
  text.
- Beat 2: `rice` finds **8 results in 3 files** (`count.js` 5 from "price" and "prices",
  `monday.txt` 2, `messy.html` 1). With **Match Whole Word** it finds **3 results in 2 files**.
  `Zobbo` finds **5 results in 3 files**: `monday.txt` 2, `tuesday.txt` 1, `wednesday.txt` 2.
- Beat 3: the paused values are 1500/0, 700/1500 and 300/700. With `total = total + price;` unsaved,
  `node count.js` still prints `Order total: N300`; after saving it prints `Order total: N2500`.

There is no public worked solution for the graded lab. Keep any marking key in the tutors' private
materials. Do not replace an individual's demonstration with their partner's result.

### Prompts for feedback

- “Which setting made that file tidy itself, and when does it run?”
- “How many matches did you expect before you pressed Replace All?”
- “What did the breakpoint show you that the printed total did not?”
- “Your fix is on screen but the output hasn't changed. What are your two suspects?”
- “What address is your browser showing, and what does `127.0.0.1` mean?”

### Completion and follow-up

Keep the full class to **120 minutes**: 10 warm-up + 25 guided practice + this 65-minute lab +
10 show & tell + 10 Ship. Record equipment or installation blockers and arrange an individual catch-up.
Do not silently add a mandatory second class block. Announce the actual submission deadline; these
materials intentionally do not invent one.

<!-- pagebreak -->

## Sources

- Local curriculum §4, week 5 (quoted deliverable) and §11 (assessment weights).
- [Class workbook](class-notes.md), especially Beats 1–3, "The job" and Appendix A–G.
- Microsoft: [Settings](https://code.visualstudio.com/docs/configure/settings),
  [Basic editing](https://code.visualstudio.com/docs/editing/codebasics) for `files.autoSave` and
  `editor.formatOnSave`, and [Extension Marketplace](https://code.visualstudio.com/docs/configure/extensions/extension-marketplace)
  for installing from a VSIX file. Links checked 29 October 2026.
