<!-- layout: workbook -->
# Week 04 — Terminal Lab

**100L · Semester 1 · File System & Terminal · Lab: 65 minutes within a 2-hour class**

## Your brief

> **Curriculum deliverable:** “Command-line drills; install the toolchain from an offline installer”.

Organise a workspace using commands, then prove your tools run. Use the [class workbook](class-notes.md).
This is 100L: no AI may write, complete or fix your work. Guided practice precedes the lab;
show & tell and submission follow it.

**Keep individual evidence.** Swap driver and navigator halfway through each part. Both learners type
and explain results. Use a fresh lab folder; the guided practice folder is not your submission.

| Part | Time | Evidence |
|---|---|---|
| 1. Set your starting point | 10 min | Absolute path and initial listing |
| 2. Organise the workspace | 20 min | Before/after listings and log |
| 3. Diagnose and recover | 10 min | Error, cause and successful retry |
| 4. Offline installation station | 20 min | Tool status and verification |
| 5. Evidence check | 5 min | Completed checklist |
| **Total** | **65 min** | |

## Part 1 · Set your starting point

1. Record your shell (PowerShell, CMD or macOS/Linux). Go to your home folder and list its contents.
2. Create a fresh folder named `edupoint-week04-lab`. If it already exists, agree a fresh name with
   the tutor; do not remove earlier work. Enter the new folder.
3. Record its absolute path. Explain which part identifies the parent of your lab folder.
4. In your notebook, start a log with these four columns. Keep **at least six meaningful entries**
   across Parts 1–3, including a move, a copy, a confirmed deletion and an error/retry.

**Log headings:** Starting folder · Command I ran · My prediction · Actual result.

## Part 2 · Organise the workspace

Create folders named `incoming`, `ready` and `scratch` inside your lab folder. Create two text files,
`welcome.txt` and `checklist.txt`, inside `incoming`. In CMD, put a short word in each using `echo`.
Show the starting state before changing it; file contents are not marked.

Then use the terminal to **move** `welcome.txt` into `ready`, **copy** `checklist.txt` into `ready`
while keeping its source, and **rename** the copy to `packing-list.txt` using the move command.
Create `trial.txt` in `scratch`; inspect it, then delete **only that file** with confirmation.
Keep `scratch`. No recursive deletion or wildcards.

<!-- pagebreak -->

## Make the result visible

For Part 2, show your partner listings of `incoming`, `ready` and `scratch`. Explain which operation
kept its source and which removed it. A correct final folder alone is not enough: preserve the
command log and before/after evidence. The rubric assesses the process as well as the result.

> **Device route:** Work on your laptop or take a keyboard turn on the shared station. If no computer
> is available, trace the operations on paper and label the work “simulation”; the tutor records the
> practical as pending and arranges a catch-up. Do not label a paper trace as executed commands.

## Part 3 · Diagnose and recover

1. From your lab folder, try to enter a child named `missing-room` without creating it.
2. Record the error in your own words. Use a location check and listing to investigate it.
3. Navigate into an existing child folder instead and record the successful result.
4. Choose a file in another child folder. Write an absolute path to it and a relative path from
   your current location. Verify that both identify the same file by listing that file.
5. Explain the failed attempt and your correction to your partner. Then swap roles.

**Record:** starting location → failed command → evidence for the cause → corrected command → result.

________________________________________________________________________

________________________________________________________________________

## Part 4 · Offline installation station

Use **class workbook section 5**. Before changing anything, check which tools already work. Use
the tutor's OS-matched kit and record the machine you used as “own”, “shared” or “prepared station”.
No personal device identifiers are needed. Record which shell you used, too. Every student takes a turn launching an installer or
unpacking the Linux archive; already-installed learners use the prepared station.

| Tool | Check | Record actual result or blocker |
|---|---|---|
| Browser | Open a local PDF or the browser's start page | ______________________________ |
| VS Code | Launch the application; no extensions or coding yet | ______________________________ |
| Git | Run `git --version`; no repository commands | ______________________________ |
| Node.js | Run the version check for your installation route | ______________________________ |

