# MFG RAG Query Routing

| Query signal | Primary retrieval | Secondary expansion |
|---|---|---|
| Asset name | Asset index | phases, KUs, tools, threats, standards |
| Phase name | Knowledge index | assets, tools, findings |
| Tool name | Tool/test mapping | assets, phases, KUs |
| Standard/control | Standards mapping | KUs, assets, evidence |
| MITRE ICS technique | Threat mapping | assets, attack paths, KUs |
| Finding/evidence | Finding schemas | remediation, retest, standards |
| Safety/OT | Safety-aware KUs | assets, threats, stop conditions |
| Broad scope | Master asset index | all linked layers |

## Example
Question: “Assess a PLC safely.”

Route: asset=PLC → OT/ICS phase → applicable KUs → tool/test mappings → MITRE/attack paths → standards → evidence/finding schema → safety gate.
