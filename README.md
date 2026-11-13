# Risk-Assessment[README (2).md](https://github.com/user-attachments/files/34817516/README.2.md)
# FundPadi Enterprise Risk Assessment

**Enterprise Risk Management (ERM) | Information Security Risk Assessment | Fintech Case Study**

A portfolio project assessing information security and operational risks for **FundPadi Digital Financial Services Ltd.**, a fictional Nigerian digital financial services provider. The project uses a structured Excel workbook to identify critical assets, analyse threats and vulnerabilities, assess risks, recommend treatments, estimate financial exposure, and define key risk indicators (KRIs).

> **Portfolio disclaimer:** This is an educational, scenario-based assessment, not an audit of a real organisation. Findings, financial estimates, proposed controls and residual ratings are based on case-study inputs; they have not been independently validated or implemented.

## Project overview

**Business context:** FundPadi is a Lagos-based fintech with approximately 180 employees, 350,000 registered users and 6,500 merchants. Its services depend on a customer database, mobile application and third-party cloud infrastructure.

**Objective:** Provide management with a prioritised view of significant risks, potential financial consequences, recommended mitigations and measurable indicators for ongoing monitoring.

**Assessment scope:**

1. **Customer database security:** Privileged-access weaknesses, including administrator accounts without MFA, shared credentials and limited access monitoring.
2. **Mobile application security:** Customer authentication and monitoring weaknesses, alongside reported unauthorised-transfer complaints requiring investigation. The cause of the complaints has **not** been confirmed.
3. **Third-party cloud services:** Vendor due-diligence, contractual responsibility, availability and business-continuity risks associated with Cloudy Solutions Ltd.

## Tools and approach

- **Microsoft Excel:** Risk registers, scoring matrices, heat maps, treatment plan, financial exposure calculations, KRIs and management dashboard.
- **Risk assessment framework:** A 5 × 5 likelihood–impact matrix, informed by ISO 31000 and ISO/IEC 27001 risk-management concepts. This project does not claim formal certification or compliance verification.
- **Quantitative exposure:** Single Loss Expectancy (SLE) and Annual Loss Expectancy (ALE).

### Risk rating methodology

Risk score = **Likelihood × Impact**, with each factor scored from 1 to 5.

| Score | Rating |
|---|---|
| 1–4 | Low |
| 5–9 | Medium |
| 10–16 | High |
| 17–25 | Critical |

Under the case-study risk appetite, only **Low** risks can be accepted without further treatment. Medium, High and Critical risks require action or appropriate management authorisation.

## Key findings

| Risk ID | Risk scenario | Inherent likelihood | Inherent impact | Inherent score | Projected residual score |
|---|---|---:|---:|---:|---:|
| R-01 | Customer database | 4 | 4 | **16 — High** | **8 — Medium** |
| R-02 | Mobile application | 4 | 4 | **16 — High** | **8 — Medium** |
| R-03 | Third-party cloud provider | 4 | 4 | **16 — High** | **8 — Medium** |

**All three risks are currently assessed as High and outside risk appetite.** If the recommended controls are implemented and operate effectively, their projected likelihood falls from 4 to 2, while impact remains 4. The resulting **Medium** residual risks would **still exceed** FundPadi's Low-only risk appetite.

### Estimated financial exposure

| Scenario | Asset value | Exposure factor | SLE | Annual rate of occurrence | ALE |
|---|---:|---:|---:|---:|---:|
| Customer database | ₦50,000,000 | 60% | ₦30,000,000 | 0.5 | ₦15,000,000 |
| Mobile application | ₦30,000,000 | 40% | ₦12,000,000 | 1.5 | ₦18,000,000 |
| Third-party cloud | ₦20,000,000 | 25% | ₦5,000,000 | 2.0 | ₦10,000,000 |
| **Combined estimated ALE** | | | | | **₦43,000,000** |

**SLE = Asset Value × Exposure Factor**  
**ALE = SLE × Annual Rate of Occurrence**

