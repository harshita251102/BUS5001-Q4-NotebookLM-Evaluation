# NotebookLM experiment log

Observed interaction date: 12 October 2026 (Melbourne). Log assembled: 13 October 2026.

## Inputs and method
The notebook was titled “WaterWise ESG Training Evaluation”. Two initial sources were visible: WaterWise Pilot Results and WaterWise Training Policy (second title truncated in screenshots). The task was to prepare an ESG briefing using these simulated coursework materials.

Assessment focuses on accuracy/relevance, academic usefulness and limitations for each observed capability. Findings below apply to this small case only. The invented 20-session dataset is input content, not a sample of 20 NotebookLM evaluations.

## E1 — Source-based questions and numerical interpretation
Prompt intent (reconstructed, not a verbatim captured prompt): calculate the percentage of all sessions ending in a summary, the percentage of completed summaries involving a location correction, and the percentage of sessions including help; explain why help is not an additional outcome group.

Observed response supplied in the conversation:
- 12 / 20 × 100 = 60% completed summaries.
- 3 / 12 × 100 = 25% of completed summaries involving a correction.
- 5 / 20 × 100 = 25% of all sessions including help.
- Help can overlap with outcomes and must not be added to the total.

Check: all three calculations agree with R2–R3 in evidence_05_source_check.png. Outcomes sum to 12 + 4 + 2 + 2 = 20. This screenshot verifies the inputs; the original calculation response is recorded above from the pasted response, not independently shown in that screenshot.

Academic usefulness: assists students with denominator selection and interpretation of a small dataset when writing an evidence-based briefing.

Limitation: correct arithmetic on invented inputs does not establish real-world effectiveness. This is three checked calculations in one scenario, not a general accuracy benchmark. No statistical or complex calculation capability was tested.

## E2 — Synthesis of limitations and training needs
Prompt provided in the workflow:
“What are the main evidence limitations of the WaterWise simulated pilot, and what staff training is needed before a real-world trial? Use only the provided sources and distinguish findings from recommendations.”

Observed result: the pasted output separated evidence limitations from recommendations. It identified missing water-saving and service-outcome data, unestablished reliability/accessibility, lack of an approved retention policy and summary-only functionality. Recommendations covered consent, minimal data, safety referral, correction, manual submission and human support.

Evidence: evidence_01_limitations.png shows the limitations portion. The full recommendations were pasted in the conversation; they are not all visible in that image.

Accuracy/relevance: the response addressed the prompt and distinguished findings from recommendations. Numerical and summary-only claims are supported by the visible source excerpt. Full verification of policy-specific assertions requires the complete training-policy source; citation badges alone do not establish accuracy.

Academic usefulness: helps a student organise policy reading into findings and practical implications, and helps a lecturer identify topics for a workshop.

Limitations: some statements depend on source coverage; absence of evidence is not evidence of a successful outcome. Recommendations require human interpretation. Bias was not systematically tested; a narrow set of authored sources can omit alternative perspectives.

## E3 — Briefing generation and revision
Initial prompt provided:
“Draft a 150-word executive briefing for campus support stakeholders using only the provided sources. Include the pilot results (60% completed summaries; 25% of completed summaries involved location correction; 25% of all sessions included help requests), key evidence limitations, and recommended staff training. Clearly state that the sessions were simulated and completed summaries were not submitted tickets. Include source citations and no follow-up question.”

Initial result: a relevant briefing, but its opening referred to “simulated pilot testing”, which could suggest actual testing rather than invented source figures. The percentages were already supplied in the prompt, so this synthesis output is not an independent arithmetic test.

Revision prompt:
“Revise this briefing to exactly 150 words, excluding the title and citations. Explicitly describe the figures as invented simulated coursework data, not actual university or chatbot test results. Preserve the percentages, evidence limitations, staff-training recommendations and source citations.”

Observed result: the revised text explicitly labelled the figures as invented coursework data, preserved the denominators and distinguished summaries from submitted tickets. The pasted final body contains 150 whitespace-separated words after removing citation markers and excluding the heading.

Evidence: evidence_02_initial_briefing.png, evidence_03_revised_briefing.png and evidence_04_saved_note.png; full transcription in EXECUTIVE_BRIEFING.md.

Academic usefulness: produces a concise first draft for a policy briefing or research summary and responds to targeted feedback.

Limitations: human review was needed to clarify provenance. “Unapproved data retention policy” may imply an existing policy awaiting approval, whereas “no approved data-retention policy” is more precise. Dense compression makes the final training sentence harder to read. The revision success does not prove the output is complete or all citations are correct.

## E4 — Citation checking
Action: inspect the original Pilot Results passage and manually compare the output figures.

Observed result: the displayed source contains 20 sessions, 12 summaries, 3 corrected summaries and 5 sessions with help. R2 also states that a summary does not mean a ticket was submitted.

Evidence: evidence_05_source_check.png.

Academic usefulness: supports traceability and checking a generated claim against its source, useful during report preparation.

Limitations: the screenshot shows the supporting passage but does not independently record the entire click sequence. Only the displayed numerical and scope claims were checked against this excerpt. A citation to an invented source supports the exercise calculation, not a real-world effectiveness claim.

## E5 — Saving and organising notes
Action: save the final response as “WaterWise Executive Briefing”.

Observed result: the note is visible in evidence_04_saved_note.png. The generated briefing also appears among the selected sources, increasing the visible count from two to three.

Academic usefulness: keeps an output available for later drafting and review.

Limitation: using the generated briefing as another source can create circular support. The workflow advised deselecting it and keeping only the two original sources for further questions. The screenshot does not verify that deselection was subsequently completed.

## Overall feasibility reflection
This case supports a limited, supervised use of NotebookLM for reading support, drafting and checking source-based summaries. It does not establish learning gains, reduced workload, accessibility, privacy compliance or technical integration with university systems. Retain human source checks, distinguish invented data from empirical evidence and prevent generated notes from becoming independent evidence. A broader university trial would need representative materials, repeated checks, diverse users, accessibility evaluation and institutional review of data handling. These are recommendations, not completed experiments.
