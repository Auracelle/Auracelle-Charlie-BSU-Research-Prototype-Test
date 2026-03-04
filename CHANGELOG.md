# Changelog

All notable changes to this project will be documented in this file.

## [0.2.0] - 2026-03-04
### Added
- **Tab ⑧ Autonomous Simulation** — fully AI-driven session mode with no human input. Runs alongside human sessions to generate comparison data for foresight validation (Objective 4).
- **Tab ⑨ Red Team & Shock Injection** — adversarial stress-testing engine:
  - 9 shock event cards (Data Breach, Unilateral Withdrawal, Classified Leak, AI Incident, Sanctions, Public Legitimacy Crisis, Industry Defection, Great Power Veto, Cyberattack on Process)
  - Red team agent designation with inverted reward functions
  - Resilience recovery curve and event log
  - Research methodology context panel (Objectives 4 & 5)
- **MITRE ATT&CK® integration** (v14, Enterprise + ICS matrices):
  - ATT&CK technique tags on all 9 existing shock cards (orange ⬡ badges mapping each shock to documented technique IDs and tactics)
  - ATT&CK group badges on red-teamed agents (e.g. APT41 for China, APT29 for credential threats)
  - 4 compound multi-step adversarial chains (fired in 3 staged turns, each turn logged to Red Team Event Log):
    - **Supply Chain Compromise** — T1195.002 → T1059 → T1562.001 · APT41 / Winnti
    - **Coordinated Influence Operation** — T1583.006 → T1586.002 → T1491.002 · Sandworm / VOODOO BEAR
    - **Insider Credential Exfiltration** — T1078 → T1552.001 → T1213 · APT29 / Cozy Bear
    - **ICS Leverage & Governance Coercion** — T0816 → T0826 → T0880 (ICS matrix) · XENOTIME / Triton
  - ATT&CK methodology note added to research context card with citation: *MITRE ATT&CK® v14, mitre.org/attack*
  - ATT&CK layer positioned as technical threat input model beneath E-AGPO-HT (framework preserved)

### Notes
- E-AGPO-HT v3.1 framework (Strata III, 7 BGC, ~40 NOF) fully preserved — ATT&CK integration is additive only
- Compound shocks apply staged delta values to all six governance indicators over 3 × 1.8s intervals
- ICS compound shock (XENOTIME) models coerced compliance — unique indicator signature for Objective 5 analysis

## [0.1.0] - 2026-03-02
### Added
- Initial single-file interactive HTML prototype (`index.html`) with:
  - Session configuration
  - Facilitator move logging
  - Governance indicators
  - Foresight validation tab
  - After-Action Review generation
  - JSON/CSV export tooling (prototype behavior)