The **mobile application** has the highest estimated annual exposure (**₦18 million**), while the **customer database** has the highest estimated single-event loss (**₦30 million**). The ₦43 million total assumes the estimates are additive and does not account for possible overlapping losses or all indirect impacts. These are **modelled exposures, not actual losses**.

## Recommended risk treatments

| Area | Priority actions | Accountable owner(s) |
|---|---|---|
| Customer database | Enforce administrator MFA; replace shared credentials with individual accounts; apply role-based access; review privileged access; alert on suspicious logins | Head of IT |
| Mobile application | Introduce customer MFA and login rate limiting; strengthen transaction/fraud monitoring; investigate reported unauthorised transfers | Head of Product |
| Cloud provider | Perform vendor security assessments; clarify data-sharing responsibilities; review service-level agreements; test continuity and contingency arrangements | Heads of IT and Procurement |

These actions are **recommendations**, not evidence that controls have been deployed.

## Key risk indicators

The workbook proposes **six KRIs**, two for each scenario:

| Area | KRI | Proposed trigger | Frequency |
|---|---|---|---|
| Database | Administrator accounts without MFA | > 0% | Weekly |
| Database | Suspicious administrator logins | ≥ 3 in 24 hours | Daily |
| Mobile | Reported unauthorised transfers | > 5 complaints in 7 days | Weekly |
| Mobile | Customer accounts without MFA | > 5% after rollout deadline | Weekly |
| Cloud | Unplanned service downtime | > 30 minutes/month | Monthly |
| Cloud | Overdue vendor security assessments | ≥ 1 overdue | Monthly |

Thresholds are **proposed for management review**, not confirmed approved operating limits.

## Workbook structure

The accompanying **`FundPadi Enterprise Risk Assessment.xlsx`** contains 12 worksheets:

| Worksheet | Purpose |
|---|---|
| Document Control | Project metadata and document classification |
| Risk Assessment Methodology | Likelihood–impact matrix and assessment criteria |
| Asset Register | Critical assets, ownership, classification and business impact |
| Threat & Vulnerability | Threats, weaknesses, risk events and consequences |
| Treatment Plan | Recommended mitigations, dependencies and priorities |
| Risk Register | Risk statements and inherent assessments |
| Inherent Risk Heat Map | Visualisation of inherent risk scores |
| Residual Risk | Projected post-treatment ratings and appetite comparison |
| Residual Risk Heat Map | Visualisation of projected residual risk |
| Financial Exposure | SLE, ARO and ALE calculations |
| KRI Register | Proposed indicators, thresholds and monitoring cadence |
| Dashboard | Summary of assessed risks by severity |

## How to explore the project

1. Open **`FundPadi Enterprise Risk Assessment.xlsx`** in Microsoft Excel.
2. Start with the **Dashboard** for the overall risk position.
3. Review the **Risk Register** and **Inherent Risk Heat Map** to understand the three High risks.
4. Open the **Treatment Plan** and **Residual Risk** sheets to see recommended actions and projected outcomes.
5. Review **Financial Exposure** for estimated losses and **KRI Register** for proposed monitoring metrics.

## Skills demonstrated

- Information security and enterprise risk identification
- Asset classification and threat/vulnerability analysis
- Likelihood–impact scoring and risk heat-map development
- Risk treatment planning and residual-risk assessment
- Quantitative financial risk estimation using SLE and ALE
- KRI design, monitoring thresholds and risk reporting
- Excel-based risk documentation and management dashboards

## Limitations and next steps

This assessment is based on supplied case-study scenarios rather than verified technical evidence. Residual scores are **forecasts**, not measured outcomes. Further work would include validating assumptions with system owners, investigating the reported mobile-transfer incidents, confirming controls through testing, approving KRI thresholds, assigning implementation deadlines and reviewing whether residual risks can be reduced to within appetite.

---

**Project type:** Portfolio case study  
**Organisation assessed:** FundPadi Digital Financial Services Ltd. (fictional)  
**Primary deliverable:** Excel-based enterprise risk assessment workbook
