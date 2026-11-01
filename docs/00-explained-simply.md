# Municipal Digital Services — Explained Simply

*A plain-language walkthrough of this project, for anyone with no technical background.* Oct 29, 2026

---

## The problem, in one sentence

Three separate projects (birth records, appointment booking, recommendation letters) each solved their own piece of the ward office's work well — but none of them talks to the others, so the same citizen gets re-entered, re-checked, and sometimes re-typed slightly differently, up to three separate times.

## The solution, in one sentence

**Connect the three systems to one shared "Citizen Registry" — so a citizen's verified details are entered once and reused everywhere — and roll that connection out in three small, low-risk phases instead of one big risky one.**

---

## The story, in 6 steps

### Step 1 — Notice the pattern across three finished projects

After finishing three separate projects — cleaning birth records, building an appointment system, and designing a recommendation-letter service — a question worth asking is: *do these need to know about each other?* Each was built well on its own, but none of them currently shares information with the others.

> Like three different departments in the same office each keeping their own paper filing cabinet for the same customer — useful on their own, but nobody notices when two cabinets spell the customer's name differently.

### Step 2 — Work out exactly what goes wrong without a connection

Without a shared record, a citizen has to give their name and details again at every system. Small typos or spelling differences between systems go unnoticed because nothing ever compares them. And a trick used by Project 2 (catching duplicate or fake records) only protects Project 2 — it isn't reused by the other two.

> Like discovering that a fraud-check trick your accounting department invented is never shared with the sales department, who re-invent weaker version of it — or skip it entirely.

### Step 3 — Design one shared record instead of three separate ones

The proposal is a single "Citizen Registry" in the middle. The birth-register project feeds it the first clean batch of records. The appointment system and the letter system both check this same registry instead of keeping their own private lists.

> Like replacing three separate filing cabinets with one shared filing cabinet that every department is trained to check first before creating a new folder.

### Step 4 — Put real numbers on the idea, not just a diagram

A good idea on paper is not yet a business case. The costs (about NPR 2,400,000 to build, NPR 600,000/year to run) are weighed against the benefit (citizens avoiding roughly 30,000 unnecessary return trips a year, worth about NPR 3,375,000/year in time saved) to work out that the idea pays for itself in about 11 months.

> Like pricing out a home renovation against how much it will actually save on the electricity bill, instead of just assuming "it'll probably help."

### Step 5 — Plan a safe order to build it in, not one big risky release

Rather than connecting all three systems at once, the plan breaks the work into three phases: first just build the shared registry quietly (lowest risk), then connect the appointment system (medium risk, citizen-facing), then connect the letter system last, because it involves banks and carries more legal weight.

> Like learning to swim in the shallow end first, then the regular pool, before ever attempting open water — each step only happens once the previous one is proven safe.

### Step 6 — Write down who is responsible for what

A RACI table spells out, for each piece of work, who decides, who does the work, who is consulted, and who just needs to be kept informed — covering ward management, the analyst, the developers, IT, and even the banks who will rely on the final letter-verification step.

> Like a wedding seating chart — written down in advance so nobody is confused on the day about who does what.

---

## The one-breath answer for an interview

> "After finishing three separate ward-office projects, I noticed none of them shared citizen information with each other, so I wrote a business case for connecting them through one shared registry. I costed it, found it pays for itself in about 11 months, and — instead of proposing one big risky rollout — sequenced it into three phases so the ward office sees a working improvement within weeks, not a year."

---

## Where each step lives in the project files

| Step | File |
| --- | --- |
| 3. Architecture | `diagrams/integration-architecture.md` (picture) · `diagrams/integration-architecture.mmd.txt` (editable source) |
| 4. Cost-benefit numbers | `analysis/cost-benefit-model.csv` |
| 4–6. Full business case, phasing, RACI, risks | `docs/01-business-case.md` |
