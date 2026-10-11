# Change log: October 2026 review of the exploratory proposal

- **Date:** 2026-10-11
- **Files changed:**
  - `proposal-rebecca.tex` (proposal)
  - `main.tex` (now a one-line wrapper that loads the proposal)
  - `admissions-plan.tex` (500-word plan of study)
  - `references.bib` (now contains only cited references)
  - `references-additional.bib` (new: verified references that are no longer cited)
  - `review-2026-10.md` (new: the review, unchanged)
- **Backup:** Git tag `proposal-v1-pre-review` (commit `6ddcfad`) preserves the earlier proposal and plan. The original York template is in commit `9fae32e`.

## Layout

- **Layout source.** York and the program publish no Communication & Culture proposal template. The layout follows the York thesis template you supplied: letter paper, 11 pt, 25 mm margins, one-and-a-half spacing, no paragraph indent, Times-style text. The Lassonde/York logo was removed, and there is no institutional branding.
- **Deviations from that template:**
  - **Citation style:** author–year (`natbib` + `plainnat`) instead of numeric `ieeetr`. The program's dissertation regulations allow "any accepted citation form", and author–year is the norm in communication and cultural studies. To switch back, change `\bibliographystyle{plainnat}` to `{ieeetr}` and drop `round,authoryear` from the natbib options.
  - **Paragraph spacing:** a 6 pt paragraph skip, because the template removes paragraph indents.
  - **Title block:** the template's thesis title page is replaced by a proposal title block.
- **Compile target.** `main.tex` now only `\input`s `proposal-rebecca.tex`, so Overleaf's Recompile shows the proposal with no settings change.

## Review comments and what changed

| # | Comment | Revision made |
|---|---|---|
| 1 | Clarify which document; remove the Lassonde logo; shorten the status note | The status note now uses the exact wording you gave. The logo and header are removed, and the layout is plain. The separate ~500-word admissions plan is revised (495 words of body text), and its file header records York's instruction. The proposal's timeline names the later formal proposal (maximum 3,500 words, prepared with the supervisory committee) as a distinct Year-2 stage. The access qualifications stay in the case-study section (§8). |
| 2 | Make the cultural stakes explicit | §1 now carries the cultural question about whose interpretations gain authority, and presents it explicitly as "a possibility to investigate, not an established effect". |
| 3 | Narrow and substantiate the gap | The broad claims ("mostly models dyads", "contestability concerns decisions about people") are removed. §2 opens with the suggested framing of the intersection, then compares three studies by participants, setting, method and finding, and states the specific question each leaves open: **Xu et al. 2026** (full text read), **Trajkova et al. 2024** (full text read) and **Epstein et al. 2020** (full text read, via PubMed Central). The contestability sentence is narrowed to what Lyons et al. 2021 actually covers: high-stakes algorithmic decisions such as hiring and sentencing. |
| 4 | Broaden participation; define authorship | §3 uses your participation wording. Authorship is defined as felt ownership, public attribution and creative responsibility; legal ownership and copyright are explicitly excluded. RQ3 now names the same three dimensions. |
| 5 | Repair the comparisons | A table specifies who proposes and who approves in each arrangement. In the human-mediated arrangement, another participant in a rotating "interpreter" role transforms the material using the same asset library, and **the contributor approves**, the same rule as contributor-led. The "separates human from model" claim is replaced by your situated-comparison wording, and the text names the other differences (timing, social relationships, expectations). |
| 6 | Explain how analysis produces knowledge | §9 now sets out a concrete procedure: multimodal episode accounts; comparison of accepted, contested and refused transformations and of disputed authorship; interviews that can challenge my reading; and comparison across sessions. Theory "tells me where to look" but does not decide findings (§4). Records are explicitly not a "true" account of intention. |
| 7 | Strengthen the research-creation component | §6 states that the creative component is the environment plus the improvised works, says what participants make (short collective audiovisual improvisations, built and performed together, then discussed), and gives one illustrative session. |
| 8 | Reframe why AI is used | §7 uses your rationale wording. "Explanation" is replaced by **generated interpretation**, with a sentence saying it cannot establish why the model produced a transformation. Engineering detail is reduced to one short Feasibility paragraph, and the command-pattern and clamping vocabulary is removed. |
| 9 | Correct the withdrawal promise; test non-AI participation | §10 uses your withdrawal wording. Non-AI participation is now "a design commitment that the workshops will test", with named provisions: reduced motion, readable and resizable text, alternatives to sound-only information, facilitator-operated controls, and the manual path. |
| 10 | Sharpen the contribution | §11 uses your contribution wording, and the "AI may be unnecessary" point is reframed as explaining when, how and why, and what that reveals about collective creativity. |
| 11 | Preparation and the connection to Rebecca | **Checked against your teammate manuscript:** participants' requests for opt-in sharing, an immediate off switch and separate icon and number permissions are reported findings (§4.8.5; also §3.9.6 and §5.4). **The "evaluative categories" point is labelled as my reflection as the designer**, because the manuscript's Table 2 labels states such as "possible physiological strain"; the manuscript itself does not report this as a finding. The proposal adds one sentence linking architecture, landscape architecture, HCI and building systems independently. §14 states your extension of her work (contribution-level recognition and contested authorship in repeated group improvisation), and §8 says her funded project's public record does not establish any AI component or this study. |

## Language and tone pass (your second instruction)

- **What changed:**
  - Paragraphs were rewritten for flow and plain wording.
  - The comparison bullets became connected paragraphs.
  - Repetitive bold labels were reduced.
  - Generic openers were removed.
  - Sentence length is more varied.
