# Clinical Specialty Pharmacist
# Data Scientist
#### Clinical Background
- Board Certified Pharmacotherapy Specialist (BCPS)
- Board Certified Oncology Pharmacist (BCOP)
- Certified Specialty Pharmacist (CSP; specialty pharmacy practice)
- Licensed Pharmacist in 16 U.S. states (active, in good standing)

#### Technical Skills
- Python, R, PyTorch; machine learning & deep learning (model development, tuning, evaluation)
- Large Language Models: domain-specific fine-tuning, instruction design, LoRA, evaluation

## Education
- Master of Science in Data Science, University of Virginia (in progress)
- Doctor of Pharmacy (PharmD), University of Florida College of Pharmacy
- Master of Science in Pharmacy, Seoul National University College of Pharmacy, South Korea
- Bachelor of Pharmacy, Ewha Women’s University College of Pharmacy, South Korea

## Professional Activity

**Data Science & Applied Artificial Intelligence in Medicine**
- Applied use of R and Python for statistical analysis, machine learning, deep learning, and large language model development
- Medical Intelligence Society (MIS) member: participation in U.S. data science workshops, monthly meetings, and weekly office-hour discussion groups
- mCODE (Minimal Common Oncology Data Elements) Community member: engagement in use-case projects focused on applying mCODE standards to support third-party reimbursement and interoperability
  
**Pharmacy & Clinical Professional Societies**
- Society of Hematologic Oncology (SOHO) - member
- Florida Society of Clinical Oncology (FLASCO) - member
- Hematology/Oncology Pharmacy Association (HOPA) - member
- National Association of Specialty Pharmacy (NASP) - member

## Projects
### Machine Learning Predictive Models on Early Discontinuation of Rheumatoid Arthritis Therapy, Adalimumab

<details open>

<summary><strong>Retrospective Observational Study(completed | 2023-2025)</strong></summary>

Accepted for publication in JMCP (November, 2025)<br>
Early discontinuation of adalimumab remains a challenge among patients with rheumatoid arthritis, yet identifying high-risk patients at treatment initiation is difficult in routine practice. Using real-world data from 300 RA patients, we developed predictive models based on baseline clinical and patient-reported features available at specialty pharmacy service initiation. Among multiple approaches evaluated, elastic net–regularized logistic regression achieved the best performance (ROC-AUC = 0.886; F1 = 0.741), demonstrating that interpretable models can effectively identify patients at risk for early discontinuation and support targeted pharmacist-led interventions.

</details>

