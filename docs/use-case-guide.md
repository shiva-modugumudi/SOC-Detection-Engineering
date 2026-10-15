# Emerging Threat Research-to-Detection Guide

Use this template for every use case. Replace prompts with evidence-backed details.

## 1. Title, summary, and status

State the threat or observable behavior, detection objective, owner, platform, creation date, and last review date. Distinguish research planned, research documented, in development, lab validated, and needs review.

## 2. Threat research and source provenance

Record the original report title, publisher, URL, publication or update date, and date reviewed. Summarize the campaign, affected environments, and observed attacker behavior. Distinguish newly documented techniques from known techniques used in recent activity. Separate source-reported facts from analyst inference; do not describe a threat as recent or emerging without dated evidence.

## 3. Attacker behavior and detection hypothesis

Explain the observable sequence and why the selected telemetry could reveal it. State what an alert can and cannot establish. Prefer behavior-based logic; document the provenance, observation dates, and limitations of any supporting indicators.

## 4. MITRE ATT&CK mapping

Record technique identifiers, names, official references, and why the source evidence supports each mapping. Do not assign techniques based only on keywords. Note uncertainty or incomplete evidence.

## 5. Telemetry and prerequisites

List log sources, collection settings, event identifiers where relevant, required fields, normalization, retention, and gaps. Provide sanitized sample events and identify behavior that cannot be observed with the available logs.

## 6. Detection logic and query

Explain conditions, sequence, grouping keys, time window, thresholds, exclusions, and baseline assumptions. Include complete platform-specific queries and schema requirements. Identify whether the implementation uses Splunk SPL, Sentinel KQL, Sigma, or another format. Do not claim portability or query execution without testing.

## 7. Validation evidence

Record the authorized lab environment, test date, inputs, expected matches, observed matches, and execution results. Test suspicious behavior, benign activity, and boundary cases. Use sanitized or synthetic events where appropriate and disclose that limitation. State explicitly when a query has not been executed. Lab validation does not imply production readiness.

## 8. False positives and tuning

Explain legitimate scenarios and how to distinguish them. Scope exclusions narrowly and describe the coverage lost through tuning.

## 9. Analyst investigation

Describe initial evidence checks, related events, identity and asset context, enrichment, and escalation criteria. Separate suspicious evidence from confirmed compromise.

## 10. Response considerations

Document proportionate containment and remediation options, evidence preservation, and required authorization.

## 11. Coverage gaps and maintenance

Document blind spots, possible evasion, telemetry dependencies, performance constraints, and untested assumptions. Record the last review date and review triggers, including updated source research, changed attacker behavior, schema changes, and new false positives. Maintain a short change log linking query changes to their evidence.
