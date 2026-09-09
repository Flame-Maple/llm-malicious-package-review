# Review Evidence Data

This repository contains the minimum structured data needed to verify the search accounting, study selection, included-study inventory, role classification, evidence assessment, claim mapping, and sensitivity analysis reported in *Large Language Models for Malicious Package Detection*.

## Search date and status

- Review search cutoff: 2026-08-31.
- Last completed search execution: 2026-08-31.
- Publication-status freeze: 2026-09-01.
- Status: the update search covering records and report versions through 2026-08-31 is complete.
- Frozen publication-status composition: 19 peer-reviewed publications, 4 accepted or proceedings-listed reports, 8 preprints, and 1 master's thesis.

## File

`review_evidence_data.xlsx` contains the following worksheets:

- `Metadata`: dataset scope, version, date fields, and missing-value conventions.
- `Search_Strategy`: executed sources, exact queries or rules, execution dates, and result counts.
- `Selection_Records`: 127 deduplicated records, comprising 39 formal-screening records and 88 record-level exclusions.
- `Selection_Flow`: review flow and primary-role counts, with workbook checks where the retained data permit direct recalculation.
- `Included_Studies`: 32 included studies, 30 research families, role assignments, ecosystems, inputs, and stable identifiers.
- `Evidence_Assessment`: study-level inputs and seven-domain assessment values for the 32 included studies.
- `Audit_Rubric`: role- and task-specific operational definitions for the seven assessment domains. This rubric is a reconstruction aid, not a validated study-quality or risk-of-bias scale.
- `Role_Codebook`: necessary conditions, exclusions, and tie-break rules for role assignment.
- `Claim_Evidence`: evidence mapping for 10 consecutively numbered review claims. C1 and C2 are cross-scenario mappings, C3 and C4 are direct corpus audits, and C5–C10 are secondary or contextual claims.
- `Sensitivity_Summary`: 72 structured combinations of three method-score thresholds, four weighting schemes, two publication subsets, and three family partitions for C1 and C2. C2 maps five retrieved-knowledge comparisons. Publication status restricts the eligible subset and does not contribute to method scores.

## Conventions and scope

`NR` means not reported. A blank cell means not applicable or unavailable. Assessment domains are interpreted against each study's stated role and task. Stable identifiers are provided as DOI or public URLs where available. Copyrighted full texts, licensed database exports, and private working notes are not included.

The structured second pass rechecked all uncertain records, citation anchors, and flagged discrepancies. For the remaining clear decisions, records were ordered by record identifier within the Include and Exclude strata, and the first and every tenth subsequent record in each stratum were selected for rechecking.

The sensitivity thresholds are structured specifications rather than validated quality cutoffs: 7/14 is the scale midpoint, and 5/14 and 9/14 are symmetric two-point departures. Equal weighting is the neutral reference; the three alternative schemes emphasize core validity, causal rigor, or reporting and reproducibility. The 27-family stress rule provisionally groups otherwise separate studies when overlapping authorship coincides with a closely related package-analysis task or modeling context, although the direct system or version relation required by the documented-family rule is absent. It additionally groups the Zeshan evaluation with the RAG evaluation/MA-MPD/LAMPS family, H2GLM with GMLLM, and RULE LLM with GenTTP. These are dependence stress assumptions, not revised lineage claims.

A public reuse licence and persistent repository identifier should be assigned by the authors before archival release.
