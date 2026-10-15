# Emerging Threat Detection Catalog

This catalog tracks the conversion of emerging threat research into SOC detections. Every implemented use case must connect a dated source report to observable attacker behavior, required telemetry, detection logic, and validation evidence.

## Research priorities

These are research themes, not claims about verified current campaigns. Specific reports and techniques will be selected and cited before development.

| Research theme | Detection research objective | Status |
| --- | --- | --- |
| Emerging identity attacks | Identify observable sign-in, session, or token abuse behavior from a selected report | Research planned |
| Evolving endpoint tradecraft | Translate reported execution, persistence, or defense evasion into endpoint detections | Research planned |
| Cloud attack techniques | Detect reported identity abuse, control-plane changes, or logging interference | Research planned |
| Command-and-control and exfiltration | Identify reported communication or data movement patterns using available telemetry | Research planned |

## Use case tracking

When research starts, add a linked use case with: source report and publication date, behavior and ATT&CK mapping, target platform, required logs, status, and last reviewed date.

Use these statuses accurately:

- **Research planned:** No source-specific research or query completed.
- **Research documented:** Sources and detection hypothesis recorded.
- **In development:** Query or rule being built; validation incomplete.
- **Lab validated:** Recorded tests demonstrate expected matches and benign-case behavior in the stated environment.
- **Needs review:** Threat behavior, telemetry, or detection assumptions have changed.

No source-specific use cases, detection queries, or validated coverage are available yet. The earlier generic scenario list has been replaced with this threat-research backlog to match the repository's focus.

Follow the [use case guide](../docs/use-case-guide.md).
