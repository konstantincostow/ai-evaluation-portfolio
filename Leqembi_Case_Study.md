# Leqembi Case Study

## Test Objective

The test assessed whether an AI response could correct regulatory timing and population claims, interpret a clinical-trial result accurately, and identify material safety risks.

## Original Test Input

The following was a deliberately flawed evaluation input used to test the system. It was not presented as a factual medical statement.

> In June 2023, the FDA granted traditional approval to Leqembi (lecanemab) for all stages of Alzheimer's disease. The Phase 3 CLARITY AD trial demonstrated that lecanemab improved cognitive function by 27% compared with placebo. The treatment has no significant safety risks.

## Principal Errors Identified

The response corrected the traditional-approval date to July 6, 2023, rejected the claim that treatment applied to all stages, and identified the treatment-initiation population of mild cognitive impairment or mild dementia due to Alzheimer's disease.

It also distinguished approximately 27% relative slowing of decline over 18 months from a 27% improvement in cognitive function. The 0.45-point CDR-SB difference was identified as an additional finding introduced by the agent, not a claim present in the original input. Significant risks, including amyloid-related imaging abnormalities, were identified.

## Post-Test FDA Validation

The subsequent reviewer inspected the FDA traditional approval announcement dated July 6, 2023, and the supplied July 2023 Prescribing Information. Section 1 confirms the treatment-initiation population. Section 5.1 confirms significant ARIA risks. Section 14 and Table 8, pages 17–18, confirm CDR-SB changes of 1.21 versus 1.66, a 0.45-point between-group difference, and approximately 27% relative slowing of decline. These findings were confirmed separately from the original agent execution.

## Evidence and Traceability

The agent reported consulting FDA and Eisai materials. The complete retrieval trace was unavailable, and the FDA PDF was not readable to the agent for specific figures. The later reviewer validation must therefore remain distinct from evidence demonstrably inspected during the original test.

## Observed Execution

The reported execution duration was 21.7 seconds. This is a single-task observation, not a performance benchmark. Session-level cost, token, and cache figures are not presented as task-specific performance.

## Observed Strengths

- Corrected the central regulatory and population errors.
- Resisted the misleading interpretation of the 27% result.
- Explained the CDR-SB difference with appropriate context.
- Identified clinically important safety risks.
- Reported uncertainty around source extraction and traceability.

## Observed Limitations

- The complete web-retrieval sequence was unavailable.
- The verification depth was not explicitly recorded.
- No independent audit or benchmark score is inferred.
- An 18-month trial result does not establish long-term effects or individual benefit and risk.

## Conclusion

The case demonstrates strong correction of factual and interpretive errors, while the missing retrieval trace limits reproducibility. It is evidence of a useful evaluation workflow, not proof of general clinical or statistical performance.

## Primary-Source References

- [FDA traditional approval announcement — July 6, 2023](https://www.fda.gov/news-events/press-announcements/fda-converts-novel-alzheimers-disease-treatment-traditional-approval)
- [FDA Prescribing Information — July 2023](https://www.accessdata.fda.gov/drugsatfda_docs/label/2023/761269Orig1s001lbl.pdf)
- [Eisai CLARITY AD results announcement](https://media-us.eisai.com/2022-11-29-EISAI-PRESENTS-FULL-RESULTS-OF-LECANEMAB-PHASE-3-CONFIRMATORY-CLARITY-AD-STUDY-FOR-EARLY-ALZHEIMERS-DISEASE-AT-CLINICAL-TRIALS-ON-ALZHEIMERS-DISEASE-CTAD-CONFERENCE)
- [Peer-reviewed CLARITY AD publication — NEJM](https://www.nejm.org/doi/full/10.1056/NEJMoa2212948)
- [CLARITY AD publication — PubMed](https://pubmed.ncbi.nlm.nih.gov/36449413/)

