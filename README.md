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
- Master of Science Candidate, Data Science @ University of Virginia
- Doctor of Pharmacy @ University of Florida, College of Pharmacy								       		
- Master of Science, Pharmacy	@ Seoul National University, College of Pharmacy	 			        		
- Bachelor of Pharmacy @ Ewha Women's University, College of Pharmacy

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

## Project
**Machine Learning Predictive Models on Early Discontinuation of Rheumatoid Arthritis Therapy, Adalimumab** (_2023 - Present_)
- **Retrospective Observational Study** (_2023 - 2025_) Accepted for publication in JMCP [GitHub Link](https://github.com/baicalein/ML-Predictive-Models-on-Early-Discontinuation-of-Adalimumab-in-RA)
  - Patients with rheumatoid arthritis (RA) initiating adalimumab may discontinue therapy within six months due to loss of efficacy or lack of perceived benefit. Specialty pharmacies are well positioned to intervene early, yet reliably identifying patients at high risk for early discontinuation at treatment initiation remains a clinical challenge.
  - We analyzed real-world data from RA patients who initiated adalimumab between 2020 and 2023. A total of 300 patients met inclusion criteria, with 37.7% experiencing early discontinuation. Nineteen baseline features derived from clinical characteristics and patient-reported data—including symptom severity and therapy type—were used to build predictive models using information available at clinical service initiation.
  - We developed and evaluated a diverse set of models, including linear discriminant analysis (LDA), elastic net–regularized logistic regression, support vector machines (linear, polynomial, and RBF kernels), random forest, k-nearest neighbors, and extreme gradient boosting (XGBoost). Model hyperparameters were optimized using Bayesian optimization or grid search to maximize ROC-AUC, with decision thresholds selected to optimize F1 score, reflecting the clinical need to balance sensitivity and precision.
  - On the held-out test set, the Elastic Net model achieved the strongest performance (ROC-AUC = 0.886; F1 = 0.741), followed closely by LDA and SVM, demonstrating consistent and robust discrimination across linear models. These results show that parsimonious, interpretable models can effectively identify patients at high risk for early adalimumab discontinuation using routinely available baseline data, supporting targeted pharmacist-led interventions in specialty pharmacy practice.
- **Prospective Observational Validation Study** (_2025 - Present_) Abstract accepted at AIMed25 (November 9–12, 2025):
  - Designed to assess the generalizability and real-world performance of previously developed machine learning models in a new cohort of patients with rheumatoid arthritis initiating adalimumab between September 2025 and August 2026. Patients will be followed for a minimum of nine months after treatment initiation.
  - To enhance clinical interpretability, SHapley Additive exPlanations (SHAP) will be applied to the best-performing predictive model to generate individualized risk explanations. These explanations will be reviewed by experienced clinical pharmacists to assess usability, interpretability, and clinical relevance in real-world specialty pharmacy workflows.
  - In parallel, the study will evaluate the impact of advanced missing-data handling strategies, including Multivariate Imputation by Chained Equations (MICE) and k-nearest neighbors (kNN) imputation, on model calibration, discrimination, and stability in a prospective setting.

**PA LLM: Large Language Model for Prior Authorization Review, Adalimumab for Rheumatoid Arthritis** (_2025 - Present_) 
- **Prototype & Ongoing Scale-Up**: Developing a domain-specific Large Language Model (LLM) to support prior authorization (PA) review for adalimumab in rheumatoid arthritis (RA), grounded in FDA-approved indications and payer-specific clinical criteria. The goal of this project is to reduce pharmacist workload in PA review while preserving clinical accuracy, regulatory compliance, and decision transparency.
- **Prototype** (Completed): The model fine-tunes a lightweight Llama-3.2–1B-Instruct backbone using LoRA for parameter-efficient adaptation. Training data consisted of synthetic patient summaries reflecting common RA PA scenarios, paired with structured JSON outputs aligned with real pharmacy workflows (diagnosis verification, step therapy assessment, safety screening, dosing confirmation, decision, and rationale). This prototype demonstrates the feasibility of a small, efficient LLM supporting structured clinical decision review in a high-stakes administrative healthcare setting. Key prototype features include: [HuggingFace Link](https://huggingface.co/baicalein/paLLM_adalimumab_RA_Lora)
  - A carefully designed instruction–response schema mirroring specialty pharmacy PA review processes
  - Use of synthetic clinical summaries to avoid PHI while encoding domain knowledge
  - Evaluation via LLM-as-a-judge, using GPT-5 as a reference model
  - External benchmarking on MedMCQA, MMLU, and RACE to assess generalizability beyond the PA task
- **Scale-Up Phase** (In Progress): The current phase focuses on scaling the prototype toward a more realistic, robust, and clinically grounded system. This scale-up phase aims to move beyond proof-of-concept toward a clinically realistic evaluation setting, where model behavior is stress-tested against nuanced, imperfect, and adversarial documentation scenarios. Planned enhancements include:
  - Expanded synthetic chart notes that more closely resemble real-world clinical documentation, incorporating: 1. Variable note lengths and formats, 2. Diverse writing styles across providers, 3. Ambiguous, edge-case, and incomplete documentation commonly encountered in PA workflows.
  - Multi-annotator LLM-as-a-judge optimization, engaging multiple experienced pharmacists with PA and specialty pharmacy backgrounds in RA care to: 1. Provide expert preference judgments, 2. Reduce single-reviewer bias, 3. Improve reliability and consistency of model evaluation
  - Exploration of advanced preference-based alignment techniques to better reflect pharmacist reasoning rather than surface-level policy matching

**Melanoma Detection using Knowledge Distillation and Mobile Phone** [GitHub Link](https://github.com/rah-ds/Deep_Learning_Final_Project/tree/main) (_2025_)
- This project investigates knowledge distillation (KD) as a strategy to enable accurate melanoma detection on resource-constrained mobile and edge devices, where traditional deep convolutional neural networks are impractical due to computational and memory limitations. Using the HAM10000 dermoscopy dataset, we trained a compact MobileNetV3-Small student model (9.1 MB) to learn from larger, high-capacity teacher models (EfficientNet-B1 and ResNet-based architectures).
- Through systematic exploration of KD design choices—including temperature scaling, distillation loss mixing ratios, pooling strategies, and focal loss for class imbalance—the distilled student model achieved strong diagnostic performance while maintaining efficiency. The best student model reached a ROC-AUC of 0.921 with Expected Calibration Error (ECE) of 0.072, surpassing teacher models in discrimination while retaining excellent calibration.
- Beyond compression, the results demonstrate that KD acts as an effective regularizer, enabling the student to generalize well despite substantially fewer parameters. The project emphasizes edge-ready deployment, model calibration, and high sensitivity for rare melanoma cases, supporting realistic use in offline, on-device skin cancer screening applications where internet access and compute resources are limited.
  
**Digital Health in Emergency Care: LLMs for Diagnostic Excellence** Capstone Project (In Progress | 2025–2026)
- Design and evaluation of LLM-based clinical decision support to improve diagnostic reasoning, reduce diagnostic error, and enhance quality and safety in emergency care, using ~100,000 de-identified ED clinical notes.
- Hands-on work with FHIR-based EHR data as part of a UVA Emergency Medicine digital health initiative, supporting interoperable analytics across emergency, urgent care, and ambulatory settings.
  
**PBM GLP-1 Optimizer: Predictive Model for Clinical Obesity Management** (_planning_)
- This project focuses on developing a specialized deep learning model, the PBM GLP-1 Optimizer, to improve the management of GLP-1 receptor agonist therapy for patients with clinical obesity, excluding those with a diabetes diagnosis. By applying advanced predictive analytics to a comprehensive dataset of claims and prior-authorization records, this tool aims to optimize drug utilization, enhance member outcomes, and ensure a fiscally responsible approach to these high-cost therapies.
- High-Value Candidate Identification: The model will identify patients who are most likely to achieve and sustain the clinical goals of GLP-1 therapy. This will allow for more accurate and data-driven prior authorization approvals, ensuring that the PBM's investment is directed toward members who are most likely to benefit. This approach helps to improve member outcomes while also managing costs effectively.
- Real-Time Utilization Management: By integrating with the PBM's pharmacy claims and prior authorization systems, the model can provide real-time insights during the PA review process. It will flag cases that are most likely to be high-responders or high-risk for discontinuation, enabling faster and more accurate approval decisions.

**Precision Medicine Project** (_2022 - 2023_)
- Provided consultative support to healthcare providers and patients in the Oncology Precision Medicine Program, advising on genomic testing (BostonGene) to guide treatment planning in collaboration with Welldyne Specialty Pharmacy
- Authored a 2022 congress summary for the International Society of Liquid Biopsy, published on the Hematology and Oncology Pharmacy Association (HOPA) website as part of the organization’s meeting resource summaries
- Supported the Psoriasis and Rheumatoid Arthritis Precision Medicine Program, consulting on the use of MindPx and PrismRA diagnostic tests to optimize biologic selection and improve patient outcomes in partnership with Welldyne Specialty Pharmacy

## Work Experience
**Clinical Pharmacist @ Healthdyne Specialty Pharmacy (formerly Welldyne Specialty Pharmacy)**  (_2019 – Present, Full-time_)
- Clinical patient management across oncology, autoimmune inflammatory diseases, hepatitis B/C, HIV, and multiple sclerosis
- Active involvement in URAC and ACHC accreditation preparation, audits, and quality compliance
- Oncology precision medicine program utilizing BostonGene molecular profiling to support treatment decisions
- Psoriasis and rheumatoid arthritis precision medicine programs incorporating MindPx and PrismRA testing
- Medical specialty program development and operational management
- Participation in oncology clinical pathway programs to support evidence-based therapy selection

**Compounding & Clinical Pharmacist @ CareMed Rx**  (_2015 – Present, Part-time_)
- Sterile compounding of chemotherapy agents and intravenous antibiotics
- Clinical consultation for infectious disease pharmacotherapy in home infusion settings
- Insurance claims review and prior authorization processing, including payer communication

**Clinical Pharmacist @ Quality Specialty Pharmacy**  (_2016 – 2019_)
- Clinical management of patients with oncology, autoimmune inflammatory diseases, hepatitis C, and HIV
- Delivery of Medication Therapy Management (MTM) services through OutcomeMTM and Mirixa platforms
- Support of Medicare Star Rating performance initiatives for chronic disease management

**Staff Pharmacist @ MacDill Pharmacy**  (_2014 – 2016_)
- Clinical patient management in oncology and dermatology
- Pharmacotherapy consultation for long-term care and assisted living facilities

## License and Certification
**Data Science**
- Artificail Intelligence in Medicine Advanced Certicate @ American Board of Artificial Intelligence in Medicine (ABAIM)
- Artificail Intelligence in Medicine Educational Certicate @ ABAIM

**Pharmacy**
- Pharmacist Licenses @ Alabama, Arkansas, Florida, Indiana, Kansas, Kentucky, Louisiana, Maryland, Michigan, Mississippi, Nebraska, Oklahoma, Tennessee, Texas, Virginia, West Virginia (Active, in good standing)
- Hematopoietic Cell Transplatation Training Course Certificate @ American Society for Transplantation and Cellular Therapy (ASTCT)
- Precision Medicine Oncology Genomics Certificate @ American College of Clinical Pharmacy (ACCP)
- Oncology Pharmacist Certificate (BCOP) @ Board of Pharmacy Specialties (BPS)
- Pharmacotherapy Certificate (BCPS) @ BPS
- Certified Specialty Pharmacist (CSP) @ National Association of Specialty Pharmacy
- Advanced Sterile Product Preparation Training Certificate @ American Society of Health-System Pharmacist (ASHP)
- Pharmacist Diabetes Care Certificate @ ASHP
- Medication Therapy Management Certificate @ American Pharmacist Association

## Publication
1. Yoon, AH., Oelofsen, M., Skomo, D., Page, N. Prospective Validation and Enhancement of a Machine Learning Model for Predicting Early Adalimumab Discontinuation in RA Patients Using Specialty Pharmacy Data. AIMed25 Abstract, November 9-12, 2025. [Link](https://aimed.swoogo.com/AIMed25)
2. Yoon, AH., Gedeck, P., Oelofsen, M. Predicting Early Discontinuation of Adalimumab in Rheumatoid Arthritis Patients Using Machine Learning: A Specialty Pharmacy-Based Approach. Journal of Managed Care & Specialty Pharmacy, Accepted November 26, 2025, to be published. 
3. Yoon, AH. International Society of Liquid Biopsy Annual Congress 2022 summary, Hematology and Oncology Pharmacy Association (HOPA) [Link](https://www.hoparx.org/resources/summaries-of-allied-organization-meetings/international-society-of-liquid-biopsy-annual-congress-2022/)
4. Yoon, H., Kim, HK., Ma, CJ., Huh, H. Induced accumulation of triterpenoids in _Scutellaria baicalensis_ suspension cultures using a yeast elicitor. Biotechnology Letters 22:1071-1075, 2000. [Link](https://link.springer.com/article/10.1023/A:1005610400511)
