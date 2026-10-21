# Build and word-count report (updated 2026-10-21)

## Root files and outputs

| Doc | Root `.tex` | Includes | PDF |
|---|---|---|---|
| A, plan of study | `admissions-plan.tex` | none | `pdf/Roman_Jahandideh_PhD_Plan_of_Research.pdf` |
| B, proposal for Dr. Caines | `main.tex` → `proposal-rebecca.tex` | `sections/*.tex` (incl. `relatedwork.tex`), `figures/study-overview.tex`, `references.bib` | `pdf/Roman_Jahandideh_PhD_Research_Proposal.pdf` |
| C, formal proposal (advance draft) | `formal-proposal-draft.tex` | `sections/*.tex` (not `relatedwork.tex`), figure, `formal-proposal-bibliography.tex` | `pdf/Roman_Jahandideh_Formal_Dissertation_Proposal_DRAFT.pdf` |

## Build

- **Engine:** Tectonic 0.17 (XeTeX engine), the same as earlier builds. For example, `tectonic -X compile main.tex`. Overleaf compiles `main.tex` (document B) by default; for A or C, set the main document in the Overleaf menu.
- **BibTeX:** B uses BibTeX with plainnat. C's two-part Select Bibliography is a generated static file, so no BibTeX run is needed. After any change to `references.bib`, it must be regenerated (the generator script is in the session scratchpad).
- **Result:** all three compile with **0 undefined citations or references**.
- **Remaining warnings:** one cosmetic underfull line in B's bibliography (a long URL). No overfull boxes.
- **Inspection:** every rendered page that changed was inspected as an image: table, figure, timeline and page breaks.

## Word counts

- **Method 1, TeXcount 3.1.1** (`texcount -inc -total -sum`): table cells count as text, and citations are not counted.
- **Method 2, PDF extraction:** body prose from the Summary heading to the bibliography. It includes headings, rendered citations and captions, and excludes the title block, table, figure text, page numbers and bibliography.

| Doc | TeXcount sum | PDF body prose | Table | Figure text | Title block | Pages | Limit |
|---|---|---|---|---|---|---|---|
| A | 493 | 460 (494 incl. heading block) | none | none | 34 | 1 | approximately 500 |
| B | 3,294 | **3,419** | 194 | 108 | 58 | 8 + bibliography (pp. 9–13) | ≤ 3,500 (self-imposed, matching C) |
| C | 3,283 | **3,397** | none | 108 | 46 | main text to p. 10; bibliography pp. 10–14 | 8–10 pages + bibliography, max 3,500 words |

- The bibliography is outside the 3,500-word maximum. The Regulations state "8 - 10 pages + bibliography (maximum = 3500 words)".
- C is set in 12 pt with 1.5 spacing, as before; A and B are in 11 pt.

## Deliberate differences between B and C

- **C:** follows York's required section order; has a dated timeline and a Sources subsection; has no related-work table (its comparison is in prose in §4); and has a split Select Bibliography.
- **B:** has the table (§5) and a year-level timeline.

## TODOs and decisions still open

1. **Venue:** the Markham Art Gallery is proposed, not confirmed. This needs Dr. Caines and the gallery.
2. **Participant community and recruitment channels:** confirm with Dr. Caines (AMPD networks, York Region arts groups).
3. **Rebecca's case studies:** integration with her SSHRC project or other case studies, to be decided later with her.
4. **Fragile Devices:** read the chapter in full when library access allows; it is currently cited through Caines & Watson's summary.
5. **Bishop, Becker, Crawford:** check the paraphrases against the books.
6. **ISS DOI:** the DOI should resolve after November 2026; the "Romman" spelling on the ACM proof needs correcting.
7. **Repository visibility:** the GitHub repository is public; consider making it private.
