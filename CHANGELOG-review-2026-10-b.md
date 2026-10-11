# Change log: second review, comparison table and schematic (October 2026)

- **Date:** 2026-10-11.
- **Instructions:**
  - The second review is preserved unchanged in `review-2026-10-b.md`.
  - The later request to add a comparison table and a study schematic is recorded under "Additions" below.
- **Version revised.** The source behind `York_University__Lassonde__Assignment_Template (2).pdf`. Its text was checked as identical to commit `648e146` before editing. The original draft and the "(1)" PDF were not used.
- **Backups:**
  - `proposal-v2-pre-review2`: the "(2)" version.
  - `proposal-v3-pre-table-figure`: the second-review draft, before the table and figure were added.

## Files

| File | Status |
|---|---|
| `proposal-rebecca.tex` (loaded by `main.tex`) | Revised proposal |
| `pdf/proposal-rebecca.pdf` | Compiled proposal |
| `admissions-plan.tex`, `pdf/admissions-plan.pdf` | Updated ~500-word plan of study, kept separate; no table or figure |
| `figures/study-overview.tex` | Editable TikZ source of Figure 1 |
| `figures/study-overview-standalone.tex`, `figures/study-overview-vector.pdf` | Standalone build and vector output of the figure |
| `references.bib` | 26 entries, all cited, none missing |
| `references-additional.bib` | Verified but uncited sources |
| `related-work-matrix.md` | Evidence matrix, table-design notes, originality test |

## Measured length (Tectonic build, 2026-10-11)

- **Main text: 3,400 words.** This counts everything before the Bibliography heading: title block, status note, headings, Table 1, both captions, all text inside Figure 1, the chapter list and the timeline table.
- **Main-text pages:** 8 (letter paper, 11 pt, 25 mm margins, 1.5 spacing).
- **Bibliography:** 3 pages (pp. 9–11). **Total:** 11 pages.
- **Benchmark:** the formal proposal guidance allows "8–10 pages + bibliography (maximum = 3500 words)" (Dissertation Regulations, rev. May 2016, re-checked 2026-10-11). This discussion draft sits within both limits with a 100-word margin. That guidance governs the later formal proposal, not this draft.
- **Admissions plan:** 508 words of body text (533 with heading), 2 pages. York asks for "approximately 500 words".

## Second review: comments and revisions

| # | Comment | Revision |
|---|---|---|
| 1 | Requirements and purpose | Re-checked the How to Apply page, the Guidelines page, the Dissertation Regulations PDF and the degree-requirements PDF; all unchanged. The draft stays separate from the admissions plan, which was updated. The length is measured and reported above. The table and figure are counted rather than treated as exempt. |
| 2 | Learn from York dissertations | Read: Chalk's methodology (recruitment, interviews, analysis, pp. 46–59), Neville's introduction (pp. 1–3) and his chapter contributions and limitations, and Richards's argument statement (pp. 24–27). Applied without copying: an explicit proposition in §10 (Richards); treating improvisers' conventions as existing practices a system can override in §1 and §5 (Neville); iterative recruitment and reporting of sample gaps in §7 (Chalk). None is a table row; see `related-work-matrix.md`. |
| 3 | Sharpen the contribution | §10 now uses the attribution-versus-recognition proposition in your wording, including the example of a log crediting one person while collaborators treat the material as someone else's, the group's or nobody's. It states the proposition is to investigate, not a finding, and maps it to RQ3 (divergence) and RQ1–2 (mechanisms). |
| 4 | Does the system manufacture ownership? | New paragraph in §5 raises the five questions and uses your scoping and co-design wording. The approval and attribution rules are marked provisional, with a "release to the group" option to test. |
| 5 | Recognition, authority, authorship; RQs; Suchman | §3 gives the three working definitions as sensitising concepts, with examples of credit without influence and influence without credit. The RQs were restructured so each targets one concept (Recognition / Authority / Authorship). §4 works through the amber-pulse episode with Suchman's framework. No theorists were added. |
| 6 | Provisional scale | Adopted three groups of 3–5 adults, four workshops of 90–120 minutes each, with a stated rationale (comparison across compositions; time for norms to form). The text now covers: co-design participants do not join the workshops; one existing ensemble is sought and prior relationships recorded; workshop 1 is manual-only and sets the written group procedure; one arrangement per later workshop, ordered differently per group; carry-over is treated as evidence; procedure changes and facilitator interventions are recorded. All numbers are labelled planning figures. |
| 7 | Episode selection and analysis | Your selection wording is integrated in §8. Interview themes contextualise episodes "without settling what it meant". Discrepant cases revise or limit explanations, with an example. An analytic trail replaces inter-rater agreement, consistent with reflexive analysis. The design journal records researcher influence. Provenance is not treated as true intention. |
| 8 | Make the creative work examinable | Re-checked the research-creation guideline ("must be available (in some form)"). §5 uses your documentation wording and explains how the environment's rules work as testable propositions. Public sharing is optional. Consent is separated into research, examination and public dissemination (§9). |
| 9 | Match bias claims to the system | The text-to-image citation is kept only for the general concern. Added primary language-model evidence: Tao et al. 2024 (cultural values), Naous et al. 2024 (Western-entity bias in multilingual and Arabic models) and Liu et al. 2022 (figurative language). The asset library and interface are named as sources of interpretation. Metaphor, idiom and non-English phrases are addressed. Conclusions are limited to the people studied. |
| 10 | Connect to Rebecca's project | Your wording is integrated in §7. The title was re-verified against the YFile announcement (24 July 2026). No methods, participants, AI component or student role are assumed. |
| 11 | Polish | "Not an AI engineering dissertation" is replaced by a positive Feasibility statement. Manuscript status is now the conventional "under revision following peer review" (bib note: "Manuscript under revision"). CMCT 7000/7200/7005 were verified in the linked degree requirements and the timeline marks offerings as subject to change. Chapters go from 9 to 7. The layout stays clean and unbranded. Bibliography metadata was re-checked; **Caines & Watson's pages are corrected to 243–277** from the article's own footer. **Authorship:** both manuscripts are anonymised for review. The teammate text refers to "the author" in the singular; the BioTerrarium authorship rests on your statement (recorded in bib `x-check`). |

