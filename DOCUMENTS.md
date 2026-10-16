# Documents: what each one is and where it is

All paths are relative to this folder (`Desktop/CV/Proposal`). Edit the `.tex` source; the `.pdf` files in `pdf/` are the compiled copies. Limits were checked against York's pages on 2026-10-13 (see `research-notes.md`, "Requirements re-check").

| # | Document | For whom / when | Source | PDF | Length | Limit |
|---|---|---|---|---|---|---|
| A | **Plan of Research: AI-Mediated Communication in Collective Creative Practice** (York's "Proposed Plan of Study") | Upload with the York application (priority deadline 15 Jan 2027) | `admissions-plan.tex` | `pdf/admissions-plan.pdf` | 498 words including title block and Table 1, 1 page | "approximately 500 words" (York How to Apply) |
| B | **Exploratory research proposal** | Send to Dr. Rebecca Caines before applying; not an application document | `proposal-rebecca.tex` (compiled via `main.tex`) | `pdf/proposal-rebecca.pdf` | 3,457 words including table and figure, 8 pages + bibliography | none set; kept under the formal-proposal ceiling |
| C | **Formal dissertation proposal (advance draft)** | Only after admission, within five months of passing the Qualifying Examination, with the program's ethics form | `formal-proposal-draft.tex` + `formal-proposal-bibliography.tex` | `pdf/formal-proposal-draft.pdf` | 3,274 words, 8 pages + bibliography | "8 - 10 pages + bibliography (maximum = 3500 words)" (Dissertation Regulations, rev. May 2016) |

## Notes

- **Ready to email:** `send-to-rebecca/` holds renamed copies (`Roman_Jahandideh_PhD_Research_Proposal.pdf`, `Roman_Jahandideh_PhD_Plan_of_Research.pdf`, `Roman_Jahandideh_Academic_CV.pdf`). It is excluded from git because the repository is public and the CV contains contact details. If you edit a document, recopy it there.

- **A is the only one of these required for the application.** The application also needs a single-authored writing sample (12–20 pages), a CV, transcripts and three academic references. Those are not in this folder.
- **C follows York's required order:** Title, Introduction, Objectives, Methods and Sources (including anticipated problems of access), Relationship to existing literature and practice, Proposed chapter outline, Proposed timeline, and a Select Bibliography split into theoretical/methodological works and substantive works. It also has a short non-technical summary. Supervisor and committee are left as "[to be confirmed]". Do not fill them in until they are agreed. It is set in 12 pt with 1.5 spacing so the page count fits the 8–10 page range; A and B stay at 11 pt.
- **C's bibliography** (`formal-proposal-bibliography.tex`) is generated from `references.bib`. If a reference changes, ask for it to be regenerated rather than editing it by hand.
- **Overleaf:** the default compile target is `main.tex`, which is document B. To compile A or C in Overleaf, open that file and choose it as the main document from the Menu.
- **Supporting records:** `references.bib`, `related-work-matrix.md`, `discussion-notes.md`, `research-notes.md`, the review records (`review-2026-10*.md`) and the change logs (`CHANGELOG-review-2026-10*.md`).
