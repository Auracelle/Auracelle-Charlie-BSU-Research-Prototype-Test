# Changelog — Auracelle Charlie

All notable changes to this research instrument are documented here.  
Format: `[Build] — Date — Summary`

---

## [BSU Demo v2] — March 2026

### Added
- **Tab ⑨ Red Team & Shocks** — fully restored and upgraded
  - 9 standard shock events with MITRE ATT&CK® technique tags (Enterprise matrix)
  - 4 compound multi-step adversarial chains with APT group attribution:
    - Supply Chain Compromise (APT41/Winnti) — T1195.002 → T1059 → T1562.001
    - Coordinated Influence Operation (Sandworm/VOODOO BEAR) — T1583.006 → T1586.002 → T1491.002
    - Insider Credential Exfiltration (APT29/Cozy Bear) — T1078 → T1552.001 → T1213
    - ICS Leverage & Governance Coercion (XENOTIME/Triton) — T0816 → T0826 → T0880 (ICS matrix)
  - ATT&CK group badges on red-teamed agent cards (visible on designation)
  - Governance resilience recovery curve (SVG)
  - Adversarial autonomous simulation engine
  - Research methodology context card with ATT&CK citation

### Fixed
- **Critical:** `switchTab()` crashed with `TypeError` when called programmatically (no live `event` object) — caused `initSession()` to abort silently, leaving session badge as "NO SESSION ACTIVE" and preventing all indicator movement
  - Root cause: `event.currentTarget.classList.add('active')` called without a real browser event
  - Fix: Safe fallback using `typeof event !== 'undefined'` check with DOM `querySelector` fallback
- **Secondary:** Removed duplicate `switchTab('facilitate')` direct call in `initSession()` (leftover from editing); only the `.click()` programmatic call is needed

---

## [BSU Demo v1] — February 2026

### Initial BSU research instrument build
- 8-tab platform: Session Design, Facilitator Mode, Governance Indicators, Foresight Validation, After-Action Review, SIPRI Data, MARL Engine
- E-AGPO-HT v3.1 framework: Stratum III g-GWC, 7 BGC scoring, governance indicator engine
- Multi-Agent Reinforcement Learning engine (Q-learning + policy gradient, EGT population)
- Autonomous simulation mode (Obj 6 comparison instrument)
- Historical case validation (EU AI Act, Paris Agreement, NPT, GDPR, Biological Weapons Convention, CPTPP)
- JSON and CSV session export
- SIPRI arms transfer and military expenditure reference data
- World Bank, UN Comtrade real-world data metrics integration
- BSU doctoral research branding: PI Evans G-A., Supervisor Dr. John Curry

---

*Framework: E-AGPO-HT v3.1 · PI: Evans, G-A. · Bath Spa University · Auracelle AI Governance Labs*