[GitHub Link](https://github.com/baicalein/ML-Predictive-Models-on-Early-Discontinuation-of-Adalimumab-in-RA)

<details open>

<summary><strong>Prospective Observational Validation Study(2025 - Present)</strong></summary>

Abstract accepted at AIMed25 (November 9–12, 2025)<br>
This prospective study will evaluate the generalizability and real-world performance of previously developed machine learning models in a new cohort of patients with rheumatoid arthritis initiating adalimumab, with follow-up for at least nine months. Model interpretability will be assessed using SHAP to generate individualized risk explanations, which will be reviewed by clinical pharmacists for usability and clinical relevance. The study will also examine the impact of advanced imputation methods, including MICE and k-nearest neighbors, on model calibration and stability in a prospective setting.

</details>

<br>

### PA LLM: Large Language Model for Prior Authorization Review, Adalimumab for Rheumatoid Arthritis
Developing a domain-specific Large Language Model (LLM) to support prior authorization (PA) review for adalimumab in rheumatoid arthritis (RA), grounded in FDA-approved indications and payer-specific clinical criteria. The goal of this project is to reduce pharmacist workload in PA review while preserving clinical accuracy, regulatory compliance, and decision transparency.

<details open>

<summary><strong>Prototype(Completed | 2025)</strong></summary>

The prototype fine-tunes a lightweight Llama-3.2–1B-Instruct backbone using LoRA for parameter-efficient adaptation, trained on synthetic patient summaries representing common rheumatoid arthritis prior authorization scenarios paired with structured JSON outputs aligned with real specialty pharmacy workflows (diagnosis verification, step therapy assessment, safety screening, dosing confirmation, and decision rationale). A carefully designed instruction–response schema mirrors real PA review processes, and model performance is evaluated using an LLM-as-a-judge framework with GPT-5 as a reference model, alongside external benchmarking on MedMCQA, MMLU, and RACE to assess generalizability beyond the PA task. This prototype demonstrates the feasibility of deploying a small, efficient LLM to support structured clinical decision review in high-stakes administrative healthcare settings.

</details>

[HuggingFace Link](https://huggingface.co/baicalein/paLLM_adalimumab_RA_Lora)

<details open>

<summary><strong>Scale-Up Phase(2026 - Present)</strong></summary>

The current phase focuses on scaling the prototype into a more realistic and clinically grounded system, moving beyond a proof-of-concept toward evaluation under real-world prior authorization conditions. This includes testing model behavior against imperfect and challenging documentation commonly seen in practice, such as incomplete notes, ambiguous wording, and edge cases. Planned enhancements include expanding synthetic chart notes to better reflect real clinical documentation with varied formats, lengths, and provider writing styles, as well as incorporating multiple experienced pharmacists into the LLM-as-a-judge evaluation process to reduce individual reviewer bias and improve consistency. The project will also explore preference-based alignment methods to better capture true pharmacist reasoning rather than simple rule or policy matching.

</details>

<br>

### Melanoma Detection using Knowledge Distillation and Mobile Phone

<details open>

<summary><strong>Melanoma Detection App (Completed | 2025)</strong></summary>

This project investigates knowledge distillation (KD) as a strategy to enable accurate melanoma detection on resource-constrained mobile and edge devices, where traditional deep convolutional neural networks are impractical due to computational and memory limitations. Using the HAM10000 dermoscopy dataset, we trained a compact MobileNetV3-Small student model (9.1 MB) to learn from larger, high-capacity teacher models (EfficientNet-B1 and ResNet-based architectures). Through systematic exploration of KD design choices—including temperature scaling, distillation loss mixing ratios, pooling strategies, and focal loss for class imbalance—the distilled student model achieved strong diagnostic performance while maintaining efficiency. The best student model reached a ROC-AUC of 0.921 with Expected Calibration Error (ECE) of 0.072, surpassing teacher models in discrimination while retaining excellent calibration. Beyond compression, the results demonstrate that KD acts as an effective regularizer, enabling the student to generalize well despite substantially fewer parameters. The project emphasizes edge-ready deployment, model calibration, and high sensitivity for rare melanoma cases, supporting realistic use in offline, on-device skin cancer screening applications where internet access and compute resources are limited.

</details>

[GitHub Link](https://github.com/rah-ds/Deep_Learning_Final_Project/tree/main)

### Digital Health in Emergency Care: LLMs for Diagnostic Excellence: Capstone Project

<details open>

<summary><strong>ER Digital Health (In progress | 2025-2026)</strong></summary>

Design and evaluation of LLM-based clinical decision support to improve diagnostic reasoning, reduce diagnostic error, and enhance quality and safety in emergency care, using ~100,000 de-identified ED clinical notes. Hands-on work with FHIR-based EHR data as part of a UVA Emergency Medicine digital health initiative, supporting interoperable analytics across emergency, urgent care, and ambulatory settings.

</details>

<br>

### Interdisciplinary Project: Exercise Science–Informed Interventions for Rheumatoid Arthritis

<details open>

<summary><strong>Personal Trainer for RA (In Preparation)</strong></summary>

Interdisciplinary project integrating exercise science, clinical pharmacy, and data science, including collaboration with certified personal trainers (ACSM-CPTs) and use of real-world trainer-collected data to inform lifestyle-based interventions for patients with rheumatoid arthritis.
Planned development of a mobile health application to deliver personalized exercise programs and support PT–trainee communication (one-on-one and group-based), with optional participation of healthcare providers (e.g., clinical pharmacists) for RA patients who consent to referral-based care coordination.

</details>

<br>

### Precision Medicine Project

<details open>

<summary><strong>Precision Medicine: Genetic Test(2022-2023)</strong></summary>

- Provided consultative support to healthcare providers and patients in the Oncology Precision Medicine Program, advising on genomic testing (BostonGene) to guide treatment planning in collaboration with Welldyne Specialty Pharmacy
- Authored a 2022 congress summary for the International Society of Liquid Biopsy, published on the Hematology and Oncology Pharmacy Association (HOPA) website as part of the organization’s meeting resource summaries
- Supported the Psoriasis and Rheumatoid Arthritis Precision Medicine Program, consulting on the use of MindPx and PrismRA diagnostic tests to optimize biologic selection and improve patient outcomes in partnership with Welldyne Specialty Pharmacy

</details>

<br>

## Work Experience
**Clinical Pharmacist @ Healthdyne Specialty Pharmacy (formerly Welldyne Specialty Pharmacy)**  (_2019 – present, full time_)
- Clinical patient management across oncology, autoimmune inflammatory diseases, hepatitis B/C, HIV, and multiple sclerosis
- Active involvement in URAC and ACHC accreditation preparation, audits, and quality compliance
- Oncology precision medicine program utilizing BostonGene molecular profiling to support treatment decisions
- Psoriasis and rheumatoid arthritis precision medicine programs incorporating MindPx and PrismRA testing
- Medical specialty program development and operational management
- Participation in oncology clinical pathway programs to support evidence-based therapy selection

**Staff Pharmacist @ CareMed Rx**  (_2015 – present, part time_)
- Sterile compounding of chemotherapy agents and intravenous antibiotics
- Clinical consultation on pharmacotherapy in home infusion and outpatient infusion settings

**Clinical Pharmacist @ Quality Specialty Pharmacy**  (_2016 – 2019_)
- Clinical management of patients with oncology, autoimmune inflammatory diseases, hepatitis C, and HIV
- Delivery of Medication Therapy Management (MTM) services through OutcomeMTM and Mirixa platforms
- Support of Medicare Star Rating performance initiatives for chronic disease management

**Staff Pharmacist @ MacDill Pharmacy**  (_2014 – 2016_)
- Clinical patient management in oncology and dermatology
- Pharmacotherapy consultation for long-term care and assisted living facilities

## License and Certification
**Data Science & Artificial Intelligence**
- Artificial Intelligence in Medicine – Advanced Certificate, American Board of Artificial Intelligence in Medicine (ABAIM)
- Artificial Intelligence in Medicine – Educational Certificate, American Board of Artificial Intelligence in Medicine (ABAIM)

**Pharmacy & Clinical Practice**
- Pharmacist Licensure: Alabama, Arkansas, Florida, Indiana, Kansas, Kentucky, Louisiana, Maryland, Michigan, Mississippi, Nebraska, Oklahoma, Tennessee, Texas, Virginia, West Virginia (Active, in good standing)
- Hematopoietic Cell Transplantation Training Certificate, American Society for Transplantation and Cellular Therapy (ASTCT)
- Precision Medicine in Oncology Genomics Certificate, American College of Clinical Pharmacy (ACCP)
- Board Certified Oncology Pharmacist (BCOP), Board of Pharmacy Specialties (BPS)
- Board Certified Pharmacotherapy Specialist (BCPS), Board of Pharmacy Specialties (BPS)
- Certified Specialty Pharmacist (CSP), National Association of Specialty Pharmacy (NASP)
- Advanced Sterile Product Preparation Training Certificate, American Society of Health-System Pharmacists (ASHP)
- Pharmacist Diabetes Care Certificate, American Society of Health-System Pharmacists (ASHP)
- Medication Therapy Management Certificate, American Pharmacists Association (APhA)

## Publication
1. Yoon, AH., Oelofsen, M., Skomo, D., Page, N. Prospective Validation and Enhancement of a Machine Learning Model for Predicting Early Adalimumab Discontinuation in RA Patients Using Specialty Pharmacy Data. AIMed25 Abstract, November 9-12, 2025. [Link](https://aimed.swoogo.com/AIMed25)
2. Yoon, AH., Gedeck, P., Oelofsen, M. Predicting Early Discontinuation of Adalimumab in Rheumatoid Arthritis Patients Using Machine Learning: A Specialty Pharmacy-Based Approach. Journal of Managed Care & Specialty Pharmacy, Accepted November 26, 2025, to be published. 
3. Yoon, AH. International Society of Liquid Biopsy Annual Congress 2022 summary, Hematology and Oncology Pharmacy Association (HOPA) [Link](https://www.hoparx.org/resources/summaries-of-allied-organization-meetings/international-society-of-liquid-biopsy-annual-congress-2022/)
4. Yoon, H., Kim, HK., Ma, CJ., Huh, H. Induced accumulation of triterpenoids in _Scutellaria baicalensis_ suspension cultures using a yeast elicitor. Biotechnology Letters 22:1071-1075, 2000. [Link](https://link.springer.com/article/10.1023/A:1005610400511)
