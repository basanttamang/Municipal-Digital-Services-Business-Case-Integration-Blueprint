# Municipal Digital Services — Business Case & Integration Blueprint

*A self-initiated systems analysis by Basant Tamang, synthesising three earlier case studies into one integration proposal.*

This project is the "fourth piece" of the portfolio: it doesn't build a new system from scratch. Instead, it looks across the three systems already designed and delivered (Birth Register Migration, Ward Appointment System, Sifaris Digital Letters) and makes the business case for connecting them — with an architecture diagram, a cost-benefit analysis, a phased rollout plan, and a RACI matrix.

> **In simple words:** three finished projects each solved one ward-office problem on its own, but none of them talk to each other. This project proposes connecting them through one shared "Citizen Registry," shows the numbers (pays for itself in about 11 months), and lays out a safe, phased order to build it in.

**New here? Start with the plain-English walkthrough:** [Explained Simply (.md)](docs/00-explained-simply.md) · [Word copy (.docx)](docs/00-explained-simply.docx)

## Deliverables

Every document below is written in **plain Markdown** (`.md`, opens formatted on GitHub) **and** saved as a **Word file** (`.docx`) for easy reading or printing. Diagrams are plain `.png` pictures with editable Mermaid source alongside them.

| # | Deliverable | Read on GitHub | Word copy | Status |
|---|---|---|---|---|
| 0 | **Explained Simply** | [.md](docs/00-explained-simply.md) | [.docx](docs/00-explained-simply.docx) | The whole project in 6 plain-English steps |
| 1 | Full business case | [.md](docs/01-business-case.md) | [.docx](docs/01-business-case.docx) | Executive summary, architecture, cost-benefit, phasing, RACI, risks |
| 2 | Integration architecture (picture) | [.md](diagrams/integration-architecture.md) | [.png](diagrams/integration-architecture.png) · [Mermaid source](diagrams/integration-architecture.mmd.txt) | Done |
| 3 | Cost-benefit model | — | [.csv](analysis/cost-benefit-model.csv) | Open in Excel/Google Sheets |

## How this project relates to the other three

| Project | What it contributes to this business case |
|---|---|
| [Birth Register Migration](https://github.com/basanttamang/birth-register-migration) | Supplies the first clean, de-duplicated citizen data to seed the shared registry (Phase 1) |
| [Ward Appointment System](https://github.com/basanttamang/ward-appointment-system) | First front-line system to connect to the shared registry (Phase 2) |
| [Sifaris Feasibility Study](https://github.com/basanttamang/sifaris-feasibility-study) | Second front-line system to connect, including the bank-facing QR verification step (Phase 3) |

## The headline numbers

| Item | Value |
|---|---|
| One-time build cost | NPR 2,400,000 (48 person-weeks) |
| Annual operating cost | NPR 600,000/year |
| Annual citizen benefit (time saved) | NPR 3,375,000/year |
| Simple payback period | ~11 months |

Full workings: [`analysis/cost-benefit-model.csv`](analysis/cost-benefit-model.csv) and Section 5 of the [business case](docs/01-business-case.md).

## Tools

Mermaid (architecture diagram), spreadsheet software (cost-benefit model), Markdown/pandoc (documents), GitHub (version history).
