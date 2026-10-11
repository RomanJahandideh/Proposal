# Research notes: PhD proposal, York Communication & Culture (Fall 2027)

Prepared 2026-10-11 for Roman Jahandideh. Prospective supervisor: Dr. Rebecca Caines.

Each claim carries one of these labels:

- **[V] Verified.** Read in the source named, on 2026-10-11.
- **[I] Interpretation.** My reading of verified material.
- **[P] Proposal choice.** A design or research decision, open to change.
- **[?] Unresolved.** Needs checking, or needs Rebecca's or your confirmation.

Companion files: `yorkspace-inventory.md` (full repository inventory), `references.bib`, `proposal-rebecca.tex`, `admissions-plan.tex`, `discussion-notes.md`.

---

## 0. Workspace inspection

- [V] The repository has one commit ("Initial Overleaf Import"). Its remote is `origin = https://github.com/RomanJahandideh/Proposal.git`. I did not push, pull or change any remote setting. I could not verify whether Overleaf is synced to that GitHub repository, and nothing written here has reached Overleaf until you push or sync it yourself.
- [V] There are no README or repository instruction files.
- [V] `main.tex` is an unmodified York-branded *assignment* template: `article`, 10pt, A4, `geometry`, `fancyhdr` with `yl.png` in the header, `y.png` on the title page. It loads `unicode-math`, so it needs XeLaTeX or LuaLaTeX. There is no `.bib` file and no citation convention. `Program Solution.py` prints "Hello World!".
- [P] The new `.tex` files are standalone. They keep the template's page geometry, header logo and `\baselinestretch{1.25}`, but drop `unicode-math`, so they compile with pdfLaTeX, XeLaTeX or LuaLaTeX. Citations use `natbib` with author–year citations and the `plainnat` bibliography style, which prints DOIs and URLs. The program's dissertation regulations say "any accepted citation form may be used", so there is no mandated style. `main.tex` was not changed.
- [V] No LaTeX was installed locally. I test-compiled with Tectonic 0.17.0, downloaded only into the session scratch folder (see §9).
- [V] CV sources: `Desktop/CV/teacher assistant/Roman_Jahandideh.pdf` and `.../Environment Tech artist/...pdf` (both March 2026). They confirm:
  - B.Arch, Tabriz Islamic Art University, 2011–2016. One CV says "Tabriz Art University".
  - MLA, Istanbul Technical University, 2020–2024.
  - SFU master's, 2025–present.
  - TA for IAT 343 Animation and IAT 313 Narrative & New Media.
  - Virtual Landscape Lab, ITU, 2021–2024.
  - Senate Graduate Studies Committee member, SFU.