## Additions: comparison table and schematic

- **A. How other papers build tables.**
  - Inspected Zhang et al. arXiv 2507.06000v1 (Appendix C, Tables 1–7; locus/dynamics/granularity of agency).
  - Inspected Rezwana & Maher arXiv 2204.07666 (Fig. 2 COFI; Table 1).
  - Inspected Xu et al. Table 3 (coding dimensions).
  - The published versions of Zhang and Rezwana could not be opened (ACM blocks automated access), so differences from the preprints are unchecked.
  - Notes are in `related-work-matrix.md`, Part A.
- **B. Evidence matrix.** In `related-work-matrix.md`, Part B: eight sources plus three dissertations. Each entry records access level (full text vs abstract only), whether the AI was implemented or only proposed, and section or page support.
- **C. Table 1.**
  - Six studies plus "Proposed study (planned)".
  - Five columns: the review's suggested "Authority/recognition focus" and "Relevant finding" columns are merged into one, to fit legibly.
  - No ticks or rankings. Every row is cited, and Suh et al. is marked "abstract only".
- **D. Originality statement (§2).** Lists what already exists, and places the extension in the combination. **Narrowed:** Xu et al. already code "unacknowledged contributions", so the draft no longer implies that recognition in AI-supported groups is unstudied.
- **E. Figure 1.**
  - TikZ, vector, grayscale-safe. Solid arrows show the creative cycle, dashed arrows the shaping conditions (interface rules, asset library, facilitation, researcher choices), dotted arrows documentation and analysis.
  - It includes the arrangements inset, keeps the creative activity and research-analysis bands separate, and contains no outcome boxes.
  - The caption marks it as planned and says the system record does not produce recognition.
  - About 45% of a page. Fonts are fixed at 7–8 pt so it renders the same in the proposal and the standalone build.
- **F. Length.** Duplicated prose was removed (e.g. the three-study paragraphs, now in the table; the arrangements paragraph, now in the figure). Fonts, margins and spacing were not reduced.
- **G. Inspection.** All 11 pages were rendered and checked: no undefined citations, no overfull lines, no clipped figure text. The only warning is one cosmetic underfull line in a bibliography URL. The main text ends cleanly on page 8.

## Unresolved, for discussion with Rebecca

1. Whether *Interfacing, Playtesting, Resetting* could host or sit alongside this study, and on what terms (data, credit, ethics).
2. Whether the provisional scale (three groups × four workshops) suits her experience of community improvisation workshops, and what honoraria are customary.
3. Whether contributor approval and visible attribution clash with improvisers' existing conventions. Scoping will test this, but her view matters first.
4. Primary framework: Suchman alone, or a stronger role for improvisation studies.
5. Major and minor fields, and possible committee members.
6. York's research ethics position on hosted AI services versus local models.
7. Caines "Fragile Devices" year: 2020 (catalogue) or 2021 (her citation).
8. Exact manuscript status wording and co-authorship (to confirm yourself before sending).
