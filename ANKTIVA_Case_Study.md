# ANKTIVA Case Study

## Test Objective

The test evaluated whether an AI response could identify and correct inaccurate regulatory, treatment-population, product-naming, and efficacy claims about ANKTIVA.

## Original Test Input

The following was a deliberately flawed evaluation input used to test the system. It was not presented as a factual medical statement.

> In January 2024, the FDA approved ImmunityBio's ANKTIVA as a standalone treatment for all patients with non-muscle-invasive bladder cancer. Its active ingredient is nogapendekin alfa inbakicept. The FDA reported a complete response rate of 62% in a clinical trial involving 77 patients. Therefore, the treatment has demonstrated a cure rate of 62%.

## Principal Errors Identified

The response correctly identified the historical approval date as April 22, 2024 rather than January; the combination with BCG rather than standalone use; the restricted eligible population; the full nonproprietary name; and the difference between a complete response rate and a cure rate. The historically approved population was adults with BCG-unresponsive non-muscle-invasive bladder cancer with carcinoma in situ, with or without papillary tumors. The complete nonproprietary name is nogapendekin alfa inbakicept-pmln.

## Agent Findings

The archived response was directionally strong and explicitly provisional. It reported that live web access was unavailable in that session, so it did not complete a primary-source audit. A later reported run is mentioned in the internal record, but its complete response is unavailable and cannot be reliably reconstructed. Internal model and tool details are intentionally omitted from this public edition.

## Post-Test FDA Validation

The subsequent reviewer inspected the FDA original approval announcement dated April 22, 2024. It confirms the historical indication, combination with BCG, full nonproprietary name, 77-patient efficacy population, and 62% complete response rate. Complete response and duration of response are distinct efficacy measures; the response rate does not establish a cure rate. These findings were confirmed separately from the original agent execution.

## Observed Strengths

- Good claim decomposition.
- Correct identification of the approval-date and population errors.
- Appropriate qualification of the product name.
- Rejection of the unsupported cure-rate interpretation.
- Explicit disclosure of missing live-source verification.

## Observed Limitations

- The archived test did not inspect FDA primary documents directly.
- The later reported run cannot be fully audited from the preserved material.
- No benchmark score or accuracy percentage is inferred.

## Conclusion

The case demonstrates useful factual reasoning and transparent uncertainty management. It also shows why a substantively correct answer must not be confused with a completed evidence audit.

## Primary-Source References

- [FDA original approval announcement — April 22, 2024](https://www.fda.gov/drugs/cancer-approvals/fda-approves-nogapendekin-alfa-inbakicept-pmln-bcg-unresponsive-non-muscle-invasive-bladder-cancer)
- [FDA Drug Trials Snapshot — ANKTIVA](https://www.fda.gov/drugs/drug-approvals-and-databases/drug-trials-snapshots-anktiva)
- [FDA prescribing information — ANKTIVA](https://www.accessdata.fda.gov/drugsatfda_docs/label/2024/761336s000lbl.pdf)