- [?] The CVs say "Master of Interactive Arts and Technology". You describe the degree as a thesis-based "MA". Use SFU's official degree name.
- [?] The CVs do not mention iViz Lab, Steve DiPaola, C#, multiplayer networking or TCPS 2: CORE. I take these from you. The manuscripts and GitHub repositories corroborate Unity, C# and multiplayer work.
- [V] Your portfolio (romanjahandideh.com) says BioTerrarium was "submitted to ACM SIGGRAPH 2026 (not accepted)" and the teammate paper is "in revision for 2027 ACM resubmission".
- [?] That is not the same as "received revision requests". The documents use neutral wording: "submitted; revisions requested; not accepted". Please confirm the exact status of each.
- [V] Your public GitHub repositories include:
  - `teammate-experiment-unity`: Unity multiplayer prototype (C#).
  - `embedding-physiological-environments` (C#).
  - `HR-HRV-experiment-design-and-data-collection-system`.
  - `environmental-massing-agents`: Python, Claude agents over an MCP server.
  - `parametric-massing-generator`.
  - [I] These show hands-on experience calling LLM APIs with structured tool use. I describe this as applied tool-building, not machine-learning research.

---

## 1. Official program requirements (Stage 1)

### 1.1 Sources read (all accessed 2026-10-11)

| Source | URL | What I took from it |
|---|---|---|
| Program home | https://www.yorku.ca/gradstudies/cmct/ | Joint York/TMU program; MA and PhD; three areas: Media & Culture; Politics & Policy; Technology in Practice: Applied Perspectives. |
| How to Apply | https://www.yorku.ca/gradstudies/cmct/future-students/how-to-apply/ | Documents, plan-of-study wording, deadlines (quoted below). |
| Future Students (York Admissions) | https://futurestudents.yorku.ca/graduate/programs/communication-and-culture | Minimum GPA B+; IELTS 7.5; TOEFL iBT 100 for tests before January 2026, or the new-scale score of 5 from January 2026; 18 terms; components are qualifying exams plus dissertation. |
| Guidelines, Policies & Forms | https://www.yorku.ca/gradstudies/cmct/current-students/guidelines-policies-forms/ | Links to the PDFs below. |
| PhD Degree Requirements (2014, updated) | linked PDF | Requirements listed below. |
| PhD Timeline to Completion (2017, updated) | linked PDF | Typical full-time schedule (below). |
| Dissertation Regulations (rev. May 2016) | linked PDF | Formal proposal rules (below). |
| PhD Qualifying Exam Regulations (Dec 2022) | linked PDF | Exam structure (below). |
| PhD Research-Creation Dissertation (April 2021) | linked PDF; also https://www.torontomu.ca/graduate/programs/comcult/forms-resources/research-creation/ | Quoted below. |
| Courses | https://www.yorku.ca/gradstudies/cmct/current-students/courses/ | Lists 7000, 7200 and electives such as 6504 *Social and Cultural Implications of New Media*, 6537 *Digital Games and Learning*, 6539 *Technological Mediations in Visual Culture*. |
| Our Faculty | https://www.yorku.ca/gradstudies/cmct/about-us/our-faculty/ | Caines listed (below). |

**PhD Degree Requirements PDF:**
- 18 credits: CMCT 7000 Perspectives; 7200 Advanced Research Methods Workshop; 7005 PhD Field Seminar; two electives in the major area; one elective in the minor area.
- A "constructed minor" is possible with the director's approval.
- MA core courses 6004 and 6002 may be required for students "lacking background".

**PhD Timeline PDF (typical full-time path):**
- Year 1: courses.
- Fall of Year 2: comprehensive exams.
- Winter of Year 2: proposal preparation and submission.
- Completion is expected by the end of Year 4. The maximum is 18 terms.

**Qualifying Exam Regulations:**
- Three parts: Major General, Major Specific, Minor.
- Normally a take-home exam with answers of about 3,500–4,000 words each.
- One oral defence.

### 1.2 Three different documents

**A. Admissions "Proposed Plan of Study"**

- [V] Length is "approximately 500 words".
- [V] Exact instruction: *"The applicant should provide a clear and detailed description of the planned research area by including the objects of study, potential methods, and the compatibility of their scholarly interests with the program. Applicants should also discuss their preparation for doctoral study in the program especially if previous academic background (in terms of degrees, courses, previous research, etc.) appears distant from the central scholarly areas of communication and culture. Additionally, applicants may highlight any accomplishments relevant to admission into the program."*
- [V] Other documents: CV; a single-authored scholarly writing sample of 12–20 pages; transcripts; three academic references (at most one professional).
- [V] A confirmed supervisor is not required, but "you should have an idea of the faculty members whose expertise aligns".
- [V] Program page: applications open 2026-09-30; priority deadline 2027-01-15; final deadline 2027-03-15. York Admissions lists 2027-01-15 for fall entry.
- [?] Confirm with the program which deadline applies to you. Aim for 15 January.
- [I] The writing sample must be single-authored. Both manuscripts are anonymised for review, and the eCAADe paper has three authors. Check with the program whether a manuscript you wrote alone qualifies, or adapt a single-authored chapter of your MA thesis.

**B. Exploratory proposal for Rebecca**

- [P] This is our own working document, about 1,500–2,000 words. The program sets no rules for it.
- [P] Its purpose is to answer Rebecca's request: methods, outputs and explicit program fit.

**C. Formal dissertation proposal (after admission and comps)**

- [V] From the Dissertation Regulations PDF: submit within **five months** of passing the Qualifying Examination.
- [V] It must contain "a brief statement in non-technical language on the purpose of the research, its relationship to existing work in the area, and the contribution that the researcher hopes to make…", plus title, supervisor and committee.
- [V] "The maximum length of a proposal is 3,500 words." The program-specific section says "Length: 8 - 10 pages + bibliography (maximum = 3500 words)".
- [V] Required format:
  - Title.
  - Introduction.
  - Objectives: problem or question; theoretical perspective; expected contribution ("the originality of the work must be demonstrated").
  - Methods and Sources, including "anticipated problems of access (to research subjects, archives, media content, etc.) and how they will be dealt with".
  - Relationship to existing literature or professional practice.
  - Chapter outline.
  - Timeline.
  - Select bibliography.
- [V] An ethics form must be submitted with the proposal.
- [V] Doctoral proposals must be approved at least six months before the oral exam.
- [V] The supervisory committee has at least three members: the supervisor, at least one other program member, and optionally one from outside the program.
- [?] The Qualifying Exam Regulations (Dec 2022) say the proposal is "normally due **four** months after" comps. The Dissertation Regulations say **five**. Confirm which applies.
- [I] **This 3,500-word limit applies to document C only. It does not apply to the admissions statement (A) or the exploratory proposal (B).** The section structure of proposal B anticipates document C so it can be reused later.

### 1.3 Research-creation: verified wording

- [V] ComCult "adheres closely" to SSHRC's definition: *"…a process that is situated within the research activity and produces critically informed work in a variety of media (art forms); a work that is not simply an interpretation or analysis of a creator's work, **not a conventional work of technological development**, or work that focuses on the creation of curricula…"*
- [V] *"A research-creation dissertation is comprised of both a creative work and a written manuscript (150-200 pages) that demonstrates how the work is implicated in and contributes to the exploration of a set of conceptual and theoretical concerns raised by the written component… The PhD Research-Creation option does not permit students to complete an artistic project in lieu of written PhD dissertation. The creative work must be available (in some form) so that the examining committee may assess its contribution."*
- [V] *"…all academic requirements, supervisory arrangements, milestones, and evaluation criteria for the research-creation option are the same as those for the manuscript-only PhD."*
- [V] *"It is assumed that students electing the research-creation option possess the practice-based skills required to complete their project at the time of admission. ComCult is not a studio-based program…"*
- [V] Technological prototypes are explicitly listed among eligible modes. Methods "which are participatory, consultative, and/or inclusive" are named as typical.
- [I] **Implication.** The Unity system cannot be the contribution in itself, because a "conventional work of technological development" is excluded. The creative work has to be the means by which a communication-and-culture question is investigated, and the 150–200-page manuscript has to carry the argument.

### 1.4 Program orientation, streams, faculty

- [V] Mission: "the application of critical theory and research to contemporary issues and practices in communication and culture".
- [V] York Admissions lists "critical analysis of technology" among the research areas.
- [V] Caines's faculty entry, verbatim: *"Media & Culture; Technology in Practice | AMPD (York University) | Accessibility; Communication, community and creativity; Creative, ICT and cultural industries; Digital humanities; Digital life; Media arts; Music studies; New media; Philosophy of technology; Youth, children and media culture; Performance studies"*.
- [V] Other listed faculty relevant to a committee (none have been contacted):
  - Game studies: Nick Taylor, Kelly Bergstrom, Alison Harvey (York); Jason Boyd (TMU).
  - Philosophy of technology and STS: Ganaele Langlois.
  - Research-creation: Patricio Davila.
  - Accessibility and inclusive design: Deborah Fels (TMU).
  - David Cecchetto supervised or sat on several relevant committees (YorkSpace metadata and acknowledgements).
- [P] Major area: **Technology in Practice**. Minor area: **Media & Culture**, or a constructed minor in HCI and design research. McArthur (2015) records that she constructed an HCI minor.
- [?] Ask the Graduate Program Director whether a constructed minor in human–computer interaction is still approved.

---

## 2. Completed dissertations (Stage 2)

### 2.1 Inventory

- [V] I harvested all 134 records in the York Communication & Culture collection through the DSpace API: **92 doctoral and 42 master's**. A keyword screen flagged 53 as relevant. See `yorkspace-inventory.md`.
- [V] Excluded as MA theses after checking `dc.degree.level`:
  - Ashizawa, *Best of Both Worlds* (VR, research-creation, 2024).
  - White, *Here Be… Dragons?* (microethnography of character creation, 2026).
  - Hanley, *AI disclosure*.
  - Argyle, *TikTok*.
  - These are useful as method precedents but are not PhD examples.
- [?] TMU-registered graduates may deposit in TMU's repository (RShare). It returned HTTP 403, so the corpus here is York deposits only.
- [V] The "Jennifer Andrews" in your brief is **P. Megan Andrews**, according to the title page and file name.
- [V] Dates: the year in the table below is the title-page date. Repository "issued" dates differ: Papagiannis is May 2014 on the title page and 2015-08-28 in the repository; Richards is November 2025 and 2026-03-10.

### 2.2 What I read

All reading was of full-text PDFs. Page numbers are the dissertation's printed numbers.

| # | Dissertation (year, supervisor) | Sections read | Not read |
|---|---|---|---|
| 1 | McArthur, *Me, Myself, and Interface* (2015, Jenson) | Abstract; ToC; 1.3–1.4 (pp. 10–14); 2.3.1 ANT (pp. 43–46); 4.2 Methodology (microethnography, pp. 126–129); 4.5.3 (pp. 141–143); Conclusion (pp. 246–248) | Chs 3, 5–7 in detail |
| 2 | Chalk, *Producing Play* (2022, Jenson) | Abstract; ToC; Ch 3 Methodology opening, realism, insider-outsider (pp. 46–50); Ch 5 conclusion (pp. 139–140); Ch 6 opening (pp. 141–143) | Ch 4 mapping; most of Ch 5 |
| 3 | Neville, *Machine Listening, Unsettled* (2026, Elmer) | Abstract; ToC; overview of the dissertation (pp. 21–23); Ch 5 Methodology (pp. 179–181); Ch 6 conclusion, chapter contributions, limitations (pp. 204–216) | Chs 2–4 bodies |
| 4 | Richards, *Nothing to See Here* (2025, Fisher) | Abstract; ToC; Introduction "Dissertation Summary" (pp. 24–27); Literature review, Critical AI Studies opening (pp. 47–49) | Parts 1–3 bodies; Conclusion |
| 5 | Andrews, *Somatic Anacrusis* (2016, Bailey) | Abstract; ToC; "Dancing and Writing Alongside Hay" (p. 25); Ch 3 auto-ethnographic and phenomenological strategies, "My Process" (pp. 87–93); Conclusion and summary (pp. 293–294) | Chs 4–6 analysis |
| 6 | Papagiannis, *AR as a New Medium* (2014, Fisher) | Abstract; ToC; Introduction (pp. 1–4, 10–11); Literature review opening (pp. 12–15); Ch 3 Research-creation (pp. 40–46); Ch 4 "Contribution to Knowledge" (pp. 87–88); Epilogue (pp. 202–204) | Ch 4 iterations; Ch 5 "40 Ideas" |
| 7 | A. Miroshnichenko, *Hybrid Multi-modal Game Design* (2020, Jenson) | Abstract; ToC; Introduction (pp. 1–5); Game Experiment #2 opening (pp. 85–88); Conclusion (pp. 101–104) | Chs 2–5 |
| 8 | Mayoral Baños, *Tech Anishinaabe Medicine Wheel* (2021, Crow) | ToC; Introduction (pp. 1–3); 1.3.3 method of "conversations" (pp. 38–40); Conclusion (pp. 292–294) | Most of Parts 2–4 |
| 9 | Borkowski, *Incredible Voices* (2025 PDF, Cecchetto) | ToC; 1.3 method (pp. 18–21); Interlude A (pp. 55–56); Conclusion (pp. 192–195) | Chs 2–4 |
| 10 | Russell, *Flesh & Metal* (2026, Boyd) | Abstract; ToC; Thesis and Questions; Method and Approach (pp. 7–10); Appendix L; Conclusion opening (pp. 158–159) | Chs 1–4 |

### 2.3 Summaries and lessons

Summaries are [V] where they paraphrase the text and [I] for the lessons.

**1. McArthur (2015).**
- *Argument:* character-creation interfaces co-construct avatars with players.
- *Framework:* Actor-Network Theory, affordances, feminist theory.
- *Methods:* an analytical framework (Avatar Affordances Framework) applied to 20 interfaces; two lab studies (n = 39 and n = 24) with video microethnography following Giddings and Kennedy; an autoethnographic chapter; best-practice guidelines.
- *Contribution:* repositions the interface as an actor, and shows self-reports diverging from observed practice. For example, 38% said hair matters to them, but few explored the hair options.
- *Practice and scholarship:* the empirical HCI studies serve a cultural argument about representation.
- *Lessons:* this is the closest precedent for combining HCI methods with a ComCult argument. Microethnography of short interface episodes fits the AI-proposal episodes in my design. Compare self-report with observation, and never treat either as ground truth. She also constructed an HCI minor.

**2. Chalk (2022).**
- *Argument:* Actual Play (improvised tabletop play as media) is a field of cultural production. Most producers cannot make a living from it, and non-economic values (participation, enjoyment, community) sustain their labour.
- *Framework:* political economy, Bourdieu's field theory corrected by ANT, labour theory (playbour; Hesmondhalgh and Baker's "good work").
- *Methods:* 24 semi-structured interviews plus documentary research. Explicit insider-outsider and "aca-fan" reflexivity.
- *Lessons:* improvised collective play is a cultural-production object. Creative labour and credit are communication-and-culture questions. Disclose your own position as a designer and enthusiast. Workshop contributions are labour, so treat compensation and credit seriously.

**3. Neville (2026).**
- *Argument:* "authoritarian diffusion" means technologies imposed without listening.
- *Cases:* health-related machine listening, Crisis Text Line, salvage ethnography. Privacy is reframed as a precondition for listening.
- *Framework:* Mumford's authoritarian technics, diffusion of innovations, Hui's cosmotechnics, two-eyed seeing, Indigenous methods.
- *Methods:* web-history analysis (Wayback Machine), interviews with volunteer counsellors, archival and land-based research-creation (Chapman and Sawchuk's "creation-as-research").
- *Lessons:* AI mediation can be analysed as a governance relation. Who may withdraw, and who listens, are central questions. Neville's Indigenous research-creation rests on his own Métis positionality and kinship relations. **This is a reason for me not to take up Indigenous contexts without such relations.** He is also candid about methodological fragmentation and limits, which is worth imitating.

**4. Richards (2025).**
- *Argument:* "safe" generative models extend a counterinsurgent mode of governance through regulatory, technical and epistemic closures.
- *Framework:* Mirzoeff's visuality; critical political economy; critical AI studies.
- *Methods:* genealogical and discursive analysis. Not empirical with participants.
- *Lessons:* model guardrails and defaults are not neutral. They shape what can be expressed. My project can study this at the micro scale, in what a model will and won't make of participants' material, without adopting his macro framework.

**5. Andrews (2016).**
- *Argument:* Hay's choreography is "a radical communication practice". Coins *somatic anacrusis*.
- *Framework:* Merleau-Ponty's phenomenology, Laban Movement Analysis, Irigaray.
- *Methods:* three months of daily practice, journals, two performances, an "emergent choreographic analysis" written from inside the practice, with an explicit section on scope and boundaries.
- *Lessons:* improvisation and embodied practice are legitimate ComCult objects. Documenting one's own practice needs a disciplined protocol (daily notes, explicit limits on claims). A "constructed situation" or score is a useful frame for designing workshop scores.

**6. Papagiannis (2014).**
- *Argument:* AR is an emerging medium moving from "overlay" to "entryway".
- *Framework:* remediation (Bolter and Grusin), McLuhan, Manovich.
- *Methods:* research-creation (an iPad AR pop-up book, two iterations) using Chapman and Sawchuk's four modes. She places her work in "research-for-creation" rather than "research-from-creation". Also a speculative "40 Ideas" framework.
- *Lessons:* a clear precedent for the four modes. Her claims of novelty ("world's first") and her future-oriented enthusiasm are exactly what I should avoid. My design is closer to "research-from-creation": data generated through participants' engagement with the work.

**Additional dissertations (shorter notes):**
- **A. Miroshnichenko (2020).** A developer-diary research-creation project (Cat Game) building a multimodal design framework. It claims games "guide behaviour formation" without participant evidence. *Lesson:* a creator's reflection alone cannot support claims about participants.
- **Mayoral Baños (2021).** Design principles derived from five years of building the Indigenous Friends Platform with community collaborators. Long-term relationships, IP and not-for-profit governance are part of the method. *Lesson:* community software is a governance project, and consent forms do not replace governance.
- **Borkowski (2025).** Archival analysis of séance practices beside Alexa, plus artist interviews (Wesley Goatley). *Lesson:* historical and discursive framing of AI voices; artists' practice as evidence.
- **Russell (2026).** Cross-media interpretive analysis of the gynoid as an "ideological interface", including "consent as a default setting". It includes a playable Twine game, *Singularis*, in Appendix L, but the game is barely integrated into the argument. *Lesson:* integrate the creative work into the argument. Her concept of consent as a design default is relevant to my design of consent and refusal.

**Cross-cutting [I]:**
1. Successful ComCult dissertations involving technology frame the interface or system as an *actor* in a cultural relation. They are not engineering contributions.
2. They name one main framework explicitly.
3. They are reflexive about the author's position.
4. Research-creation dissertations vary a lot in how far the creative work carries the argument. The ones that integrate it treat the artifact as a site where evidence is generated.

None of these is a template. The program sets requirements, not models.

---

## 3. Rebecca Caines and her projects (Stage 3)

### 3.1 Role and status

- [V] AMPD profile (https://ampd.yorku.ca/profile/?p=107851): **Associate Professor**, Department of Theatre; Program Coordinator, Creative Technologies at Markham. Executive member of the International Institute for Critical Studies in Improvisation (IICSI). Director of the Regina Improvisation Studies Centre, 2013–2019. PhD in Performance Studies, University of New South Wales.
- [V] Her personal site (about.html) still says "Assistant Professor in Creative Technologies in the Department of Theatre and Performance", so it is out of date. The 2022 seminar listing also says Assistant Professor.
- [V] ComCult faculty member, listed in Media & Culture and Technology in Practice.
- [V] Publications checked:
  - Caines (2026), *American Journal of STEM Education* 21: 175–202, DOI 10.32674/aztpg851. A research-creation study of GenAI in STEAM classrooms. Full text read.
  - Caines and Watson (2023), *Performance Matters* 9(1–2): 253–277. Abstract read.
  - "Fragile Devices: Improvisation as an Interdisciplinary Research Methodology", chapter 19 in *The Bloomsbury Handbook of Sonic Methodologies*, pp. 325–340. Abstract read. The year is given as 2020 or 2021; see the note in the bib file.
  - Book in progress, *Fragile Devices: Improvisation, Emerging Technologies and Community*, for Temple University Press (IICSI page).
- [V] From Caines (2026), full text:
  - She taught "Creating with AI" in Fall 2024 and the final showcase, "Synthetic Horizons", was in 2025.
  - She describes "AI as companion species" (after Jennifer Walshe), a "third way" between unthinking uptake and "strategic AI illiteracy", and GenAI creativity as "a kind of critical improvisation practice".
  - She is attentive to privacy tiers: she paid for subscriptions with no-training guarantees and chose not to require students to use HeyGen.
  - She observed demographic defaults in DALL·E 3 portraits.
  - She is co-developing "Biskaabiiyaang", an Anishinaabe-language game world, with Dr. Maya Chacaby and Nokiiwin Tribal Council. It is funded through Connected Minds and a SSHRC reconciliation grant. "Our youth workshops specifically using GenAI in game creation began in Spring 2026."
  - [V] The Biskaabiiyaang website names Chacaby, Nokiiwin Tribal Council, York and UniVirtual, and states adherence to OCAP®. It does **not** name Caines.

### 3.2 Project-fit table

| Project | Dates and status | Caines's documented role | Aims, participants, methods, outputs, verified technologies | Relevance to my proposal [I] | Needs her confirmation [?] |
|---|---|---|---|---|---|
| **multiPLAY** (multiplay.ca; rebeccacaines.org/project1.html) | 2019–2022 per project1 page; 2019–2021 per multiplay.ca. **Historical.** | Lead artist / coordinator, with a national team | Canada Council-funded digital community engagement with regional Canadian improvisers. Methods: workshops, open studios, livestreamed talks, an artist-run hackathon. Technologies: panoramic livestream video, VR, facial recognition, participatory physical computing, digital radio. Output includes the **multiPLAY app**: 360° video and positional sound across six artists' scenes, developed by John Campbell, launched 2022-09-23, archived on the Internet Archive (WebGL, iOS, Android, Windows, macOS). | Precedent for digitally mediated improvisation and ethical artist/community collaboration. Possible source of artists and interview participants. The app is a precedent, not a platform I can modify. | Whether former multiPLAY artists could be invited to interviews; any lessons from the project about mediation. **Not an active recruitment project.** |
| **ImprovEnabled** (rebeccacaines.org/project4.html; improvenabled.rebeccacaines.org/canada/) | Pilot 2015–16, feasibility 2016–17; "Improvise and Mobilize" 2017–19; described as expanding to Canada, Northern Ireland and Australia. | Co-lead with Dr. Michelle Stewart | Strengths-based improvisation with people living with FASD in Saskatchewan and Yukon. Principle: "people living with FASD are the experts on FASD". Methods: improvised theatre games, storytelling, iPad instruments, craft. Output: *Playing to Our Strengths* toolkit. | A participant-led, strengths-based precedent for how to design workshops and consent. **I will not propose FASD or disability-focused recruitment.** | Whether its consent and facilitation practices can inform my protocols. |
| **Sonic Blankets** (project2) | 2018–2020; sub-project of multiPLAY. **Historical.** | Lead artist with Stewart | Sound and wearables (hoodie with body speakers and LEDs) with youth with sensory differences. | Precedent for wearables in community art, close to my MA's wearable work. | Not relevant for recruitment. |
| **Yukon Wanderers** (project3) | Through 2021. Historical; final showcase planned for 2021. | Lead artist with Stewart | Digital photography, GPS drawing and video with peer leaders, with Options for Independence, FASSY and Yukon Arts Centre. | Context only. | — |
| **Improvised Remembering: Noise into Signal** (project5) | 2016 residency, ISEA2016HK. Historical. | Co-artist with John Campbell | DIY digital media and participatory performance tools for remembering place. | Precedent for participatory digital performance tools. | — |
| **Liquid Art** (project6) | Undated. | Curator | Live painting with improvised music, schools and elders. | Context only. | — |
| **Improvisation Methodologies in Creative Technologies** (IICSI) | Undated; University of Regina. | Co-lead with Charity Marsh | Documents how improvisatory methodologies help negotiate "human/technology interaction", including "access, media literacy, differing abilities, responsibility" and facilitator–participant power. | Directly relevant concepts: facilitator power and improvisation as a methodology for technology. | Whether there are related publications I should read. |
| **"Creating with AI" course / research-creation study** | 2024–2026 (Caines 2026) | Instructor and researcher | GenAI tools (ChatGPT Teams, NotebookLM, DALL·E 3, Midjourney) in a mixed CS, engineering and fine-arts class. | Shows her current interest in GenAI and "improvisatory" AI practice. A possible pilot or interview context **only with separate ethics approval and no teaching conflict.** | Whether alumni or showcase artists could be interviewed. |
| **Biskaabiiyaang** | Ongoing; GenAI youth workshops from Spring 2026 | Co-developer and fundraiser, per Caines (2026). Not named on the project site. | Indigenous-led (Chacaby, Nokiiwin); OCAP®. | **Out of scope.** I have no relationship, governance role or relevant expertise. Mentioned only so I don't approach it unknowingly. | Only if Rebecca and the project's Indigenous leadership invite it, which I don't expect. |
| **Interfacing, Playtesting, Resetting: Reframing Technology Use Through Improvised Creative Technologies** | Announced 2026-07-24 (YFile). SSHRC **Insight Grant**, **$118,750**. YFile says Insight Grants support research "over four to six years"; this project's own duration isn't stated. | Named recipient (AMPD) | **Only the title and amount are public.** No methods, participants, partners, technologies or AI component are documented. | The title ("playtesting", "interfacing", "improvised creative technologies") suggests a fit with iterative, participatory testing of interfaces, but that is my inference. | Everything: aims, timeline, whether it includes workshops, whether a student sub-study is possible, whether AI is in scope, data governance, authorship of outputs. |

### 3.3 Case-study context

- [P] **Primary, if she agrees:** a student sub-study within, or alongside, *Interfacing, Playtesting, Resetting*. It would run small-group digital improvisation workshops with adult improvising artists and creative-technology practitioners in Toronto, using the project's playtesting framework if one exists. This depends on her confirming the project's scope.
- [P] **Alternative, independent of her funded project:** I recruit adult improvisers and creative practitioners myself, through open calls to Toronto improvisation, theatre and sound communities and to York AMPD students. I would exclude students I teach. A community arts organisation could host, if one agrees, with honoraria. Rebecca's IICSI networks would help, but I would not assume them.
- [P] **Excluded unless properly invited and governed:** Indigenous-led projects (Biskaabiiyaang) and FASD or disability communities (ImprovEnabled).

---

## 4. Manuscript analysis (Stage 4)

### 4.1 Files

- [V] *Reading a Remote Teammate's Body*: `Downloads/Reading_a_Remote_Teammate_s_BodyACM 2026 Turino.pdf`. 27 pages, "Manuscript submitted to ACM", July 2026. **The "(4)" version you named does not exist on this computer.** I read this one in full.
- [V] BioTerrarium exists in two different versions:
  - `SIGGRAPH_2026_….pdf`: 10 pages, dated 2026-01-22, "Paper ID 1585". This is the SIGGRAPH-named version you specified (identical copies in Downloads ×2 and Desktop/SIG Video). Read in full.
  - `Embedding_Physiological_….pdf`: 11 pages, 2026-07-11, ACM template with placeholder venue. Revision. Read in full.
  - **The "(20261011-064925)" file does not exist.**
- [V] eCAADe 2023: `Downloads/ecaade2023_198.pdf`, read in full. Jahandideh, Romman; Jahandideh, Aran; Kim, Ikwan (Crossref: Ikhwan). eCAADe 41, Vol. 1, pp. 149–158, DOI 10.52842/conf.ecaade.2023.1.149.
  - Method: 60 participants, Quest 2, Unreal 4.27, forced-choice paired comparisons (12 colour conditions × 4 transparency levels; 264 comparisons each), Kendall's coefficients of agreement and consistency.
  - Reported finding: classical colour and luminance depth cues held at 10% and 40% transparency but reversed at 60–90%, where cool and dark colours were seen as nearer.
  - [?] The results text supports H3 "in 40% and 60%" and rejects it "in 60% and 90%". 60% appears in both, which is an internal inconsistency.
  - [I] The discussion's claims about machine-learning implications go beyond the data.

### 4.2 Teammate paper: what it does

**Research questions [V]:**
- Study 1: can players identify HR and HRV states from the icon (RQ1); do the channels carry graded meaning (RQ2); is workload acceptable (RQ3).
- Study 2: does the cue improve awareness (RQ2.1), support timing (RQ2.2), invasiveness (RQ2.3), and pipeline reliability (RQ2.4).

**Commitments [V]:**
- STS: Bowker and Star on classification, Barad on measurement as constitutive, Haraway on situated knowledge.
- Suchman and Dourish on situated reading.
- No emotion labels; states relative to each player's baseline; constant amber hue; baseline "shimmer" so that calm isn't presented as the ideal.

**System [V]:**
- Apple Watch (Series 7+) → HealthKit companion app → local API → bridge that classifies four HR states × four HRV (RMSSD) states → Unity.
- Only the classified state is replicated over the network.
- A debounce rule controls flicker.

**Study 1 [V]:**
- Online; 36 participants; 16 animated stimuli.
- HR identified at 66.3%, HRV at 58.2% (chance 25%); joint identification 44.6% (chance 6.25%).
- Monotonic trends in urgency, stability and support intention.
- TLX below midpoint.
- Privacy boundaries ("only with clear consent and an easy off switch").

**Study 2 [V]:**
- 36 new participants in 12 triads; Overcooked-style Unity task; No Cue / Numeric / Icon, Latin square; three scripted pressure events.
- Support response time: 15.3 s (none), 12.5 s (numeric), 11.4 s (icon). Icon vs none: −3.9 s, p < .001. Icon vs numeric: not significant.
- Numeric was rated more useful (5.50 vs 5.30), more trusted (5.55 vs 5.24) and scored higher on missions (932 vs 896).
- Icon was rated less invasive (3.19 vs 4.39) and lower in workload.
- Desire for visibility control rose under *any* disclosure.
- Communication coding (488 utterances): support offers and strategy-change talk rose under the icon.

**Findings vs. general conclusions [I]:**
- Reported: label-free icons are legible above chance in this sample, and the icon condition is associated with faster support after scripted events.
- Not established:
  - That the cue *caused* teammates to read a teammate's state. The paper doesn't show the cue changed at the pressure events.
  - That it "steadies coordination at a lower privacy cost" in general. Invasiveness was self-rated, and the sample was a convenience sample of 36 people.

**Things to check before resubmission [?]:**
1. *Measurement and representation:* during play, participants were classified as "Reduced/Suppressed" HRV (V3/V4) on 84.6% of samples, and HR4 on only 0.1%. Table 2 labels V3/V4 "possible physiological strain" and "reduced regulatory stability". The display avoids words, but the classification itself carries evaluative labels, and most play was placed in the "strained" categories. This bears directly on the paper's own STS argument.
2. *HRV source:* the paper says HRV was "computed as RMSSD through HealthKit". HealthKit's native HRV type is SDNN, so RMSSD needs beat-to-beat (heartbeat series) data. Confirm exactly how it was computed, and how valid short-window PPG HRV is during active play.
3. *Did the cue change at the events?* Support speed could reflect game cues rather than the halo. Report the cue states around event onset.
4. *Citations:* "Amos 2015", cited for research-creation, is actually a RACAR book review about craft and the woman professional. Müller et al. 2013 concerns brain synchronisation in guitar improvisation, not cooperative biosignal display. Gan et al. 2022 is a PCANet health-detection paper, not an affective-gaming survey.
5. *Ethics wording:* Study 1 says the live pipeline was "proposed… at the time", but §3.6 says both studies were approved together before data collection. Harmonise.
6. *Abstract:* calls the Study 2 sample "trained", while the limitations section stresses "first-time viewers" with one tutorial round.
7. *Reliability:* the trust construct has α = .66, TLX items α = .13, one primary coder, and no a priori power analysis at the team level (the paper acknowledges the last two).

### 4.3 BioTerrarium: what it does

**January version [V]:**
- Unity "glass-bottle" survival ecosystem. Apple Watch → BLE/HealthKit → Swift bridge → WebSocket → "Bioadaptive State Engine".
- Four HR-reserve zones: ≤60%, 61–70%, 71–80%, >80%, with HRmax = 220 − age.
- Drives fog, vegetation, light and blur. At "overdrive", controls degrade.
- Within-subjects design, n = 24, bioadaptive vs. control ("identical environmental changes" in a "fixed, randomized" sequence).
- Reported: HR 71.4 vs 76.7; RMSSD 65.8 vs 50.8 ms; PANAS+ up, PANAS− down; FSS 6.2 vs 4.9; MAAS up (p < .05).
- Qualitative themes: "breathing back", "calming when I calmed".

**Inconsistencies to resolve before any reuse [?]:**
1. **Tense and status:** the July revision describes participants as people who "will be recruited" and analysis that "will be" run, yet keeps the same results tables and abstract. Either the study was run or it wasn't. Clarify what data exist.
2. **Quotes changed between versions:** January has "The world felt responsive when I calmed down"; July has "It felt like the world was breathing back—when I calmed down, the fog lifted". Participant quotations must be verbatim from transcripts.
3. **HR-reserve zones vs. reported HR:** for a 26-year-old (HRmax = 194) with a resting HR of about 70, 60% of reserve is about 144 bpm. Mean HRs of 71–77 bpm imply almost all play was in Zone 1, which contradicts the reported 79% vs. more time in Zones 3–4.
4. **HRV mapping:** the abstract and §3 say HRV shapes the world. §3.7 says HRV "was recorded… but not visually represented".
5. **Control condition:** "fixed, randomized" is contradictory. A sequence that degrades the world independently of the player is also not a neutral comparison.
6. **Session details:** "12 males and 12 males"; sessions described as 20, 30 and 45 minutes; conditions "on different days" but also "each 45-minute session" including both; latency below 100 ms in one place and below 200 ms in another; Series 7 vs Series 8.
7. **Measures:** MAAS is a trait measure used as a state outcome. Table 3's MAAS SD differs from the text. Figure 6's bar values don't match Table 3.
8. **Mis-cited sources:** Chakrabarti et al. 2007 (network visualisation), Tearse 2011 (Minstrel story generation), Christoforou et al. 2021 (crowdsourced data), Zaccaro et al. 2018 (cited for somaesthetics) and Porges (cited for direct control mappings) don't support the claims attached to them. July adds "Martin-Niedecken's" zoning with no reference.
9. **Causal language:** "demonstrating that self-regulatory control was improved" is too strong for this design.

**[I] Use in the PhD documents:** mention BioTerrarium only as an implemented responsive Unity environment whose evaluation is under revision. **Do not cite its results.**

### 4.4 Transferable strengths [I]

- Building end-to-end systems alone: Unity, C#, networked multiplayer, a device-to-engine bridge, data minimisation (sending classified states rather than raw streams), logging.
- Mixed-methods design: forced-choice legibility tests, Latin-square counterbalancing, communication coding, reflexive thematic analysis, ethics approval.
- A recurring theme of designing for interpretation rather than verdicts.
- The teammate paper's richest finding is about visibility *control* and consent ("the right to be illegible"), not speed.

### 4.5 Intellectual shift [I]

- Both MA projects ask how a system can make a person's state readable to someone (teammates or the self), and how people interpret what it displays.
- The unresolved issue in both is **who controls the system's interpretation**: participants asked for off switches and permissions, and the classification scheme encoded evaluative categories.
- The PhD moves from *involuntary bodily signals interpreted by the system* to *deliberate creative contributions transformed by a generative model*, and from *consent to visibility* to *recognition, contestation and refusal of transformation*.
- It keeps the strengths of the MA work (shared spaces, ambient and spatial communication, participant interpretation) and drops emotion inference completely.

---

## 5. Literature and the research gap (Stages 4–5)

### 5.1 What exists

All [V] from abstracts or full text, as noted.

1. **Mixed-initiative and co-creative AI.**
   - Horvitz 1999; Amershi et al. 2019 (guidelines include "support efficient dismissal" and "efficient correction").
   - Guzdial et al. 2019: creators read an AI level editor as friend, collaborator, student or manager.
   - Rezwana and Maher 2023 (COFI); Zhang et al. 2025: a scoping review of 134 papers on agency in co-creation.
   - These model *individual* human–AI dyads and control mechanisms.
2. **Generative AI in groups.**
   - Xu et al. (CHI 2026, abstract): 27 students in small groups, analysed through distributed cognition. In synchronous use, the GenAI interaction space worked as "attentional anchors, shared memory, and negotiable contributions to group decisions".
   - Johnson et al. 2025: a CSCW workshop on GenAI for groupwork.
   - **So group GenAI use is an established and growing topic. "Groups plus generative AI" is not a gap.**
3. **AI and improvisation/performance.**
   - Mathewson and Mirowski 2017: improvised theatre with AI performers.
   - Mirowski et al. 2023: co-writing scripts.
   - Trajkova et al. 2024: LuminAI dance partner, focus groups with 24 dancers, dyadic.
   - These treat AI as a **partner or performer**, not as a **mediator** that transforms one participant's material into a shared work for others.
4. **Authorship and credit.**
   - Epstein et al. 2020: how credit is assigned depends on whether the AI is anthropomorphised. Experimental vignettes.
   - Draxler et al. 2024: the "AI ghostwriter effect" in individual writing.
   - Jiang et al. 2023: harms to artists.
   - Epstein et al. 2023: art and generative AI.
   - Mostly individual, experimental or survey-based. They do not observe authorship being negotiated *in situ* in groups.
5. **Contestability and refusal.**
   - Hirsch et al. 2017; Lyons et al. 2021 (contesting algorithmic *decisions about people*).
   - Garcia et al. 2020 (refusal as a feminist data practice).
   - Im et al. 2021 and Strengers et al. 2021 (affirmative, ongoing consent).
   - These come from decision-making and platform contexts. Contesting a machine's *creative reading of your contribution* is less theorised.
6. **Participation and power.** Birhane et al. 2022: participatory AI and "participation-washing"; Bennett and Keyes 2020: disability and the limits of fairness.
7. **Model defaults.** Bianchi et al. 2023: text-to-image stereotypes. Caines (2026) observed DALL·E defaults. Richards (2025) describes "safe-model" closures.
8. **Communication and cultural theory.**
   - Suchman 2007: agency and authorship are *attributed* in situated practice.
   - Woolgar 1990: technologies configure their users.
   - Fischlin, Heble and Lipsitz 2013: improvisation as an ethics of co-creation and rights.
   - Sawyer and DeZutter 2009: distributed creativity.
   - Chapman and Sawchuk 2012; Loveless 2019: research-creation.
9. **Interpretation.** Gaver et al. 2003; Sengers and Gaver 2006; Boehner et al. 2007; Barrett et al. 2019; Stark and Hoey 2021: the limits of inferring affect. These are the bridge from my MA work.

**Not yet read in full (to read before the formal proposal):** Xu et al. 2026 (abstract only); Trajkova et al. 2024 (metadata and summary only); Johnson et al. 2025 (abstract only); Hua and Raley 2020; Woolgar 1990; Fischlin et al. 2013 (introduction). I didn't find SIGGRAPH literature that genuinely informs this design, so none is cited. Your own SIGGRAPH submission is the only SIGGRAPH link.

### 5.2 Testing the provisional question

- Provisional: *"How do participants and facilitators negotiate whose creative intentions are represented when generative AI transforms their contributions into a shared digital environment?"*
- [I] **Weak version:** "how do groups use GenAI together?" Already studied (Xu et al. 2026). Novelty from Unity or the technology combination is not a contribution.
- [I] **Defensible version:** existing work leaves three things under-explained:
  - (a) how a *particular person's* contribution comes to count (acknowledged, transformed, incorporated, credited) once a model has reinterpreted it in a group;
  - (b) how the right to contest or refuse a machine's transformation is exercised *socially*: who has the standing to object, and who resolves disagreement, including facilitators;
  - (c) how the interface, the model's defaults and the facilitator's practices together *configure* these possibilities in improvisation, where uptake of others' offers is a core cultural norm.
- [P] **Refined question:** *In collaborative digital improvisation, how do participants, facilitators and a generative-AI interface jointly determine whether, and how, a person's contribution is acknowledged, transformed, taken up, contested and credited in the shared work?*

### 5.3 Framework

- [P] **Primary: Suchman's human–machine reconfigurations (2007).** Plus Woolgar's "configuring the user" for the design side.
- [P] **Complementary: critical improvisation studies,** limited to two ideas: uptake or "listening" to offers, and co-creation as an ethical and rights-bearing relation (Fischlin et al. 2013; Caines 2021).
- [I] **Operational links:**
  - **Attribution** (Suchman): code how participants assign agency and authorship in talk and action ("the AI made it", "that's mine", "we decided"). Compare with what the provenance log records.
  - **Configuration** (Woolgar/Suchman): document how my design decisions, the interface's permissions, the model's defaults and the facilitator's moves make some actions easy and others hard. My design journal is data.
  - **Located accountability** (Suchman): who is treated as responsible when a transformation misrepresents someone.
  - **Uptake** (improvisation): was the offer acknowledged and built on? Uptake is a social achievement, not a click count.
- [I] **Why not ANT, used by McArthur and Chalk?** ANT is also viable. Suchman is chosen because she focuses on how agency is *attributed* and on situated interaction with machines, which is exactly the authorship question, and because she provides a vocabulary for the designer's own accountability.

---

## 6. Three directions compared (summary of Stage 5)

| | A. AI-mediated collective authorship in digital improvisation (chosen) | B. Participant-governed interpretation in ambient responsive environments (no AI necessity) | C. Discursive and practice study of GenAI in Canadian creative-technology education (no system) |
|---|---|---|---|
| Question | How contributions come to count when a model transforms them in group improvisation | How groups set rules for how a shared space represents them (extending the teammate paper's visibility controls) | How educators and artists frame "improvisatory" AI literacy |
| ComCult fit | Strong: participation, authorship, cultural production, Technology in Practice | Moderate: risks being an HCI continuation | Strong, but distant from your practice strengths |
| Rebecca fit | Strong: improvisation, creative technologies, her current AI interest | Moderate | Strong, but overlaps her own published study |
| Why AI is needed | Studying responses to *machine interpretation* of creative material needs an interpretive, non-deterministic transformer | Not needed: rules would do | Object of study, not a tool |
| Feasibility for you | High: Unity, multiplayer, studies, LLM API experience | High | Moderate: interviews and discourse analysis are newer methods for you |
| Main risk | Access to groups; model costs and data processing | Weak originality | Little research-creation; competes with her work |

[P] **A is chosen.** B's concern with participant control is folded into A's design. C becomes background interviews in Phase 1.

---

## 7. Design choices [P] (details in the proposal)

- **Input:** short typed text phrases, optionally with a choice from a small set of participant-made sketches in later phases. Text first, because it is easiest to log, consent to and process with minimal data. Speech-to-text was rejected because voice data adds third-party processing and identifiability.
- **AI role:** an existing language model maps one contribution to one *proposal*. The proposal is a JSON object, validated against a schema, choosing from a closed vocabulary of Unity actions over a curated asset library: place or modify a form, light, colour field, weather or particle system, sound layer, text fragment, all with clamped parameters. It includes a one-sentence "reading" of the contribution that participants can see.
- **What the AI cannot decide:** whether anything enters the shared work, who is credited, whether a contribution is removed, and anything about participants themselves.
- **Controls:** the contributor and/or the group can inspect, edit parameters, accept, reject, ask for another reading, or undo. A **non-AI path** (place or transform material manually from the same library) is always available.
- **Unity execution:** a command pattern over whitelisted actions only, so every action is undoable and logged. Model output is never executed as code.
- **Failure handling:** invalid JSON or unknown asset/action → discard and show "no proposal", the non-AI path stays open; timeouts; a rate-limit fallback; "AI off" for the session.
- **Provenance:** each element stores contributor pseudonym, original text, model and prompt-template version, the proposal, and each decision with who made it and when. Attribution visibility is a session setting, because visible credit can also expose people.
- **Model and cost:** prefer a locally run open-weight model if quality is adequate, which avoids third-party processing. Otherwise use a hosted API under York-approved terms with no training on inputs, sending only the text contribution. Costs for short text requests are modest but must be budgeted and confirmed. No training or fine-tuning of foundation models.
- **Mediation arrangements compared (as probes, not a controlled experiment):**
  1. The contributor alone accepts or rejects proposals for their own material.
  2. The group decides on proposals.
  3. A non-AI arrangement where a human (facilitator or participant) transforms material using the same library.
  - Arrangement 3 is the meaningful comparison: it separates "being transformed by someone else" from "being transformed by a model".

---

## 8. Unresolved questions (also in `discussion-notes.md`)

1. The exact status of both manuscripts, and whether the BioTerrarium study was run as reported (§4.3).
2. Whether *Interfacing, Playtesting, Resetting* can host a student sub-study, and what its methods, timeline and governance are.
3. Whether the proposal should be due four or five months after comps (§1.2).
4. Whether a constructed HCI minor is still offered.
5. Whether a single-authored writing sample exists.
6. Whether York's research ethics board permits hosted LLM processing of participant material, and under which institutional agreements.
7. The year of the Bloomsbury chapter: 2020 or 2021.

---

## 9. Source and process log

| Date | Item | Location | Limitation |
|---|---|---|---|
| 2026-10-11 | York program pages and PDFs (§1) | URLs in §1.1 | Some PDFs are dated 2014–2017 "updated". Policies may have been revised since. |
| 2026-10-11 | YorkSpace API harvest, 134 records | yorkspace.library.yorku.ca/server/api | York deposits only |
| 2026-10-11 | 10 dissertation PDFs | handles in `references.bib` | Partial reading; see §2.2 |
| 2026-10-11 | Caines pages: rebeccacaines.org (about, project1–6), multiplay.ca, multiplay app page, improvenabled …/canada/, AMPD profile, TMU profile, IICSI pages, Google Scholar | URLs in §3 | The personal site blocks scripted access, so I read it through a fetch tool, and it is out of date |
| 2026-10-11 | YFile 2026-07-24 announcement | URL in §3.2 | Title and amount only |
| 2026-10-11 | Caines 2026 full text | DOI 10.32674/aztpg851 | — |
| 2026-10-11 | Crossref DOI checks of every journal/proceedings entry | api.crossref.org | Abstracts unavailable for some ACM items (ACM DL returns 403) |
| 2026-10-11 | Your PDFs and CVs | local paths in §0 and §4 | The two filenames you gave were not found; the closest versions were used |
| 2026-10-11 | Tectonic 0.17.0 (session scratch folder only) used to compile | github.com/tectonic-typesetting | Overleaf may use a different engine and TeX Live version |