For Node.js, record the installer/archive name, OS, machine route, command used to launch or unpack
it, and version result. Use “already installed”, “installed today”, “observed only” or “blocked”
honestly. The Linux portable route uses the explicit executable path from the workbook.

**If blocked:** record the exact message and ask for a prepared station after three minutes.
Permission and compatibility problems are not solved by guessing commands or downloading random
installers. Verify the other tools and record the follow-up the tutor arranges.

## Part 5 · Evidence check

Each learner checks their own log and evidence. Circle one operation you can explain without your
partner. Keep the remaining five-minute task small: organise your evidence now; submission gets its
own ten minutes after show & tell.

<!-- pagebreak -->

## Show, explain, submit

**Show & tell · 10 minutes after the lab.** Two pairs demonstrate a navigation or file operation and
an error they understood. The navigator answers one question. Everyone checks their own explanation.

**Ship · final 10 minutes of class.** Git workflows arrive in week 11. Use the submission destination
the tutor announces. No pull request is required this week. Do not upload student work to this public
teaching-materials repository. The tutor confirms the due date through the class channel.

### Submit one evidence pack per learner

- Your log: at least six meaningful entries with starting folder, command, prediction and result.
- Screenshots or clear photos of the initial and final folder listings, plus the deletion confirmation.
- Your error/retry explanation and two paths to the same file, with a successful verification.
- Your installation record and four-tool checklist. Label shared-device evidence and unresolved blockers.

**Naming:** use `week-04-<surname>-<firstname>-<n>.png` for screenshots or `.jpg` for photos, numbering
from 1. If combining evidence into one PDF, use `week-04-<surname>-<firstname>.pdf`. Keep private files,
other students' details and unrelated windows out of the capture. Submit through the class channel only.

**No internet:** save the pack locally and give it to the tutor by USB/local transfer, or hand in the
paper log for collection. The tutor records receipt; delayed connectivity must not erase your work.

## Marking · 10 points

| Criterion | Points | Evidence for full marks |
|---|---|---|
| Location and paths | 2 | Correct starting location; absolute and relative paths verified against the same file |
| File operations | 3 | Creates, moves, copies and renames as specified; deletes only the disposable file with confirmation |
| Diagnosis and reasoning | 2 | Six-entry log with predictions/results; explains the path error and demonstrates a successful retry |
| Toolchain verification | 2 | Launches/unpacks using the offline route; records status and verifies all four tools on own or shared equipment |
| Evidence and explanation | 1 | Clear, individually owned evidence and a credible explanation of the work |
| **Total** | **10** | |

The weekly-submission category remains **10% of the semester**, not 10% per lab. Hardware or permission
blockers are recorded for follow-up, not treated as a completed install or an automatic failure.
Affected practical criteria stay pending until the learner demonstrates them on a suitable station.

### Optional extras · after the core work, no extra marks

- Practise Tab completion and explain what happened when two names began with the same letters.
- Give your partner a new starting folder and ask for a route to a file without touching the mouse.
- Explain why a file renamed with a different extension may still contain the same kind of data.

<!-- pagebreak -->

## For tutors


### Run sheet · exactly 120 minutes

| Elapsed time | Minutes | What to run |
|---|---|---|
| 00:00–00:10 | 10 | Section 1: show a real file; students identify, draw and explain |
| 00:10–00:18 | 8 | Section 2: open the correct shell and create the practice folder |
| 00:18–00:25 | 7 | Section 3: predict locations; swap roles; navigate between siblings |
| 00:25–00:35 | 10 | Section 4: create, move, copy, confirm deletion, repair a bad path |
| 00:35–01:40 | 65 | Lab Parts 1–5: 10 + 20 + 10 + 20 + 5 minutes |
| 01:40–01:50 | 10 | Two short demos; ask a non-driver to explain a path or error |
| 01:50–02:00 | 10 | Each learner checks evidence, saves and submits; collect offline work |

Demonstrate one command, then stop speaking while learners try it. Keep typed text large enough to
read from the back. Ask “Where are you now?” before correcting a path. Use the diagrams as maps:
learners should point to their current node, not simply repeat command names.

### Prepare before students arrive

- Print the pre-read, workbook and lab; save PDFs and image assets locally. Draw the folder tree
  on the board if the projector fails. No web access is needed during the core lesson.
