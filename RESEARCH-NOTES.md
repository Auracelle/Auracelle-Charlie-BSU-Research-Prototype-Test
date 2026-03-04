# Research Notes

This folder is a placeholder for:
- Scenario packs and inject libraries
- Measurement model notes (indicators, coding schemes)
- AAR rubric templates


## MITRE ATT&CK Integration (v0.2.0)

### Architecture
ATT&CK is layered **beneath** the E-AGPO-HT governance framework as the technical threat input model. It provides a peer-reviewed, citable taxonomy for classifying adversarial behavior within the governance negotiation simulation. The E-AGPO-HT framework (Strata III, 7 BGC, ~40 NOF) is preserved intact.

### Technique mapping
Each shock event in Tab ⑨ is tagged with the most relevant ATT&CK technique(s) from the Enterprise matrix (v14):

| Shock | Techniques | Tactics |
|---|---|---|
| Data Breach Disclosure | T1530, T1078 | TA0010, TA0006 |
| Unilateral Withdrawal | T1657, T1489 | TA0040 |
| Classified Leak | T1552, T1213 | TA0009, TA0010 |
| AI Incident Event | T1499, T1565 | TA0040 |
| Sanctions Imposed | T1657, T1491 | TA0040 |
| Public Legitimacy Crisis | T1491.002, T1059 | TA0040 |
| Industry Defection | T1489, T1485 | TA0040 |
| Great Power Veto | T1498, T1583 | TA0040, TA0042 |
| Cyberattack on Process | T1498, T1499, T1046 | TA0040, TA0043 |

### Compound shocks
Four multi-step adversarial chains model documented APT group TTPs:

1. **Supply Chain Compromise** (APT41 / Winnti) — T1195.002 → T1059 → T1562.001
2. **Coordinated Influence Operation** (Sandworm / VOODOO BEAR) — T1583.006 → T1586.002 → T1491.002
3. **Insider Credential Exfiltration** (APT29 / Cozy Bear) — T1078 → T1552.001 → T1213
4. **ICS Leverage & Governance Coercion** (XENOTIME / Triton) — T0816 → T0826 → T0880 *(ICS matrix)*

The ICS compound shock is notable for producing a *coerced compliance* signature (compDelta positive in Stage 3) rather than compliance collapse — a distinct governance indicator pattern relevant to Objective 5 design principles analysis.

### Citation
MITRE ATT&CK® v14. The MITRE Corporation. https://attack.mitre.org/
