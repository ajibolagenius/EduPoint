# Assignment 01 — The CampusChop Case File

**100L · Semester 1 · Covers weeks 1–3 · Take-home · About 3 hours · Marked out of 10**

This assignment brings the first three weeks together. You'll investigate one made-up app from every
angle you've learned so far:

| Task | What you do | Draws on | Marks |
|---|---|---|---|
| 1. Map it | Draw how an order travels from a student's phone to CampusChop and back | Weeks 1 and 2 | 3 |
| 2. The support desk | Work out what went wrong in eight complaints | Weeks 1 and 2 | 2 |
| 3. Who does the job? | Decide which part of the system does each feature, and read an API reply | Week 2 | 2 |
| 4. Check the AI's plan | Fact-check a plan written by a coding assistant | Weeks 1, 2 and 3 | 2 |
| 5. Three weeks, one picture | Explain how the weeks connect, and rate yourself again | Weeks 1–3 | 1 |

You don't need the internet for any part of it. Everything you need is in this case file and your class
notes for [week 1](../week-01/class-notes.md), [week 2](../week-02/class-notes.md) and
[week 3](../week-03/class-notes.md).

---

## Before you start

**The rules**

1. **Unaided.** This is 100L work, so no AI tool may write, complete, check or fix any part of it. That
   includes writing helpers built into word processors, such as "Help me write" in Google Docs or Copilot
   in Word. Task 4 is *about* an AI's answer, and you check it with your notes, not with another AI.
