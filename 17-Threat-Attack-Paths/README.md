# 17 — Threat, Attack Paths & MITRE ATT&CK for ICS

## Purpose
This layer adds adversary-oriented reasoning to the Manufacturing VAPT Knowledge Base while preserving the complete asset and phase scope. It helps auditors connect individual findings into realistic attack paths and business/plant consequences.

## Files
- `MFG-MITRE-ICS-TACTIC-CATALOG.csv` — 12 current MITRE ATT&CK for ICS tactics.
- `MFG-MITRE-ICS-TECHNIQUE-CATALOG.csv` — manufacturing-relevant MITRE ICS techniques/sub-techniques used by this KB.
- `MFG-ATTACK-PATH-CATALOG.csv` — 40 reusable manufacturing attack-path scenarios.
- `MFG-ASSET-THREAT-ATTACK-MAPPING.csv` — coverage for all 406 assets.
- `MFG-THREAT-ATTACK-PATH-MATRIX.md` — human-readable path matrix.
- `MFG-THREAT-ATTACK-PATH-ASSESSMENT-METHODOLOGY.md` — assessment, safety, evidence and reporting methodology.
- `MFG-THREAT-MAPPING-QA-REPORT.md` — coverage and consistency checks.

## Important boundary
ATT&CK describes adversary behavior. It does not mean every technique should be actively executed during a VAPT. Production OT testing remains constrained by authorization, ROE, plant operations, safety, quality and recovery requirements.

## Authoritative references
- MITRE ATT&CK for ICS Matrix: https://attack.mitre.org/matrices/ics/
- MITRE ICS Techniques: https://attack.mitre.org/techniques/ics/
- MITRE ICS Assets: https://attack.mitre.org/assets/
- NIST SP 800-82 Rev.3: https://csrc.nist.gov/pubs/sp/800/82/r3/final
