# SOC Detection Engineering

**Turning emerging threat research and evolving attacker tactics into actionable SOC detection use cases.**

A threat-informed detection engineering portfolio focused on identifying recent and emerging threats, understanding attacker tactics, techniques, and procedures (TTPs), and translating that research into SIEM detection logic and analyst investigation workflows.

Created by [Siva Modugumudi](https://github.com/shiva-modugumudi), a security professional with experience in SOC operations, incident response, threat hunting, and cloud security.

## Purpose

Show how a published threat report becomes a practical detection: identify the attacker behavior, determine the required logs, develop a query, test its coverage, and document how an analyst should investigate the alert. Help students learn this process and let hiring managers assess the research, reasoning, and validation behind each use case.

## Research-to-detection workflow

1. Select a recent threat advisory, campaign report, or newly documented technique.
2. Record the original source, publication date, research date, and relevant evidence.
3. Extract observable attacker behaviors and map supported behaviors to MITRE ATT&CK.
4. Identify telemetry requirements and write a detection hypothesis.
5. Build platform-specific detection logic using Splunk SPL, Microsoft Sentinel KQL, or Sigma where appropriate.
6. Test suspicious and benign activity; record results, false positives, and visibility gaps.
7. Document investigation steps and review the detection as the threat evolves.

A newly published report may describe an established technique. Each use case will distinguish newly observed behavior from known techniques used in a recent campaign. Publication dates alone do not establish novelty.

## Focus areas

- Emerging campaigns and changes in attacker tradecraft
- Identity compromise and authentication abuse
- Endpoint execution, persistence, and defense evasion
- Cloud identity abuse and control-plane activity
- Command-and-control activity and data exfiltration
- Detection gaps, tuning, and investigation guidance

Behavior-based detection is the primary focus. Indicators such as IP addresses, domains, and file hashes may support an investigation; their source, observation date, and limitations must be documented.

## Use case catalog and status

See the [detection catalog](detections/README.md) for research priorities and implementation status.

**Current status:** Research workflow, repository structure, and documentation guide established. No specific emerging campaign has been researched in this repository yet. Detection queries and validation evidence have not been added.

## What each use case will include

| Component | Details |
| --- | --- |
| Threat research | Original references, publication dates, research date, campaign context, and evidence |
| Attacker behavior | Observed TTPs, detection hypothesis, and supported ATT&CK mappings |
| Required telemetry | Log sources, event types, fields, collection settings, and gaps |
| Detection logic | Platform-specific query, correlation window, thresholds, and assumptions |
| Validation | Test inputs, expected and observed results, environment, and date |
| False positives | Legitimate explanations and scoped tuning options |
| Investigation | Evidence checks, correlation, enrichment, and escalation criteria |
| Maintenance | Coverage limitations, last review date, and changes in attacker behavior |

## Repository guide

| Location | Purpose |
| --- | --- |
| [detections](detections/README.md) | Threat research backlog and future detection use cases |
| [Use case guide](docs/use-case-guide.md) | Research-to-detection documentation and validation template |

When work begins, use a descriptive folder such as `detections/<threat-or-behavior>/`. Keep research notes, queries, and sanitized validation examples together. Every query must identify its platform, log schema, prerequisites, and actual test status.

## Quality and evidence

Use original advisories, vendor research, or incident reports where available. Separate reported facts, analyst inferences, and lab observations. Mark work as lab validated only when test evidence is recorded; lab validation does not imply production readiness. Do not publish credentials, private incident data, or unsanitized logs.

## Relationship to Secure Automations

This is a dedicated detection engineering repository. [Secure Automations](https://github.com/shiva-modugumudi/Secure-Automations) remains the separate portfolio for automation workflows and integrations.