2. **On paper or on a laptop, your choice.** Handwrite it, or type it in any word processor (Word,
   Google Docs, LibreOffice). For the Task 1 diagram, you can draw on paper and photograph it, or draw it
   on the laptop in [Excalidraw](https://excalidraw.com/) or any drawing app. You can mix the two, for
   example typed answers with a photographed diagram.
3. **Your own words.** You may talk ideas over with your partner, but you may not share written answers.
   If two scripts match, both lose the marks for that task.
4. **Be ready to explain.** Your tutor may ask you to explain any answer aloud. Work you can't explain
   counts against you.

**What you need:** paper and a pen (with a second colour for Task 1), or a laptop, plus your notes from
weeks 1–3.

**Plan your time.** Spread the work over a few days. Task 1 takes the longest, so start with it.

---

## The case file

> **CampusChop** is a food-ordering service for a university campus. It is made up for this assignment.
>
> - Students order meals from campus canteens on the website **`campuschop.example`**, or on the
>   **CampusChop mobile app** for Android and iPhone.
> - Both the website and the app get their data from the **same CampusChop backend**, through the
>   **CampusChop API**.
> - CampusChop's server is at the IP address **`198.51.100.40`**.
> - Students log in with an email address and a password. Every page uses HTTPS.
> - Menus, prices, carts, orders and accounts are stored in a **database** on CampusChop's server.
> - Canteen owners (vendors) change their menus and prices from a **vendor dashboard** on the website.

---

## Task 1 — Map it (3 marks)

A student opens `campuschop.example` in their phone's browser, logs in, and orders a plate of jollof
rice. Draw the whole journey, from the moment they type the address to the moment the "Order placed"
page appears.

### Your diagram must show

- **Every part, in order:** Student → Browser → DNS → Server (backend) → Database → Response → Browser.
- **The IP address** from the case file, in the right place.
- **Where the password is checked.** Mark it with a ★.
- **HTTPS**, on the link where it belongs.
- **The mobile app** as a second frontend. Show that it reaches the **same backend** through the API.
- **Labelled arrows.** Every arrow says what travels along it.
- **Requests and responses that look different,** for example solid and dashed arrows, or two colours.
  Add a key.
- **No more than 12 boxes.**

### Under your diagram, write

1. **The journey, step by step.** Number the steps, as in
   [week 1, section 7](../week-01/class-notes.md#7-the-whole-journey). There should be six to ten steps,
   in your own words. After each step, write which part does the work in brackets: *(frontend)*,
   *(backend)*, *(database)* or *(DNS)*.
2. **After Task 2:** come back to your diagram and mark **three** of the support tickets on it. Write
   the ticket number in a ✗ at the exact place where that problem breaks the journey.

---

## Task 2 — The support desk (2 marks)

You're working on CampusChop's support desk. These eight complaints arrived this week:

| # | Ticket |
|---|---|
| 1 | *"I typed `campuschop.exmaple` on my laptop and got: This site can't be reached. The server's DNS address could not be found."* |
| 2 | *"When I tap Track my order, the page just says 500 Internal Server Error."* |
| 3 | *"The menu loads, but it's plain black text in a long list. No pictures, no colours, nothing in columns."* |
| 4 | *"I clicked a link in a group chat to get free food. My browser said Your connection is not private, and the address bar showed `campuschop-free.example`."* |
| 5 | *"I put jollof and a drink in my cart on my phone. Later I logged in on a library computer and my cart was empty."* |
| 6 | *"Someone in our hostel says they used developer tools to change the price of their meal to ₦50, and they got a Payment successful page."* |
| 7 | *"Mama Titi's canteen changed its prices an hour ago. My friend sees the new prices, but I still see yesterday's."* |
| 8 | *"With airplane mode on, the app still opens and shows my past orders, but Place order does nothing."* |

Make a table with these columns and fill in one row per ticket:

| # | What failed, or what is happening | Whose side is it on? | Your advice, in one sentence |
|---|---|---|---|
| 1 | | | |

- **What failed, or what is happening:** name the step or part, using week 1 and 2 words: DNS,
  connection, certificate, request (4xx), server (5xx), database, follow-up files, cache, frontend,
  backend.
- **Whose side is it on?** Choose *the user's device or network* or *CampusChop's servers*. Some tickets
  may be **working exactly as designed**. If so, write that and say why.
- **Your advice** goes to the user, or to the CampusChop team if they're the ones who must fix it.

**Ticket 6 is the most serious one.** Under your table, write two or three sentences explaining *why* it
is serious, and where the price must be decided instead.

---

## Task 3 — Who does the job? (2 marks)

### Part A: Place the features

For each feature, write the part that does its **main job**, and one line saying why. Choose from:
`HTML & CSS alone` · `JavaScript in the browser` · `Backend` · `Database`.

| # | CampusChop feature |
|---|---|
| A1 | The menu page, with each meal's name, photo and price |
| A2 | The menu rearranging itself into one column on a small phone |
| A3 | A running total that updates as you tap + and − on your cart |
| A4 | Checking that a discount code like `FRESHERS10` is real and hasn't expired |
| A5 | Your order history, the same on the website and on the app |
| A6 | Stopping one vendor from changing another vendor's prices |
| A7 | A "Show ingredients" box that opens and closes |
| A8 | The number of plates of jollof sold today, across every student |

If a feature needs the server, ask yourself whether its main job is **deciding** (backend) or
**remembering** (database), as in [week 2, section 4](../week-02/class-notes.md#4-everything-you-receive-you-can-read).

### Part B: Read an API reply

When the app shows "Track my order", it asks the CampusChop API and gets back this reply:

```json
{
  "order_id": "CC-20481",
  "status": "on_the_way",
  "vendor": "Mama Titi's Kitchen",
  "items": [
    { "name": "Jollof rice and chicken", "qty": 1, "price": 2500 },
    { "name": "Bottled water", "qty": 2, "price": 300 }
  ],
  "total": 3100,
  "eta_minutes": 12
}
```

Answer in full sentences:

1. Where is the order now, and how long until it arrives?
2. Check the total yourself. Show your working in naira. Is the reply's total correct?
3. This reply has no colours, no fonts and no pictures. Why not? Who, or what, is it written for?
4. The website and the app show exactly the same order details. Explain how, using the words *API* and
   *backend*.
5. The app asks for order `CC-99999`, which doesn't exist. Which group of status codes (2xx, 3xx, 4xx or
   5xx) should the API reply with, and why?

---

## Task 4 — Check the AI's plan (2 marks)

A CampusChop developer asked a coding assistant: *"Write a short technical plan for CampusChop."* Here
are eight sentences from its answer. It sounded equally sure about every one.

> 1. When a student types `campuschop.example`, DNS turns the name into an IP address such as
>    `198.51.100.40` before any request is sent.
> 2. To make login faster, the app should check the vendor's password in JavaScript on the user's
>    phone, so no request to the server is needed.
> 3. All traffic should use HTTPS, which has run on port 8443 since 2021.
> 4. Each student's cart should be stored in their browser only. That way it appears on any device they
>    log in from.
> 5. HTTPS stops the hostel Wi-Fi owner from reading a student's order, and it also stops CampusChop
>    itself from seeing what students order.
> 6. The website and the mobile app can both talk to the same backend through one API.
> 7. According to the 2025 Nigerian Campus Food Survey, 87% of students order food online at least twice
>    a week.
> 8. HTML and CSS alone can make the menu change its layout to fit a small phone screen.

### Part A: The verification log

Make a log like the one from the week 3 lab, with one row per sentence:

| # | Verdict | What I checked it against | If it's not right: the correction, in my own words |
|---|---|---|---|
| 1 | | | |

- **Verdict:** *Right*, *Almost right*, *Wrong* or *Made up / can't be checked*.
- **What I checked it against** must be specific, for example "Week 1 notes, section 6". "I just know" is
  not a source.

### Part B: The most dangerous mistake

Choose the sentence that would do the **most harm** if CampusChop built it as written. In four to six
sentences:

1. Say what could happen to real students or vendors.
2. Explain **why** the assistant might have written it. Use one reason from
   [week 3, section 4](../week-03/class-notes.md#4-confidently-wrong): *likely, not checked*;
   *training cut-off*; *no live view*; *goes along with you*.
3. Name the stage of the software development lifecycle
   ([week 2, section 8](../week-02/class-notes.md#8-the-software-development-lifecycle)) where the team
   should have caught it, and say how.

---

## Task 5 — Three weeks, one picture (1 mark)

1. **Explain it to a classmate.** A new student joins in week 4 and missed everything so far. In one
   paragraph of six to ten sentences, explain how weeks 1, 2 and 3 connect. Use **at least six** words
   from the key word tables, correctly, and **underline** each one.
2. **Rate yourself again.** Copy your four ratings from the week 2 worksheet (Section A, question 4) for
   these topics, then rate yourself again today, from 1 to 5:

   | Topic | Week 2 | Today |
   |---|---|---|
   | How a page gets from a server to my screen | | |
   | What HTML, CSS and JavaScript each do | | |
   | The difference between frontend and backend | | |
   | What an API is | | |

   In one sentence, say which rating changed most, and what made it change. If none changed, say why.

---

## Submission

Git is taught in week 11. Until then, upload your work to the class submission folder **by the deadline
your tutor gives you**.

- **On paper:** photograph every page, in task order. Name the files
  `assignment-01-<surname>-<firstname>-<n>.jpg`, numbered 1, 2, 3 and so on.
- **On a laptop:** put everything, including the diagram, into **one PDF**, in task order. Most word
  processors can save or download a document as a PDF. Name it `assignment-01-<surname>-<firstname>.pdf`.

Check that your diagram is sharp enough to read every label. Keep your copy: your Task 1 diagram grows
again once the programme reaches APIs, React and your own backend.

## Marking (10 points)

| Criterion | Points | What earns full marks |
|---|---|---|
| Task 1: the diagram | 2 | Every required part, in order; DNS, IP address, ★ and HTTPS in the right places; the app reaching the same backend through the API; labelled arrows with a key |
| Task 1: the steps and ✗ marks | 1 | Steps match the diagram, each with the right part named; three tickets marked in the right places |
| Task 2: the support desk | 2 | Each ticket placed in the right step and on the right side, with sensible advice; ticket 6 explained clearly |
| Task 3: features and API reply | 2 | Features placed correctly, each with a reason; all five API questions answered correctly, with working shown |
| Task 4: the AI's plan | 2 | Every sentence given a verdict and a specific source, with corrections; a well-reasoned choice of the most dangerous mistake that uses a week 3 reason and an SDLC stage |
| Task 5: reflection | 1 | A clear paragraph with six key words used correctly; both sets of ratings, with an honest sentence |

You're marked on your reasoning, not your handwriting, typing or drawing skills, and paper and laptop
work are marked the same way. In Task 5, a low rating scores as
well as a high one.

---

## Sources

- Curriculum document §4 (100L S1, weeks 1–3) and §11 (assessment model)
- The class notes and labs for weeks 1–3
- MDN Web Docs: [An overview of HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Overview) ·
  [HTTP response status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Status) ·
  [Glossary: DNS](https://developer.mozilla.org/en-US/docs/Glossary/DNS) ·
  [Glossary: API](https://developer.mozilla.org/en-US/docs/Glossary/API) ·
  [Working with JSON](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Scripting/JSON)
