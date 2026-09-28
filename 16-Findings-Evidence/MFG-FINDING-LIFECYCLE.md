# Finding Lifecycle and QA

## Lifecycle

`Observation` → `Evidence` → `Validated Finding` → `Risk Rated` → `Remediation` → `Retest` → `Closed / Risk Accepted / Further Remediation`

### 1. Observation
Record expected versus observed state and the exact scope linkage.

### 2. Evidence
Capture enough material to support the observation while minimizing sensitive data. Evidence must have an identifiable source, timestamp, handling classification, and storage reference.

### 3. Validation
A reviewer checks whether the evidence actually supports the claimed weakness, whether scope and authorization are valid, and whether scanner output has been independently contextualized where necessary.

### 4. Risk rating
Use the engagement-approved severity model. CVSS can express technical severity, while manufacturing risk must also consider production, safety, quality, recovery, engineering/IP, and business context.

### 5. Remediation
Recommendations should address root cause where feasible and identify compensating controls where immediate remediation is constrained by production or safety requirements.

### 6. Retest
Retest the original condition using an equivalent or justified alternative method. Record evidence and limitations. A changed scanner result alone is not sufficient closure evidence.

### 7. Closure / risk acceptance
Close only when the required remediation is verified or an authorized risk acceptance is documented. Preserve residual-risk information.

## QA checklist

- [ ] Finding has unique ID.
- [ ] Asset, phase, environment, and knowledge unit are linked.
- [ ] Observation is factual and reproducible where possible.
- [ ] Evidence IDs are present and traceable.
- [ ] Sensitive evidence is classified and handled appropriately.
- [ ] Safety/operational constraints are documented.
- [ ] Impact covers C/I/A and relevant manufacturing consequences.
- [ ] Severity methodology is stated.
- [ ] Root cause is distinguished from symptom.
- [ ] Recommendation is actionable and scoped.
- [ ] Owner and target date are recorded when applicable.
- [ ] Retest references the original finding.
- [ ] Residual risk is documented.
- [ ] Reviewer/approval is recorded.
