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
  version: "3.1.2"
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

**Ask the user and wait when required intake is unresolved.** Before starting
the full audit, establish the target journal, article type, whether the user
has a local author guide (and its path if applicable), and which files and
versions belong to this submission. Ask about stage or review model when it
affects applicability and cannot be resolved from available evidence. Reuse
answers already given for this submission. See
[journal intake](references/journal-requirements.md) for evidence and access.

Scan a supplied folder read-only. Show the candidate filenames, count and
provisional roles, then ask which files to include unless the user has already
clearly identified the submission set. A directory listing alone is not
confirmation. Ask separately about quantity only if the scan is incomplete
or conflicts with the user's description.

Send the missing questions as a user-visible message, grouped when practical.
Use the host's question tool when available. If the tool is unavailable, ask
in a chat reply and end that turn. Wait for the user's answer before running
checks that depend on it. While waiting, a read-only inventory or lookup of
public journal instructions may help prepare the audit. Do not infer answers
from filenames or treat silence as confirmation. Produce a partial audit
before intake is resolved only if the user requests one. Limit it to confirmed
inputs, label it provisional and withhold a whole-package conclusion. Once
the scope is confirmed, proceed even if required files are known to be missing.

Offer the optional [recent-paper comparison](references/recent-publications-benchmark.md)
once during intake unless the user already answered. Ask alongside required
questions when possible. An unanswered benchmark offer never delays the audit.
Mode B asks only for information needed for the requested checks.

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
