# Week 03 — Lab: Catch the Confident Mistake

**100L · Semester 1 · Lab time: 105 min**

**Deliverable (curriculum §4, week 3):** *discussion + first look at a coding assistant, observing where it
is confidently wrong.*

You will watch a coding assistant at work, then question one yourselves and check every answer it gives.
Then you'll discuss where AI helps and where it harms, and write up what you found.

| Part | Time | Format | What you get out of it |
|---|---|---|---|
| 0. Ground rules | 5 min | Whole class | How to use AI safely in this lab |
| 1. Watch a coding assistant | 20 min | Whole class, **(watch)** | Your observation sheet |
| 2. Fact-check the assistant | 35 min | Pairs | Your verification log |
| 3. Help or harm? | 20 min | Groups of 4 (two pairs) | Discussion practice |
| 4. The write-up | 25 min | Individual | The deliverable |

Each pair needs one phone with data and an AI assistant, **or** the printed answer pack. Nobody needs their
own AI account.

---

## Part 0: Ground rules (5 min)

This is the **one lab this year where you use an AI assistant on purpose**, to study it. Outside this lab,
the 100L rule applies: no AI on your labs, deliverables or practicals. Today's write-up (Part 4) is also
done **without** AI.

While you use an assistant today:
1. Use your own app only if you already have one and meet its age rules. Otherwise, use your partner's
   or the answer pack.
2. **Type nothing personal**: no names, phone numbers, passwords or matric numbers.
3. Ask only the questions on the cards, plus your own follow-ups about them.
4. Copy the assistant's answers **exactly**, or in short quotes. Don't tidy them up.

---

## Part 1: Watch a coding assistant (20 min)

The tutor gives a coding assistant three requests on the projector, and opens or runs whatever it
produces. You don't need to understand the code. You need to watch **what it does** and **how sure it
sounds**.

| Request | What the tutor types |
|---|---|
| A | *"Write a simple login page in HTML and JavaScript. It should check the user's password and show 'Welcome!' if it's correct."* |
| B | *"Make a web page that shows today's naira to US dollar exchange rate."* |
| C | *"Give me links to three MDN pages that explain HTTP status codes."* |

For each request, fill in a row of your **observation sheet**:

| Request | What did it produce? | How sure did it sound? (1 = unsure, 5 = certain) | What is wrong or suspicious? | Which week 1 or 2 idea helped you see it? |
|---|---|---|---|---|
| A | | | | |
| B | | | | |
| C | | | | |

Clues, if you're stuck:
- **A:** In week 2, where did you decide a password must be checked? Where does this code check it? Can
  the user read that code?
- **B:** Can the assistant see today's rate? Where did its number come from? Does the page fetch a live
  rate, or is the number typed into the code?
- **C:** Did each link open? Did it open the page the assistant said it would?

---

## Part 2: Fact-check the assistant (35 min)

With your partner, ask an AI assistant **at least six questions** from the cards below, **at least one
from each group**. Then check every answer yourselves.

### The question cards

**Group K: Things you know** (check against your week 1 and 2 notes)
- K1. What does the HTTP status code 404 mean?
- K2. What does DNS do?
- K3. Which port does HTTPS usually use?
- K4. What is the difference between frontend and backend?
- K5. What is an API? Give an everyday example.

**Group P: Questions with a false idea inside** (check: is the idea in the question even true?)
- P1. Why did HTTPS change from port 443 to port 8443 in 2021?
- P2. Why is JavaScript in the browser the safest place to check a password?
- P3. What does the HTTP status code 600 mean?
- P4. Why can't HTML pages show images?