- **What did not change:**
  - The research questions (word for word).
  - The arguments, methods, arrangements and the AI setup.
  - The citations and their placement, and all numbers and factual details.
  - The sentences the review prescribed, which keep their substance and nearly all their wording.
- **The admissions plan** was revised for comment 1 but did not get a separate tone pass. I can apply one.

## Sources: what was verified, and how

| Claim in proposal | Source | Access |
|---|---|---|
| Xu et al.: 6 × 3 students, one 45-minute session, shared ChatGPT, 9 interviews; AI as anchor, memory, negotiable part of decisions; analysis emphasised information flow over trust and accountability | Xu et al. 2026, CHI | Full text (Newcastle eprints, CC BY): §3.1–3.2, §4, §7 |
| Trajkova et al.: focus groups with 24 dance students; partnered improvisation; designing an AI partner | Trajkova et al. 2024, CHI | Full text (NSF PAR): abstract, §4.1, §7 |
| Epstein et al.: vignette experiments; agent vs tool framing shifts credit and responsibility | Epstein et al. 2020, iScience | Full text (PubMed Central) |
| Contestability developed for high-stakes decisions (hiring, sentencing) | Lyons et al. 2021 | Full text (arXiv): abstract and introduction |
| Text-to-image stereotypes persist even without demographic terms | Bianchi et al. 2023 | arXiv abstract |
| Participation is not automatically empowering (risk of co-optation) | Birhane et al. 2022 | arXiv abstract |
| Consent: specific, revisable / ongoing | Im et al. 2021; Strengers et al. 2021 | Abstracts only (Semantic Scholar). Claims kept at abstract level. |
| Reflexive thematic analysis | Braun & Clarke 2019 | Abstract |
| Microethnography of interface episodes | McArthur 2015 | Full-text sections read (§4.2) |
| "Research-from-creation" | Chapman & Sawchuk 2012 | **Not read directly.** Wording is checked against Papagiannis's (2014) quotation of the article and against search records of the four modes. |
| Suchman's framing | Suchman 2007 | **Book not accessible.** Claim limited to the publisher's description ("how agencies are currently figured at the human-machine interface", "how humans and machines are enacted as similar or different in practice"), as reproduced on the EMCA wiki. The three analytical questions are presented as my questions, informed by Suchman, not as her named concepts. |
| Improvisation as research method (risk, active listening, collaborative response) | Caines 2020 | **Chapter not read.** Based on its description quoted in a 2020 review of the handbook (Research Catalogue). Paraphrased, not quoted. |
| Caines 2026: research-creation, GenAI, ethics, access, collaboration, improvisatory skills | Caines 2026 | Full text read |
| Caines & Watson 2023: "socially responsive creative technologies" | Caines & Watson 2023 | Title and abstract |
| SSHRC project title and funding; no other details public | YFile, 2026-07-24 | Read |
| Research-creation: creative work plus 150–200-page manuscript | ComCult PhD Research-Creation (April 2021) | Re-checked 2026-10-11; file unchanged |
| Formal proposal max 3,500 words | Dissertation Regulations (May 2016) | Re-checked 2026-10-11; file unchanged |
| Admissions plan instructions | How to Apply page | Re-checked 2026-10-11; text unchanged |

**Removed from the proposal** (citations without enough accessible support for the claim made): Fischlin et al. 2013, Woolgar 1990, Sawyer & DeZutter 2009, Jordan & Henderson 1995, Barrett et al. 2019, Stark & Hoey 2021, Horvitz 1999, Guzdial et al. 2019, Rezwana & Maher 2023, Zhang et al. 2025, Mathewson & Mirowski 2017, Mirowski et al. 2023, Draxler et al. 2024, Hirsch et al. 2017, Loveless 2019, Khaled et al. 2018. They are kept in `references-additional.bib` for later chapters.

## Unresolved (worded so the proposal does not depend on them)

1. **Year of Caines's "Fragile Devices" chapter.** The British Library catalogue and a 2020 review give 2020; Caines (2026) cites 2021. The proposal uses 2020. Confirm on the Bloomsbury page.
2. **Whether *Interfacing, Playtesting, Resetting* could host the study.** Unknown. The proposal says only the title and funding are public and leaves it to Rebecca.
3. **The exact status of both manuscripts.** The wording used is "submitted to ACM venues and received revision requests; neither has been accepted." Your portfolio describes the SIGGRAPH paper as "not accepted" and the teammate paper as "in revision for 2027". Confirm before sending.
4. **BioTerrarium results.** Its results are not cited, because the January and July versions disagree on whether the study was run (see `research-notes.md` §4.3).
5. **Length.** The revised proposal is about 2,600 words of prose (excluding the chapter list, timeline and bibliography), above the earlier ~2,000 working length, because the review asked for the comparison studies, definitions, a session example and an analysis procedure. If Rebecca prefers something shorter, the three-study comparison and the ethics section are the easiest to condense.
6. **The review copy.** `review-2026-10.md` was transcribed from your message. If you have the original file, compare it once.

## Compilation

- **Tool:** Tectonic 0.17.0 (XeTeX engine) in a scratch folder. Overleaf is set to LuaLaTeX; the files are written for pdfLaTeX, XeLaTeX and LuaLaTeX.
- **`main.tex` (proposal):** 0 undefined citations, 0 overfull boxes. One underfull line inside the bibliography (cosmetic). Section headings do not fall at page bottoms.
- **`admissions-plan.tex`:** no warnings; 495 words of body text.
- **Fonts:** TeX Gyre Termes (a Times-style font).
- **Submission:** nothing submitted, emailed or pushed as part of this revision.