- Test the exact drills in Windows PowerShell 5.1, Command Prompt and a macOS/Linux shell used by the cohort.
  Check file-extension display and prepare one ordinary-user account for demonstrations.
- Prepare USB copies of official installers for the browser, VS Code, Git and supported Node.js LTS.
  Check OS and processor architecture; don't assume one file fits every device. Keep original file
  names, version, download source and verification details in a **kit manifest**. Distribute the Node
  copies under the short names used in section 5, without changing their contents.
- Preflight each platform with networking disconnected. Windows: omit optional build-tool downloads.
  macOS: check package permissions and compatibility. Linux: include the compatible prebuilt archive
  and test `tar`/xz support. Prepare cached packages and dependencies for other missing Linux tools.
  A package manager may otherwise try to download dependencies even when given a local package.
- Place the kit in each learner's home-folder `edupoint-installers` before the timed installation
  station. Set up spare stations for unsupported devices, missing admin permission and no-laptop learners.
- Check that the class submission destination works, and announce the deadline through the normal
  class channel. No new deadline or assessment weight is introduced by these notes.

### Protect practice time

Cap an individual installation blockage at three minutes: record it, move the learner to a prepared
station and arrange follow-up. Do not keep the whole class watching a progress bar. Verify all four
tools; don't require a reinstall if they already work. Students in that situation explain the route
and operate the prepared installation station. Disable or avoid AI assistance during assessed work.

Use the ungraded self-check boxes for discussion. The lab has a rubric, but no worked solution belongs
in this public repository. Do not replace an individual's demonstration with their partner's result.


<!-- pagebreak -->

## Sources

- Local curriculum §4, week 4 (quoted deliverable) and §11 (assessment weights).
- [Class workbook](class-notes.md), especially sections 2–5 and its linked command references.
- Software Carpentry: [Navigating files and directories](https://swcarpentry.github.io/shell-novice/02-filedir.html)
  and [Working with files and directories](https://swcarpentry.github.io/shell-novice/03-create.html),
  consulted for beginner exercise sequencing. The challenge above is original.
- [Node.js downloads](https://nodejs.org/en/download) and
  [Microsoft's msiexec reference](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/msiexec),
  consulted for the offline installation route. Links checked 26 October 2026.

## For tutors · lab delivery

### Kit and room setup

Use the preparation checklist in the preceding tutor section: offline PDFs; OS-matched installer kits and manifest;
pretested Windows, macOS/Linux and spare stations; chargers; printed logs; an offline collection route.
The `edupoint-installers` folder is separate from both the practice folder and the graded lab folder.
Have kits copied before the installation station starts. A web installer is not an offline installer.

### Run the 65-minute lab

| Part | Duration | Tutor action |
|---|---|---|
| 1 | 10 min | Check the correct shell and fresh lab folder; confirm each learner has a log |
| 2 | 20 min | Swap drivers at ten minutes; inspect process evidence, not just the final folder |
| 3 | 10 min | Ask what the error proves; require a location/listing check before suggesting a fix |
| 4 | 20 min | Rotate individual installation turns; verify version results; redirect blocked learners |
| 5 | 5 min | Check that each learner can explain one operation and has evidence ready |

Allow shared use of one workspace on a single laptop, but observe each student typing and explaining.
Collect separate logs; the students should identify their own actions. If a learner needs to repeat
the whole drill, use a fresh folder name instead of resetting or deleting somebody else's work.

### Prompts for feedback

- “What was your current folder when that relative path failed?”
- “How could you prove that a copy kept its source?”
- “Which exact file will this deletion affect?”
- “What proves the application can run, rather than merely being downloaded?”

There is no public worked solution to this graded challenge. Use the ungraded checks in the class
notes for demonstrations and discussion. Keep any marking key in the tutor's private materials.

### Completion and follow-up

Keep the full class to **120 minutes**: 10 warm-up + 25 guided practice + this 65-minute lab +
10 show & tell + 10 Ship. At the end, record equipment or installation blockers and arrange an
individual practical catch-up. Do not silently add a mandatory second class block. Announce the
actual submission deadline; these materials intentionally do not invent one.