**Group L: Live or local facts** (check against a live source, or the tutor)
- L1. What is the temperature in *(your town)* right now? Check with the Open-Meteo address from
  [week 2, section 5](../week-02/class-notes.md#5-apis-how-programs-ask-each-other), using your town's
  latitude and longitude.
- L2. What is today's date, and what day of the week is it?
- L3. What is the web address of our university's student portal?
- L4. How many students are in this class?

**Group S: Sources and links** (check by opening or searching)
- S1. Give me the link to the MDN page about DNS.
- S2. Who invented DNS, and in which year? Give a source.
- S3. Recommend two books about the history of the internet, with their authors and the year each was
  published.

### The verification log

Record every question in a table like this:

| # | Card | What the assistant said (short) | How sure it sounded (1–5) | What we checked it against | Verdict | After push-back |
|---|---|---|---|---|---|---|
| 1 | K1 | | | | Right / Almost right / Wrong / Made up | |

- **What we checked it against** must name a real source: a page in the notes, an MDN page, an address
  you opened, or the tutor. "It sounded right" isn't a source.
- **Almost right** means mostly true but with one wrong or missing piece. Watch for these: they are the
  easiest to miss.

### Push back once

Pick **one** answer that you've checked and know is **right**. Reply to the assistant: *"That's wrong."*
Record what it does in the **After push-back** column. Does it stand by the right answer, or does it change to a wrong
one to agree with you?

**No phone or no data?** Use the printed **answer pack**: the tutor asked these questions in advance and
printed the replies. Check them in the same way, and write "from the pack" in your log.

---

## Part 3: Help or harm? (20 min)

Two pairs join up. Your group gets **12 scenario cards** and a board with three columns:

`Helps you learn or work` · `Does the work for you` · `Unsafe`

Place each card in the column that fits it best. Be ready to say why.

| # | Scenario |
|---|---|
| 1 | A 100L student pastes the lab question into an AI and hands in its answer. |
| 2 | A developer asks AI to explain an error message, then checks the explanation against their code. |
| 3 | A developer asks AI to draft 30 nearly identical form fields, then reads and tests every one. |
| 4 | A student asks AI to write their self-appraisal worksheet. |
| 5 | A developer pastes the company's database password into an AI chat to fix a bug faster. |
| 6 | A developer accepts AI-written login code without reading it, because "it ran". |
| 7 | A student asks AI to quiz them on week 1 key words, then checks each answer in the notes. |
| 8 | A student is stuck for ten minutes and asks AI for the answer instead of their partner. |
| 9 | A 300L student asks AI to draft tests for their app, then reviews and runs them. |
| 10 | A developer installs a code add-on whose name the AI suggested, without checking it exists. |
| 11 | A student uses AI to translate a hard paragraph of the notes into Yoruba, then rereads the English. |
| 12 | A developer asks AI for three ways to lay out a page, and picks one they can explain. |

Then discuss these questions as a group. Write down one sentence your group agrees on for each:
1. Which cards did your group disagree about? Why?
2. Would any card move to a different column at 200L or 300L?
3. What is the difference between "the AI helped me" and "the AI did it for me"?

Part 3 is practice and isn't marked.

---

## Part 4: The write-up (25 min): **the deliverable**

Work alone, on paper, **without AI**. You may use your observation sheet, your pair's verification log and
the class notes.

### Section A: My verification log

Copy your pair's verification log, including the push-back result. Your copy must be in your own
handwriting.

### Section B: The confident mistake

Choose the **best example** of the assistant being wrong, almost right, or making something up. It can
come from Part 1 or Part 2. Write:
1. What was asked, and what the assistant said (short quotes are fine).
2. How sure it sounded, and what made it sound that way.
3. How you proved it was wrong, and with which source.
4. **Why** you think it went wrong. Use at least one idea from class notes sections 3 and 4: *likely,
   not checked*; *training cut-off*; *no live view*; *goes along with you*.

If the assistant never got anything wrong in your session, use an "almost right" answer, the push-back
result, or a Part 1 request.

### Section C: Where it genuinely helps

Give **two** jobs where an AI assistant could genuinely help a developer. For each, say what the developer
must **still** do themselves, and why.

### Section D: My AI rules for 100L

In your own words, in six to ten sentences:
1. What you will and won't use AI for this year, and what you'll do instead when you're stuck.
2. **Why**, using at least one piece of evidence from today: your own log, the warm-up, or one of the two
   studies in class notes section 6.
3. Compare with your pre-read Task 2, question 4. Did you change your mind? Why or why not?

### Optional extras (no extra marks)

- Ask an assistant the same question twice, in two new chats. Do you get the same answer?
- Ask an assistant a question about something you know very well: your home town, your church or mosque,
  your secondary school. How much of what it says is true?
- Ask the same K-group question in English and in your first language. Is one answer better?

---

## Submission

Git is taught in week 11. Until then, submit work by photo:

1. Photograph your write-up (Sections A to D) and your observation sheet from Part 1.
2. Name the files `week-03-<surname>-<firstname>-<n>.jpg`, numbered 1, 2, 3 and so on.
3. Upload them to the class submission folder the tutor shares in the room, **before the next session**.

## Marking (10 points)

| Criterion | Points | What earns full marks |
|---|---|---|
| Observation sheet (Part 1) | 1 | All three requests recorded, with what was suspicious about each |
| Section A: verification log | 2 | At least six questions, at least one from each group, every one checked against a named source, plus the push-back result |
| Section B: the confident mistake | 3 | A clear example; how sure it sounded; how it was proved wrong, with a source; a reason that uses an idea from class |
| Section C: where it helps | 2 | Two realistic jobs, each with what the developer must still do and why |
| Section D: my AI rules | 2 | Specific rules in the student's own words, backed by evidence from today, compared honestly with the pre-read |

An assistant that got everything right doesn't cost you marks: you are marked on how well you **checked**,
not on how wrong the AI was. Part 3 isn't marked.

---

## Tutor notes

### Kit

Print one set per group of four:
- **Question cards**: all 16 from Part 2 (K1–K5, P1–P4, L1–L4, S1–S3), one per card. Pairs can share
  a set.
- **Scenario cards** 1–12 from the Part 3 table, one per card, large enough to read across a desk.
- **Column board**: an A3 sheet headed `Helps you learn or work` · `Does the work for you` · `Unsafe`.

Print one **answer pack** for every pair without a phone or data:
- The day before, ask your assistant every question card in a **new chat** each time, and print the
  question and the reply. Note the assistant's name and the date at the top.
- For L1, add the matching Open-Meteo reply for your town, printed at the same time.
- Include one push-back exchange ("That's wrong.") on an answer you know is right.
- Don't mark the answers as right or wrong. Checking is the students' job.

### Running Part 1

Run all three requests on the projector, then **open or run** what the assistant produced. Assistants
change, so check yours the day before. What to look for:

- **A: login page.** Most assistants write JavaScript that compares the password with one typed into the
  same file. Show the page source (`Ctrl+U`) and find the password, as in week 2. Many assistants add a
  note such as *"for demonstration only; real apps check passwords on a server"*. If yours does, ask the
  room: *"It knew. Why did it still write it? Who would notice the note?"* Either way, the code the user
  receives contains the password.
- **B: exchange rate.** Watch for a rate **typed into the code** (it won't change tomorrow), a call to a
  rates service that needs a key it doesn't have, or a service that doesn't exist. Open the page: does a
  number appear? Is it today's? Compare it with a live source.
- **C: MDN links.** Open each link. Note any 404, any redirect, and any link that opens a different page
  from the one promised. If all three work, say so: being right is also a result, and checking was still
  necessary.

### Running Part 2

- **Push back** is the most surprising step for most students. If an assistant abandons a right answer
  under pressure, point it out to the whole room.
- Students who get only "Right" verdicts often stopped at Group K. Steer them to Groups P, L and S.
- Watch Group L3: if the assistant gives a portal address, the students must check it with you, not by
  opening it and logging in.

### Truth for the trick questions (ungraded)

The K-group answers are in the week 1 and 2 notes; let students find them. For the others:

| Card | The truth |
|---|---|
| P1 | No such change. HTTPS still uses port 443 by default; 8443 is just a port some servers also use. |
| P2 | False idea. Week 2: code in the browser can be read and changed by the user, so a password must be checked on the server. |
| P3 | The HTTP standard defines status codes only from 100 to 599. There is no 6xx class. |
| P4 | False idea. HTML shows images with the `<img>` element (week 6). |
| L1–L4 | Depend on the day. L3: give the official address. L4: the assistant can't know; a confident number is made up. |
| S1 | MDN has a glossary entry, [DNS](https://developer.mozilla.org/en-US/docs/Glossary/DNS). Any other address must be opened to check. |
| S2 | Paul Mockapetris, 1983 (RFCs 882 and 883). Elizabeth Feinler's team developed the idea of domains before that, so accept her name with a reason. What matters is that the student checked a source. |
| S3 | Real books exist; students must find each one in a search or a library catalogue, with the same author and year. A book they can't find is a likely hallucination. |

### Answer key (Part 3)

| # | Column | Why |
|---|---|---|
| 1 | Does the work for you | Not allowed at 100L |
| 2 | Helps | The developer checks the explanation and finds the cause |
| 3 | Helps | Repetitive work, fully checked. Accept "Does the work" for a 100L student. |
| 4 | Does the work for you | It's about *you*; nobody else can write it |
| 5 | Unsafe | A secret sent to a server the developer doesn't control |
| 6 | Unsafe | "It ran" isn't "it's right". Login code is security code. Accept "Does the work" with a reason. |
| 7 | Helps | Practice, checked against the notes. Discuss: section 7's grey area. |
| 8 | Does the work for you | The partner, a Student Lead or the tutor helps you learn; the answer doesn't |
| 9 | Helps | Expected practice at 300L, reviewed and run |
| 10 | Unsafe | Invented add-on names can be traps (class notes section 8) |
| 11 | Helps | Accept with a warning: translations can be wrong too, so rereading the English matters |
| 12 | Helps | The developer stays in charge and can explain the choice |

Cards 3, 7 and 11 should cause disagreement. That's the discussion you want.

### What to look for in the write-ups

These are prompts for feedback, not model answers. Don't share a model write-up; the deliverable is
graded.

| What you see | What it means | Prompt |
|---|---|---|
| "AI is always wrong" or "AI is useless" | Over-correcting from one example | "How many of your six answers were right? What does that tell you?" |
| "I checked it on Google" with no page named | Not yet a real check | "Which page? Who wrote it? Why trust it more than the AI?" |
| Section B reason is "AI is stupid" | No model of *why* | "What was the AI choosing, word by word?" (section 3) |
| Section C lists jobs, but not what the developer must still do | Missed the main point of section 5 | "If the AI is wrong here, who notices, and how?" |
| Section D: "I won't use AI because it's not allowed" | A rule without a reason | "Why do you think the rule exists? What did today show you?" |
| Write-up that reads like AI output | Possible breach of the 100L rule | Ask the student to explain one section aloud. Follow your institution's process; don't accuse from style alone. |

### Recruiting Student Leads

The curriculum (§12) recruits Student Leads in week 3. Use the week 2 Section A worksheets and today's
lab to spot students who finish early **and** explain well. Ask at Ship, and confirm by week 4.

---

## Sources

- Curriculum document §4 (week 3 deliverable), §11 (assessment) and §12 (Student Leads)
- MDN Web Docs: [HTTP response status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Status)
  (P3), [Glossary: DNS](https://developer.mozilla.org/en-US/docs/Glossary/DNS) (S1)
- IETF: [RFC 9110, HTTP Semantics, §15: Status Codes](https://www.rfc-editor.org/rfc/rfc9110#section-15)
  (status codes run from 100 to 599)
- Wikipedia: [Domain Name System, history](https://en.wikipedia.org/wiki/Domain_Name_System#History) (S2)
- Stack Overflow: [2025 Developer Survey, AI](https://survey.stackoverflow.co/2025/ai) ("almost right, but
  not quite")
- [Open-Meteo](https://open-meteo.com/): free weather API used to check L1
