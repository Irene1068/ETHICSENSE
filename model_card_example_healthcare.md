# Digital Dignity Model Card Example (Healthcare)

## 1. Model Overview

- **Model Name:** Patient Readmission Risk Scoring Model
- **Version:** 1.0
- **Date:** 2024-08-01
- **Developer/Owner:** Regional HealthNet Analytics Team
- **Intended Use:**  
  To predict the likelihood of patient hospital readmission within 30 days, supporting clinical prioritization and care planning for adult inpatients.
- **Not Intended For:**  
  Use as the sole basis for denying care, insurance eligibility, or discharging patients without clinician review.

---

## 2. Data & Methods

- **Dataset(s) Used:**  
  Diabetes 130-US hospitals dataset (UCI Machine Learning Repository)
- **Data Collection Methods:**  
  Retrospective analysis of de-identified patient records from over 130 hospitals (1999–2008)
- **Relevant Features:**  
  Age, gender, race/ethnicity, comorbidities, prior admissions, medications, lab results
- **Potential Data Biases or Gaps:**  
  Underrepresentation of some minority groups; dataset reflects historical healthcare access disparities; social determinants not fully captured

---

## 3. Digital Dignity Assessment

- **Fairness & Equity:**  
  Model performance was evaluated across age, gender, and racial groups. Disparate impact was detected: prediction accuracy was lower for Black and Hispanic patients. Steps taken include re-sampling and algorithmic adjustments. These disparities and remediation efforts are documented for transparency.
- **Privacy & Consent:**  
  All data used was de-identified per HIPAA standards. No personally identifiable information (PII) is included. Data collection did not require explicit patient re-consent due to de-identification.
- **Transparency & Explainability:**  
  Model explanations (feature importance) are provided to clinicians via simple charts. Patients and staff receive plain-language summaries on how and why the model is used in care planning.
- **Autonomy & Respect:**  
  Model recommendations are advisory only. Clinicians retain full authority to override model outputs. Patients are informed when AI tools are used in their care, and can request more information.
- **Accountability:**  
  The Analytics Team is responsible for model maintenance. A process is in place for clinicians and patients to raise concerns or appeal decisions.

---

## 4. Limitations & Risks

- **Known Limitations:**  
  The model does not account for recent changes in care protocols or local demographic shifts. Predictive accuracy may be lower for small subgroups not well represented in the data.
- **Potential Harms:**  
  Risk of reinforcing historical disparities; risk of clinicians over-relying on model outputs
- **Uncertainty Factors:**  
  Dataset time frame (1999–2008); incomplete social determinants of health
- **Mitigation Measures Taken:**  
  Bias monitoring at regular intervals; clinician training on model interpretation; policy requiring human oversight for all major decisions

---

## 5. Monitoring & Improvement

- **Monitoring Plan:**  
  Quarterly audits of model performance and fairness metrics across demographic groups. Annual re-validation of dataset relevance.
- **Feedback Mechanisms:**  
  Feedback form for clinicians and patients provided via the hospital intranet; direct contact for urgent issues.
- **Future Improvements Planned:**  
  Incorporate more current data; expand features to better capture social determinants; partner with patient advocacy groups for ongoing review.

---

## 6. Contacts & Acknowledgments

- **Primary Contact:**  
  Jamie Patel, Data Science Lead (jamie.patel@regionalhealthnet.org)
- **Contributors:**  
  Analytics Team, Clinical Advisory Board, Patient Advocate Group
- **References / Resources:**  
  - [UCI Diabetes 130-US hospitals dataset](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
  - IBM AI Fairness 360 toolkit documentation
  - HIPAA Privacy Rule Overview

---
