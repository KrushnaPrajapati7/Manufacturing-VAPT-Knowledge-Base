# Manufacturing VAPT Knowledge Architecture

The repository uses two dimensions:

## VAPT phases
1. Reconnaissance
2. Scanning & Enumeration
3. Vulnerability Assessment
4. Identity / Authentication / Authorization
5. Web / API / Application / Infrastructure
6. Internal / OT / ICS
7. Validation / Business Impact
8. Reporting / Remediation / Retest

## Cross-cutting domains
- Foundation
- Engineering / IIoT / Cloud
- Network / Remote / Supply Chain
- Data / Privacy / IP
- Monitoring / Detection

An asset can participate in multiple phases. For example, an ERP can be discovered during recon, enumerated during scanning, assessed for vulnerabilities, tested for authentication/authorization, assessed at the application/API layer, and then mapped to business impact and reporting.

This prevents the knowledge base from incorrectly treating an asset and a VAPT phase as the same dimension.


## Master retrieval matrix
The authoritative asset-to-phase-to-knowledge cross-reference is `MFG-MASTER-ASSET-VAPT-KNOWLEDGE-MATRIX.csv` with a human-readable Markdown companion. It maps all 406 taxonomy entries to applicable VAPT phases, retrieval candidate knowledge units, standards, assessment mode, prerequisites and expected evidence.
