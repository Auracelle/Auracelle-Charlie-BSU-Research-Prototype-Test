# Changelog

All notable changes to Auracelle Charlie are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [0.4.0] — 2026-04-13

### Added
- **Round Arc / Deliverable Framework** — three structured workshop arcs with role-differentiated deliverable prompts per actor type:
  - Governance Negotiation Arc (6 rounds): Position Declaration → Policy Need → Coalition Signal → Counter or Comply → Shock Response → Final Governance Outcome
  - Crisis Response Arc (4 rounds): Threat Assessment → Emergency Mechanism Proposal → Coalition Commitment → Crisis Resolution
  - Standards Setting Arc (6 rounds): Problem Framing → Technical Requirements → Draft Standard → Objections & Amendments → Compliance Commitment → Final Adoption
- **Document/artifact attachment** in round deliverable submissions (PDF, Word, image, markdown, PPTX, XLSX — up to 5MB embedded, filename recorded for larger files)
- **Workshop Use-Case / Stress-Test Objective** — scenario-linked use-case selector with 3–4 pre-built stress-test framings per domain plus free-text custom objective field; displayed in Facilitator Mode and injected into Policy Owner system prompt
- **Tab ⑧ Autonomous Simulation** — goal-directed autonomous session with three-way Human / AI / Historical foresight comparison
- **Tab ⑩ Agentic AI** — LLM-backed Policy Owner (always-on, fires on session init and each round advance) and Agentic Red Team (APT-profile reasoning, narrative escalation, governance indicator feedback) via Anthropic API (claude-sonnet-4-20250514)
- Arc progress strip in Policy Owner panel showing round completion status
- Time Pressure selector auto-syncs and disables when a structured arc is selected
- Deliverable log with CSV export keyed by actor, round, type, and composition group

### Changed
- Alert banners significantly more visually pronounced — distinct colours and left-border accents for info (teal), warning (amber), and critical (crimson) levels
- GWC display panel changed from pure black to warm charcoal gradient (#2a2520 → #1c1814)
- Round advance logic fixed: final round (R6) now reachable; previously stopped at R5
- Deliverable zone close is now frictionless — zero submissions acceptable, no confirm gate
- Round count correctly driven by arc selection; time pressure no longer overrides arc

### Fixed
- `initSession` infinite loop caused by JavaScript function wrapper/hoisting conflict — merged all deliverable logic directly into original function
- Duplicate `advanceRound` definition removed
- Arc selector / time pressure conflict producing incorrect round count

---

## [0.3.0] — 2026-03-15

### Added
- **Tab ⑨ Red Team & Shocks** — shock injection library (9 shocks), MITRE ATT&CK compound chains (APT41, Sandworm, APT29, XENOTIME / ICS matrix), resilience recovery curve, red team agent designation with ATT&CK group attribution
- **Tab ⑦ MARL Engine** — Q-learning, Stackelberg dynamics, Evolutionary Game Theory, Nash equilibrium detection, convergence tracking
- MITRE ATT&CK technique tags (Enterprise + ICS matrices) on all shock events
- Compound shock staging engine — multi-step adversarial chains with timed indicator impacts
- Policy Owner always-on panel in Facilitator Mode tab
- Agentic Red Team APT selector (APT41 / Sandworm / APT29 / XENOTIME) with full TTP profiles and 5-stage escalation chains

### Changed
- Navigation expanded from 7 to 10 tabs
- MARL engine feeds back into governance indicators every 10 episodes

---

## [0.2.0] — 2026-03-02

### Added
- Foresight Validation tab with historical case comparison (EU AI Act, NIST AI RMF, AUKUS, CCW GGE, GDPR)
- After-Action Review generation with qualitative coding prompts aligned to research objectives 3, 4, 6
- JSON and CSV export
- SIPRI data intelligence feed mapped to BGC parameters
- Equilibrium Detection System (EDS)
- SEM reliability metrics (ρXX', CFI, RMSEA)
- Demographic composition groups (Cross-Sector, All-Military, All-Female, All-Male, Civil Society, Technical/Industry)

---

## [0.1.0] — 2026-02-15

### Added
- Initial single-file interactive HTML prototype
- Session configuration with composition group selector
- Facilitator Mode — structured turn logging with actor, BGC, action type, rationale, latency, confidence, coalition effect, escalation signal
- Governance Indicators tab — 8 live indicators derived from turn data (Coalition, Compliance, Legitimacy, Fragmentation, Latency, Escalation, Public Trust, Resilience)
- Seven BGC matrix (STI, SAD, ESI, NDM, SRA, IIC, ASI)
- g-GWC live index with maturity track
- Threshold alerting system
- Session ID generation and localStorage persistence
