# Detection Use Case Guide

Use this structure for each detection. Replace prompts with evidence-backed details.

## Title and status

State the behavior, owner, platform, and status. Distinguish planned work, unvalidated queries, lab validation, and production deployment.

## Threat scenario and objective

Explain the activity being detected, its security relevance, and what the alert can and cannot establish.

## Telemetry and prerequisites

List log sources, collection settings, event identifiers where relevant, required fields, normalization, retention, and known gaps. Provide a sanitized sample event.

## Detection logic and query

Explain the conditions, grouping keys, correlation window, thresholds, exclusions, and baseline assumptions. Include the complete query and actual platform/schema requirements. Do not claim portability without testing.

## MITRE ATT&CK mapping

Record relevant technique identifiers, names, official references, and why the observed behavior supports the mapping. Do not add mappings based only on keywords.

## Validation evidence

Record the test environment and date, sample input, expected matches, observed matches, and query execution results. Include benign activity and boundary cases. State explicitly when execution has not been tested.

## False positives and tuning

Explain legitimate scenarios and how to distinguish them. Scope exclusions narrowly and document their impact on coverage.

## Analyst investigation

Describe initial evidence checks, related events to correlate, identity and asset context, enrichment sources, and escalation criteria. Separate suspicious evidence from confirmed compromise.

## Response considerations

Describe possible next actions and required authorization. Avoid assuming every alert warrants blocking or account disablement.

## Limitations and maintenance

Document blind spots, possible evasion, data dependencies, performance considerations, and when the detection should be reviewed.
