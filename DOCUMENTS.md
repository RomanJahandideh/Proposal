# Documents: what each one is and where it is

All paths are relative to this folder (`Desktop/CV/Proposal`). Edit the `.tex` source; the `.pdf` files in `pdf/` are the compiled copies. Limits were checked against York's pages on 2026-10-13 (see `research-notes.md`, "Requirements re-check").

| # | Document | For whom / when | Source | PDF | Length | Limit |
|---|---|---|---|---|---|---|
| A | **Plan of Research: AI-Mediated Communication in Collective Creative Practice** (York's "Proposed Plan of Study") | Upload with the York application (priority deadline 15 Jan 2027) | `admissions-plan.tex` | `pdf/Roman_Jahandideh_PhD_Plan_of_Research.pdf` | 494 words including heading block (460 body), 1 page, no table | "approximately 500 words" (York How to Apply) |
| B | **Exploratory research proposal** | Send to Dr. Rebecca Caines before applying; not an application document | `proposal-rebecca.tex` (compiled via `main.tex`) | `pdf/Roman_Jahandideh_PhD_Research_Proposal.pdf` | 3,419 words body prose (TeXcount 3,294), 8 pages + bibliography | none set; kept under the formal-proposal ceiling |
| C | **Formal dissertation proposal (advance draft)** | Only after admission, within five months of passing the Qualifying Examination, with the program's ethics form | `formal-proposal-draft.tex` + `formal-proposal-bibliography.tex` | `pdf/Roman_Jahandideh_Formal_Dissertation_Proposal_DRAFT.pdf` | 3,397 words body prose (TeXcount 3,283), main text to p. 10 + bibliography | "8 - 10 pages + bibliography (maximum = 3500 words)" (Dissertation Regulations, rev. May 2016) |

## Notes

- **Ready to email:** the PDFs in `pdf/` are named for sending: `Roman_Jahandideh_PhD_Plan_of_Research.pdf` and `Roman_Jahandideh_PhD_Research_Proposal.pdf`. Attach the CV from `Downloads/Roman_Jahandideh_Academic_CV.pdf` (kept out of this public repository because it contains contact details). The formal draft is not for sending yet.

- **A is the only one of these required for the application.** The application also needs a single-authored writing sample (12–20 pages), a CV, transcripts and three academic references. Those are not in this folder.
- **C follows York's required order:** Title, Introduction, Objectives, Methods and Sources (including anticipated problems of access), Relationship to existing literature and practice, Proposed chapter outline, Proposed timeline, and a Select Bibliography split into theoretical/methodological works and substantive works. It also has a short non-technical summary. Supervisor and committee are left as "[to be confirmed]". Do not fill them in until they are agreed. It is set in 12 pt with 1.5 spacing so the page count fits the 8–10 page range; A and B stay at 11 pt.
- **C's bibliography** (`formal-proposal-bibliography.tex`) is generated from `references.bib`. If a reference changes, ask for it to be regenerated rather than editing it by hand.
- **Overleaf:** the default compile target is `main.tex`, which is document B. To compile A or C in Overleaf, open that file and choose it as the main document from the Menu.
- **2026-10-20 redevelopment:** B and C share their text through `sections/*.tex`; see `revision_audit.md`, `source_verification.md` and `build_and_wordcount_report.md`. The 2026-10-21 revision (MA continuity, case-study architecture) is recorded in `change_memo_2026-10-21.md` and `decision_list.md`.
- **Supporting records:** `references.bib`, `related-work-matrix.md`, `discussion-notes.md`, `research-notes.md`, the review records (`review-2026-10*.md`) and the change logs (`CHANGELOG-review-2026-10*.md`).
