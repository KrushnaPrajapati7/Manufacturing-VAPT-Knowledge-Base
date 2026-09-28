# Manufacturing VAPT — Standards & Control Mapping Matrix

## Purpose
This matrix connects the manufacturing VAPT knowledge base to recognized frameworks and standards. It is an assessment cross-reference, **not a certification or compliance determination**. A mapping means the assessment area can provide evidence relevant to the referenced framework; it does not mean that testing alone demonstrates conformity.

## Primary baseline
- **NIST CSF 2.0** — governance and cybersecurity risk outcomes.
- **NIST SP 800-82 Rev.3** — finalized OT security guidance; the September 2026 Rev.4 publication is an initial public draft and should not replace Rev.3 as the finalized baseline.
- **NIST SP 1800-10** — manufacturing-focused integrity protection practice guide.
- **NIST SP 800-115** — technical security testing and assessment guidance.
- **ISA-95 / IEC 62264** — manufacturing/enterprise architecture and information exchange.
- **ISA/IEC 62443** — IACS cybersecurity lifecycle, zones/conduits, risk and security requirements.
- **MITRE ATT&CK for ICS** — threat-informed attack-path mapping.
- **OWASP Top 10 / API Security Top 10** — web and API application testing.
- **CWE** — weakness/root-cause classification.
- **CVSS v4.0** — vulnerability severity communication; OT safety and business impact remain separate contextual considerations.
- **CIS Controls v8.1** — prioritized enterprise safeguards.
- **ISO/IEC 27001:2022** — ISMS and risk-governance reference.

## How auditors should use it
1. Start with the asset and phase in the master matrix.
2. Use this mapping to identify relevant control objectives.
3. Execute only the tests permitted by the engagement ROE and safety gate.
4. Record observations and evidence using `16-Findings-Evidence/`.
5. Map confirmed weaknesses to CWE where useful, CVSS v4.0 where applicable, and MITRE ATT&CK for ICS where threat behavior is relevant.
6. Link findings to the applicable standard/control areas without claiming certification.
7. Retest remediation and preserve the evidence chain.

## Important distinction
**Framework mapping ≠ compliance.** An auditor should state whether an item was **Tested, Finding, Not Applicable, Out of Scope, Not Tested, or Unknown** and preserve the reason/evidence.
