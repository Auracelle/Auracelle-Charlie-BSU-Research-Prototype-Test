# Auracelle Charlie — BSU Research Instrument

**Testing Public Policy Outcomes through War Gaming Methodologies for Strengthening AI Governance**

> Evans, G-A. (2024–) · Bath Spa University · Supervisor: Dr. John Curry  
> Framework: **E-AGPO-HT v3.1** · Strata III · 7 BGC · ~40 NOF  
> Affiliation: Auracelle AI Governance Labs · UC Berkeley CLTC Non-Resident Senior Fellow

---

## Overview

Auracelle Charlie is a browser-based, single-file wargaming simulation platform developed as a doctoral research instrument at Bath Spa University. It operationalises the **Evans Accelerated Governance Policy Optimisation — Hierarchical Theory (E-AGPO-HT)** framework to test AI governance policy outcomes through structured multi-actor simulation.

The platform enables facilitators and researchers to design and run governance negotiation sessions, capture structured move-level data, model adversarial behavior, and evaluate governance indicator trajectories — all within a single self-contained HTML file requiring no installation or server infrastructure.

---

## Research Context

**Dissertation title:** *Testing Public Policy Outcomes through War Gaming Methodologies for Strengthening AI Governance*

**Core research objectives operationalised by this instrument:**

| Objective | Charlie Implementation |
|-----------|----------------------|
| Obj 1 — Actor composition & scenario design | Session Design tab (① Setup) |
| Obj 2 — Structured move capture with rationale | Facilitator Mode (② Facilitate) |
| Obj 3 — BGC scoring across turns | BGC Full Matrix |
| Obj 4 — Governance indicator measurement | Governance Indicators tab (③) |
| Obj 5 — Resilience design principles | Red Team & Shock Injection (⑨) |
| Obj 6 — Foresight validation vs. historical cases | Foresight Validation tab (④) |
| Obj 7 — Autonomous simulation comparison | MARL Engine (⑦) + Autonomous Mode |

---

## Platform Architecture

Charlie is a **single-file HTML instrument** — all logic, styling, and data are self-contained. No build step, no dependencies, no server required.

### Tabs

| Tab | Function |
|-----|----------|
| ① Session Design | Configure scenario, actor composition, time pressure, validation case, session notes |
| ② Facilitator Mode | Log structured moves: actor, BGC domain, action type, rationale, latency, confidence |
| ③ Governance Indicators | Real-time indicator tracking: Coalition Strength, Compliance Signal, Fragmentation Risk, Legitimacy, Public Trust, Escalation Index, Institutional Resilience |
| ④ Foresight Validation | Compare simulation trajectories against historical governance cases (EU AI Act, Paris Agreement, NPT, GDPR, etc.) |
| ⑤ After-Action Review | Structured AAR export with indicator summaries, objective fulfilment, and research notes |
| ⑥ SIPRI Data | Reference SIPRI military expenditure and arms transfer data for geopolitical context |
| ⑦ MARL Engine | Multi-Agent Reinforcement Learning simulation — Q-learning and policy gradient agents under cooperative/competitive regimes |
| ⑨ Red Team & Shocks | Adversarial stress-testing: shock injection, red team agent designation with MITRE ATT&CK group attribution, compound multi-step attack chains |

### E-AGPO-HT Framework Structure

```
Stratum III   →   g-GWC (Global Wargaming Coefficient)
Stratum II    →   7 BGC (Boundary Governance Capabilities):
                  STI · SAD · ESI · NDM · SRA · IIC · ASI
                  + 4 ACC AI Factors
Stratum I     →   ~40 NOF (Negotiation Operational Factors)
```

---

## MITRE ATT&CK Integration

Tab ⑨ integrates the **MITRE ATT&CK® Enterprise and ICS matrices** as a technical threat input model beneath the E-AGPO-HT governance layer.

- **9 standard shocks** — each mapped to documented ATT&CK technique IDs and parent tactics
- **4 compound shocks** — multi-step TTP chains from named APT groups, staged over 3 simulation turns:

| Compound Shock | APT Group | Technique Chain |
|----------------|-----------|-----------------|
| Supply Chain Compromise | APT41 / Winnti | T1195.002 → T1059 → T1562.001 |
| Coordinated Influence Operation | Sandworm / VOODOO BEAR | T1583.006 → T1586.002 → T1491.002 |
| Insider Credential Exfiltration | APT29 / Cozy Bear | T1078 → T1552.001 → T1213 |
| ICS Leverage & Governance Coercion | XENOTIME / Triton | T0816 → T0826 → T0880 (ICS) |

> ATT&CK provides the adversarial input model; E-AGPO-HT remains the governance intelligence architecture. Cite as: MITRE ATT&CK® v14, mitre.org/attack.

---

## Usage

### Run locally
```bash
# No installation required — open directly in any modern browser
open index.html
```

### GitHub Pages (live demo)
The instrument is deployed via GitHub Pages. Access at:  
`https://[username].github.io/auracelle-charlie/`

### Session workflow
1. **① Session Design** — select scenario domain, actor composition, time pressure, and historical validation case
2. Click **▶ Initialise Session** — platform switches to Facilitator Mode automatically
3. **② Facilitator Mode** — log each actor move with rationale, BGC domain, action type, and confidence
4. Monitor **③ Governance Indicators** updating in real time after each turn
5. Inject **⑨ Red Team shocks** at any point to stress-test resilience
6. Run **⑦ MARL Engine** for autonomous simulation comparison (Obj 6)
7. Export session data (JSON / CSV) from the After-Action Review tab

---

## Data Export

Sessions export in two formats from the AAR tab:

- **JSON** (`charlie-[SESSION_ID].json`) — full session object including composition, scenario, all turns, and final indicator values; structured for longitudinal analysis
- **CSV** (`charlie-turns-[SESSION_ID].csv`) — turn-level data for quantitative analysis in R/Python/SPSS

---

## IP & Attribution Notice

The **E-AGPO-HT framework** (Stratum architecture, BGC taxonomy, NOF structure, and associated mathematical formalisations) is the proprietary intellectual property of Grace-Alice Evans / Auracelle AI Governance Labs. The simulation instrument is made available for academic research and institutional demonstration purposes.

**Citation:**
```
Evans, G-A. (2024). Auracelle Charlie: A Wargaming Simulation Instrument for 
AI Governance Policy Optimisation. Bath Spa University Doctoral Research Instrument. 
E-AGPO-HT v3.1. https://github.com/[username]/auracelle-charlie
```

---

## Affiliations

- **Bath Spa University** — Doctoral Research, Supervisor: Dr. John Curry
- **UC Berkeley, Center for Long-Term Cybersecurity (CLTC)** — Non-Resident Senior Fellow
- **Auracelle AI Governance Labs** — Founder & Director

---

## Related Platforms

| Platform | Focus |
|----------|-------|
| Auracelle Bach | Academic/civil society — foundational E-AGPO-HT deployment |
| Auracelle Mozart | Diplomatic/institutional — multilateral treaty language |
| Auracelle Lyra | Applied practitioner sandbox — standards stress-testing, IAEA/nuclear focus |
| Auracelle Orion | Dual-track cyber/space governance — Geneva Cyber Week 2026 |
| Auracelle Delphi | Strategic foresight — IAIG Framework |

---

*Framework version: E-AGPO-HT v3.1 · Instrument build: BSU Demo v2 · Last updated: March 2026*
