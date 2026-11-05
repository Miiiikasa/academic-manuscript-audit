---
name: academic-manuscript-audit
description: >-
  Audit academic submission packages against the current requirements for a
  specific journal, article type and submission stage. Check completeness,
  anonymisation, cross-file consistency, format, figures, references, integrity,
  argument, language and abbreviations. Supports full, targeted and follow-up
  audits, revision packages and optional recent-publication benchmarks.
metadata:
  category: academic-writing
  version: "3.1.1"
  last_updated: "2026-11-05"
  license: CC-BY-NC-SA-4.0
---

# Academic manuscript audit

## Select the mode

- **A · Full submission audit.** Use when the user requests a submission
  readiness or whole-package audit. Start with intake and scope confirmation
  below. Review the complete confirmed package.
- **B · Targeted audit.** Use for named areas such as figures, references,
  abbreviations, anonymisation, supplementary material, layout, language or
  argument. Confirm only what the requested checks depend on. Use journal
  sources for journal-specific claims. Apply general guidance if the user
  wants a generic review. Label the narrower scope in both outputs. A full
  document supplied for a targeted review does not trigger mode A.
- **Follow-up audit.** Apply the requested A or B scope to the current
  versions and prior findings. Report new, changed or still-open items.
  Use [follow-up and revision](references/re-audit-and-revision.md).
- **Journal revision.** Apply revision-stage instructions to the chosen
  scope, including clean, marked and response artifacts where required.
  A revision package can also be a follow-up audit.
- **Recent Publications Benchmark.** Run as an optional module or on its own.
  Use [benchmark protocol](references/recent-publications-benchmark.md) for
  eligibility, inspection, counting and comparison. Published practices
  inform optional suggestions and cannot set submission requirements.

All audit modes are read-only for supplied materials. A, B and follow-up
audits produce `Submission Checklist.md` and `Issues and Recommendations.md`.
When a benchmark runs, use `Recent_Publications_Benchmark.md` as its output.
Reports give findings and repair directions. Keep replacement wording,
rewritten passages and revisions outside the audit.

## Full-audit intake

First collect the target journal's full title, article type, author-guide
availability and local path if downloaded, and the submission folder or
explicit file set. Resolve ambiguous journal identity with an official URL or
ISSN when needed. Ask only for missing information, preferably in one short
message. If the user says no guide was downloaded, find the current official
guide. If there is a local guide, read it and compare it with the current
official version where possible.

Scan the supplied location and show filenames, count and provisional roles.
Confirm the intended set unless it was already confirmed. Ask separately about
quantity only if access is incomplete or the scan conflicts with the user's
description. Ask about stage or review model when needed for applicability.
While scope is incomplete, continue with the confirmed subset and label any
reports provisional. Conclusions about a full package require a confirmed scope.

Unless already answered, offer the optional comparison using around ten recent
PDFs from the target journal and same article type. Any sample size is
acceptable. Continue the submission audit if the user declines, does not
answer, or supplies no sample.

## Review workflow

1. **Bind the rules to this submission.** Use
   [journal requirements](references/journal-requirements.md) to build the
   authority and applicability ledger. Prefer current applicable official
   instructions to local guides, general guidance and historical checklists.
2. **Check the package and reconcile copies.** Use
   [submission package](references/submission-package.md) for inventory,
   anonymisation, front matter, Cover Letter, cross-file facts, final layout
   and export checks. For a revision or follow-up, apply the corresponding
   version and artifact checks before comparing the files.
3. **Inspect evidence and its presentation.** Apply the relevant checks in
   [figures, tables and equations](references/figures-tables-equations.md),
   [references and citations](references/references-and-citations.md), and
   [integrity and availability](references/integrity-and-availability.md).
   Record what could actually be opened, rendered, checked externally or
   corroborated. Keep partial coverage and unverified items visible.
4. **Review the manuscript as an argument.** Use
   [whole-paper review](references/whole-paper-review.md) for evidence,
   contribution, paragraph function and necessity, repetition, and the editor
   and reader assessment. Then use [language review](references/language-review.md)
   and [abbreviation review](references/abbreviation-review.md). Apply this step
   only to the requested dimensions in mode B. Keep reasoning notes internal
   unless needed to explain a finding.
5. **Compare recent publications if requested.** Inspect the sample, report
   each feature's assessable denominator and compare observed practices
   with the current official rules and any supplied manuscript. Use the
   [benchmark template](templates/Recent_Publications_Benchmark.md).
6. **Record evidence and prioritise.** Use the
   [report contract](references/report-contract.md) and the
   [checklist](templates/Submission%20Checklist.md) and
   [issues](templates/Issues%20and%20Recommendations.md) templates. Reconcile
   IDs and locations across the two files. Distinguish mandatory rules,
   journal recommendations, general norms and optional improvements.

## Review principles

- Preserve scientific meaning. Check values, precision, denominators, units,
  time windows, populations, categories, directions, citations, attribution,
  uncertainty and claim strength. A repair direction must not invent evidence,
  mechanisms, novelty, policy implications or stronger conclusions. Flag
  scientific terminology and meaning decisions for author confirmation.
- Tailor the checks to the article, stage and design. A missing section,
  unnumbered equation, embedded figure, language variant, or absent declaration
  is actionable only when the applicable rule or scientific need supports it.
  Respect figure readability and explain project-specific codes where needed.
- Use only the five result states defined in the report contract. Separate
  an evidenced defect from an outstanding author decision or access limit.
- There is no quota. Merge manifestations of one root cause and prioritise
  supported findings over optional style ideas. Report no issues when the
  evidence warrants it. The existence of a possible alternative does not
  make the original defective.
- A check passes only for the stated scope when its evidence supports that
  result. Do not infer authenticity, ethics approval, valid
  authorship, reproducibility or lack of image manipulation from a declaration
  or a visual scan. Do not infer AI use from writing style.
- Review supplied materials locally. Public lookups can use public citation
  identifiers, journal names and approved public links. Do not transmit
  unpublished text, data, images, author information or reports to external
  services or a portal without explicit permission. A submission audit never
  submits, uploads, publishes or changes portal state.
- An optional local profile can be supplied explicitly or named
  `academic-audit.local.md` in the confirmed manuscript directory. Use the
  [project profile template](references/project-profile-template.md) only when
  needed. The profile records evidence and author decisions. It cannot
  override current applicable requirements or support invented claims.

For provenance and redistribution terms, see [NOTICE.md](NOTICE.md).
