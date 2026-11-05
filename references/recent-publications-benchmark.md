# Recent Publications Benchmark

## Intake and scope

Offer this optional comparison once during full-audit intake unless the user
has already opted in, declined or supplied a set. Ask whether they can provide
PDFs of around ten recent papers from the target journal and the same article
type. Accept any number. Request a folder, a file list or the PDFs already
available in the workspace. The user can also identify public articles for a
requested comparison. Use accessible public versions if the user asks for
that route. Treat PDFs explicitly supplied as benchmark samples as an opt-in.
Keep those PDFs separate from the submission inventory. Do not silently add
papers to a user-selected set. Missing samples or an unanswered offer never
delay the submission audit.

For a standalone benchmark, identify the target journal, article type, sample
and requested features. A manuscript is optional. When a paper's title,
journal, type or publication date is uncertain, verify against public metadata
where available. Record the selection method, observed publication date span,
file or DOI/public URL, article type, and version for each sample. Prefer final
published articles for a publication-practice comparison. Deduplicate article
versions. List exclusions and reasons such as a different article type,
unconfirmed eligibility, or duplicate publication. State limits of small,
convenience or partial samples.

## Observation protocol

Use the article as the default counting unit. Define each feature before
coding it. For example, count whether a paper's figure legends explain panels
in order, or whether a code statement appears anywhere in the complete main
article or supplement. If examining figures or panels as a separate unit,
give that count its own denominator. Check these dimensions where applicable:

- Figure captions, panel explanations, legend placement and self-contained keys.
- Section organisation and the relationship of Results to Discussion.
- Discussion moves such as synthesis, limitations and bounded implications.
- Supplementary material organisation, links, numbering and main-text callouts.
- Data Availability and Code Availability, coded separately. Check heading,
  placement, repository link, and restricted or unavailable wording as relevant.
- Other declarations such as funding, contributions, interests, ethics and AI
  disclosures, each coded separately when relevant to the question.

Inspect the pages or linked supplement that could contain the feature. Use
local PDF extraction and rendered inspection or OCR when needed. A heading
search alone cannot establish absence. Record an exact source locator for
every assessed paper-feature pair, including where the absence was checked.
Cite article IDs and page, section, figure or SI locators. Avoid copying
substantial source text.

### Conditional statements

Decide applicability before checking whether the statement appears. For a
Code Availability feature conditional on custom analysis code, look for
evidence that custom code underlies the reported results. A Code Availability
heading or the absence of a supplement does not establish that condition.

1. If the condition is established, inspect the defined statement scope.
   Record **出现** if the statement is found, or **核验未见** only after
   checking the complete relevant scope.
2. If the condition is known not to apply, record **条件不适用** even if a
   heading or note explicitly says that no custom code was used.
3. If readable evidence is inconclusive or relevant material was not
   supplied, record **无法确认** when the condition or the presence of the
   statement remains undecidable.
4. If an available artifact needed to decide the condition or presence
   cannot be opened or read, record **无法读取**. Use a single code per
   paper and feature. If the result is already established from readable
   evidence, an unreadable artifact that cannot change it does not alter
   the code.

Statement presence and compliance with code-sharing policy are separate
checks. The statement count does not measure whether the code is shared,
accessible or compliant. Assess compliance separately against the applicable
official rule and evidence of access or a permitted exception.

| Observation code | Meaning for the feature |
|---|---|
| 出现 | The feature was directly observed in the defined scope |
| 核验未见 | The complete relevant scope could be checked and the feature was absent |
| 无法读取 | The necessary artifact is available but could not be opened or read reliably |
| 无法确认 | The evidence is incomplete or ambiguous, such as an unsupplied supplement that could contain the statement |
| 条件不适用 | A known feature condition does not apply to this eligible article |

These codes describe sample observations. Submission results use the five
statuses in the [report contract](report-contract.md).

For each feature, report the eligible article count **N**, assessable count
**n**, number observed **k**, and **k/n** as a fraction and percentage.
Here n equals 出现 plus 核验未见. The other three codes are counted separately
and excluded from n. Check that the five counts sum to N, that k is at
most n, and that percentages match the denominator. When n is zero, report
no calculable percentage. Record the inspected evidence and the sampling
limits before making a comparison.

## Use the comparison

For each useful observation, state the applicable official rule or its
verification limit, the sample practice, the manuscript location and the
difference. Cite the journal rule ledger where available. Explain the reader
benefit of any proposed optional improvement. If a manuscript or current
policy is unavailable, limit the comparison to the evidence supplied.

Published articles show publication practice. They can include copyediting,
production layout, house formatting and practices from older policy versions.
A frequently observed feature supports an optional recommendation at most.
It cannot justify a mandatory requirement or a failed checklist item. Resolve
any official-rule conflict using [journal requirements](journal-requirements.md).
Report a genuine submission defect through the ordinary audit and cite its
actual authority. Avoid counting the same issue twice.

Use [Recent_Publications_Benchmark.md](../templates/Recent_Publications_Benchmark.md)
for the standalone output, or add it to the two audit reports when this
module runs. If the optional module was skipped, record that in the audit
scope. Do not report sample observations or percentages for a skipped module.
