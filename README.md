# SOC Detection Engineering

**SIEM use cases, detection logic, and analyst investigation workflows.**

A growing portfolio that turns security scenarios into documented detections, with attention to log requirements, query logic, validation, false positives, and investigation steps.

Created by [Siva Modugumudi](https://github.com/shiva-modugumudi), a security professional with experience in SOC operations, incident response, threat hunting, and cloud security.

## Purpose

Help students understand how detections work and give security teams and hiring managers a clear view of the reasoning behind each use case—from the suspicious behavior to the evidence an analyst should examine.

## Scope

- Authentication and identity threats
- Endpoint execution and persistence
- Cloud account and configuration changes
- Network activity and potential command-and-control behavior
- Data access and potential exfiltration
- Detection tuning and investigation guidance

Queries may use Splunk SPL, Microsoft Sentinel KQL, or Sigma where appropriate. Each implementation will identify its actual platform, log schema, prerequisites, and validation status.

## Use case index

See the [detection catalog](detections/README.md) for planned scenarios and implementation status.

**Current status:** Repository structure and documentation guide established. Detection queries and validation evidence have not been added yet.

## What each use case will include

| Component | Details |
| --- | --- |
| Threat scenario | Behavior of interest and why it matters |
| Required telemetry | Log source, event types, required fields, and collection prerequisites |
| Detection logic | Query, correlation window, thresholds, and assumptions |
| ATT&CK mapping | Relevant techniques with supporting rationale and references |
| Validation | Test input, expected result, observed result, and environment |
| False positives | Legitimate explanations and scoped tuning options |
| Investigation | Evidence checks, enrichment, escalation criteria, and response considerations |
| Limitations | Visibility gaps, evasion opportunities, and unsupported cases |

## Repository guide

| Location | Purpose |
| --- | --- |
| [detections](detections/README.md) | Detection catalog and future use case folders |
| [Use case guide](docs/use-case-guide.md) | Consistent format for developing and reviewing detections |

Use descriptive folders such as `detections/password-spraying/` when an implementation begins. Keep its documentation, platform-specific queries, and sanitized validation examples together.

## Development approach

Define the behavior and required telemetry, build the query, test expected matches and benign cases, document investigation steps, then review tuning and limitations. Mark a detection as validated only when evidence is recorded. Lab validation does not imply production readiness.

## Relationship to Secure Automations

This is a dedicated detection engineering repository. [Secure Automations](https://github.com/shiva-modugumudi/Secure-Automations) remains the separate portfolio for automation workflows and integrations.
