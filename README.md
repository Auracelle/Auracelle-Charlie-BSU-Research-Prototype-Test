# Auracelle Charlie — BSU Doctoral Research Instrument

**PI:** Grace-Alice Evans · Bath Spa University · Auracelle AI Governance Labs
**Supervisor:** Dr. John Curry, Bath Spa University
**Framework:** E-AGPO-HT v3.1 (Evans-Accelerated Governance Policy Optimisation — Hierarchical Theory)
**Affiliation:** Non-Resident Senior Fellow, UC Berkeley Center for Long-Term Cybersecurity (CLTC)

---

## What this is

Auracelle Charlie is a browser-based governance wargaming simulation instrument built for doctoral research into AI governance policy outcomes. It operationalises the E-AGPO-HT framework as a structured multi-actor negotiation environment, enabling facilitated and autonomous simulation sessions with full data capture for qualitative and quantitative analysis.

The instrument is a single-file HTML application — no build step, no server required, no external dependencies beyond Google Fonts and the optional Anthropic API for agentic features.

---

## Capability overview

| Tab | Function |
|-----|----------|
| ① Session Design | Participant composition, scenario domain, round arc, stress-test use-case |
| ② Facilitator Mode | Live turn logging, round deliverable capture, Policy Owner always-on panel |
| ③ Governance Indicators | Real-time E-AGPO-HT indicator dashboard (8 indicators, 7 BGC scores) |
| ④ Foresight Validation | Simulated vs. historical case comparison (EU AI Act, NIST AI RMF, CCW GGE, AUKUS, GDPR) |
| ⑤ After-Action Review | Structured AAR generation, qualitative coding prompts, JSON/CSV export |
| ⑥ SIPRI Data | Military expenditure context feed mapped to BGC parameters |
| ⑦ MARL Engine | Multi-Agent Reinforcement Learning — Q-learning, Stackelberg dynamics, EGT |
| ⑧ Autonomous Sim | Goal-directed autonomous session — three-way Human / AI / Historical comparison |
| ⑨ Red Team & Shocks | Shock injection library, MITRE ATT&CK compound chains (APT41, Sandworm, APT29, XENOTIME) |
| ⑩ Agentic AI | LLM-backed Policy Owner (always-on) + Agentic Red Team via Anthropic API |

---

## Quick start

### Option A — open locally (simplest)
1. Download or clone this repository.
2. Open `index.html` in Chrome, Edge, or Firefox.
3. No installation required.

### Option B — serve locally (recommended)
Some browsers restrict local file APIs when opening HTML directly from disk. For consistent behaviour:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080` in your browser.

### Option C — GitHub Pages
This repository is configured for GitHub Pages deployment. Enable Pages in your repository settings pointing to the `main` branch root, and the instrument will be available at your Pages URL.

---

## Agentic AI features (Tab ⑩)

The Policy Owner and Agentic Red Team features require an Anthropic API key. The key is:
- Entered once per browser session in Tab ⑩
- Stored only in browser session memory
- Never persisted to disk or transmitted beyond `api.anthropic.com`

To obtain an API key: [console.anthropic.com](https://console.anthropic.com)

Model used: `claude-sonnet-4-20250514`

---

## Session workflow

1. **Tab ①** — Select participant composition group, scenario domain, and stress-test use-case. Choose a round arc (Governance Negotiation, Crisis Response, or Standards Setting) or free-form.
2. **Tab ②** — Run the session. Log participant moves, capture round deliverables (text and/or attached documents), advance rounds. The Policy Owner panel issues governance challenges automatically each round.
3. **Tab ③** — Monitor live governance indicators during the session.
4. **Tab ⑨** — Inject shocks or fire compound ATT&CK chains to stress-test framework resilience.
5. **Tab ⑤** — Generate After-Action Review, export JSON/CSV for analysis.

---

## Round arcs

Three structured deliverable frameworks are available:

**Governance Negotiation Arc (6 rounds)**
Position Declaration → Policy Need → Coalition Signal → Counter or Comply → Shock Response → Final Governance Outcome

**Crisis Response Arc (4 rounds)**
Threat Assessment → Emergency Mechanism Proposal → Coalition Commitment → Crisis Resolution

**Standards Setting Arc (6 rounds)**
Problem Framing → Technical Requirements → Draft Standard → Objections & Amendments → Compliance Commitment → Final Adoption

Each round opens a deliverable submission zone with role-differentiated prompts per actor type (state, institution, civil society, industry). Text and document attachments are both supported. Submissions are logged and exportable as CSV.

---

## Research framework

All sessions are logged against the **E-AGPO-HT framework**:

- **g-GWC** — General Governance Wargaming Capacity index
- **7 BGC** — Broad Governance Capabilities (STI, SAD, ESI, NDM, SRA, IIC, ASI)
- **8 governance indicators** — Coalition Strength, Compliance Probability, Legitimacy Score, Fragmentation Index, Decision Latency, Escalation Index, Public Trust, Institutional Resilience

Session data exports include full turn logs, indicator trajectories, BGC scores, AAR text, and qualitative coding prompts aligned to research objectives 3, 4, and 6.

---

## MITRE ATT&CK integration

Tab ⑨ includes compound shock chains mapped to the MITRE ATT&CK Enterprise and ICS matrices:

- **APT41 / Winnti** — Supply Chain Compromise (T1195.002)
- **Sandworm / VOODOO BEAR** — Coordinated Influence Operation (T1583.006, T1586.002)
- **APT29 / Cozy Bear** — Insider Credential Exfiltration (T1078, T1552.001)
- **XENOTIME / Triton** — ICS Leverage & Governance Coercion (T0816, T0826, T0880)

Citation: MITRE ATT&CK® v14 — [mitre.org/attack](https://attack.mitre.org)

---

## Files

```
index.html                  Main application (single-file, no build)
README.md                   This file
CITATION.cff                Academic citation metadata
CHANGELOG.md                Version history
CONTRIBUTING.md             Contribution guidelines
CODE_OF_CONDUCT.md          Community standards
SECURITY.md                 Vulnerability reporting policy
LICENSE                     MIT License
docs/
  ETHICS.md                 Responsible use guidance
  RESEARCH-NOTES.md         Scenario packs, measurement notes
  FACILITATOR-GUIDE.md      Workshop facilitation guide
.github/
  ISSUE_TEMPLATE/           Bug report and feature request templates
  workflows/                GitHub Pages deployment workflow
```

---

## Citation

Please cite this instrument using the metadata in `CITATION.cff` or:

> Evans, G-A. (2026). *Auracelle Charlie: A Governance Wargaming Research Instrument* (v0.4.0). Bath Spa University / Auracelle AI Governance Labs. https://github.com/auracelle/auracelle-charlie-bsu-sandbox

---

## License

MIT License. See [LICENSE](LICENSE).

## Contact

**Grace-Alice Evans**
Founder & Principal Investigator, Auracelle AI Governance Labs
Doctoral Candidate, Bath Spa University
Non-Resident Senior Fellow, UC Berkeley CLTC
LinkedIn: [grace-alice-evans-5a9632a3](https://www.linkedin.com/in/grace-alice-evans-5a9632a3)
Platform: [Auracelle AI Governance Labs](https://auracelle.github.io/Auracelle-AI-Governance-Labs-Platform-Comms-Public)
