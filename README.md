# Clinical Pharmacist
# Data Scientist
## Clinical Background
- Board Certified Pharmacotherapy Specialist (BCPS)
- Board Certified Oncology Pharmacist (BCOP)
- Certified Specialty Pharmacist (CSP specialty pharmacy practice)
- Licensed Pharmacist in 17 U.S. states (active, in good standing)

## Technical Skills
#### AI & Machine Learning
- Python, R, PyTorch  
- Machine Learning & Deep Learning
- Predictive Modeling, Model Evaluation
- Model Interpretability
- Statistical Analysis

#### Large Language Models & Agentic AI
- LLM Evaluation & Benchmarking
- Prompt Engineering
- Retrieval-Augmented Generation (RAG)
- LoRA Fine-Tuning
- LangGraph
- Multi-Agent Orchestration
- Model Context Protocol (MCP)

#### Healthcare AI & Clinical Informatics
- FHIR, SMART-on-FHIR
- Clinical Decision Support
- AI Governance & Validation Workflows
- Prior Authorization Workflow Modeling
- FAERS Data Analysis

#### Data Engineering & Analytics
- Data Preprocessing
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Tableau
- Dashboard Development

#### Cloud & Deployment (in progress)
- Microsoft Azure AI Foundry
- AI Workflow Deployment
- Governance-Aware AI Systems

## Education
- Master of Science in Data Science, University of Virginia
- Doctor of Pharmacy (PharmD), University of Florida College of Pharmacy
- Master of Science in Pharmacy, Seoul National University College of Pharmacy, South Korea
- Bachelor of Pharmacy, Ewha Women’s University College of Pharmacy, South Korea

## Professional Activity

**Data Science & Applied Artificial Intelligence in Medicine**
- Medical Intelligence Society (MIS) member: participation in U.S. data science workshops, monthly meetings, and weekly office-hour discussion groups
- mCODE (Minimal Common Oncology Data Elements) Community member: engagement in use-case projects focused on applying mCODE standards to support third-party reimbursement and interoperability
  
**Pharmacy & Clinical Professional Societies**
- Society of Hematologic Oncology (SOHO) - member
- Florida Society of Clinical Oncology (FLASCO) - member
- Hematology/Oncology Pharmacy Association (HOPA) - member
- National Association of Specialty Pharmacy (NASP) - member

## Projects & Programs
## Flagship Projects
### Governance-Aware Prior Authorization AI Framework (LangGraph + Azure AI Foundry)
<details open>

<summary><strong>Enterprise Healthcare AI Governance Framework (2026 – Present)</strong></summary>
Designing and deploying a governance-aware agentic AI framework for prior authorization (PA) workflows using LangGraph orchestration and Microsoft Azure AI Foundry. The system integrates domain-specific clinical reasoning with deterministic validation layers, audit logging, and human-in-the-loop review to support safe and explainable AI-assisted utilization management.

The framework is being developed using the highest-performing LLMs identified through an internally developed PA benchmark and evaluation pipeline. Core architecture components include structured workflow orchestration, policy-aware reasoning, validation firewalls, traceable execution paths, and governance checkpoints designed for high-stakes healthcare environments.

Planned capabilities include:

- Dynamic retrieval of payer-specific PA criteria and clinical guidelines
- Structured decision support for specialty pharmacy and payer workflows
- Audit-ready logging and traceability for AI-generated outputs
- Safety-focused validation and escalation layers
- Deployment-oriented architecture using Azure AI infrastructure

This project focuses on translating healthcare LLM research into operationally realistic, governance-aware AI systems suitable for enterprise healthcare environments.

</details>

<br>

### Clinical LLM Evaluation Framework for Prior Authorization Reasoning
<details open> <summary><strong>Benchmark Development & Evaluation Framework (2025 – Present)</strong></summary>

Developing a clinically grounded benchmark and evaluation framework to assess large language model (LLM) performance in prior authorization (PA) review for adalimumab in rheumatoid arthritis (RA). The project focuses on evaluating whether LLMs can safely and reliably support utilization management workflows under realistic clinical documentation conditions.

The benchmark includes synthetic but clinically realistic chart notes designed to reflect variability commonly encountered in specialty pharmacy and payer workflows, including incomplete documentation, conflicting information, diverse provider writing styles, and edge-case scenarios.

Current and planned evaluation components include:

- Multi-pharmacist adjudication framework for gold-standard labeling
- Quantitative evaluation using accuracy, F1 score, ROC-AUC, false approval rate, and false denial rate
- LLM-as-a-judge assessment for rationale quality, faithfulness, and sufficiency
- Clinical error taxonomy analysis for failure mode characterization
- Comparative benchmarking across leading proprietary and open-source LLMs
- Exploration of retrieval-augmented generation (RAG) and preference-alignment strategies

The project emphasizes healthcare AI evaluation, clinical reliability, governance, and decision transparency rather than model fine-tuning alone.

</details>

[GitHub: PA-RA-Benchmark](https://github.com/baicalein/pa-ra-benchmark)

[Hugging Face: meta-llama/Llama-3.2-1B-Instruct with chart note summary](https://huggingface.co/baicalein/paLLM_adalimumab_RA_Lora)

[Hugging Face: meta-llama/Llama-3.2-3B-Instruct + LoRA with PA-RA-Benchmark](https://huggingface.co/baicalein/llama-lora-pa-reasoning)

[Hugging Face: google/gemma-4-E4B-it + LoRA with PA-RA-Benchmark](https://huggingface.co/baicalein/gemma-lora-pa-reasoning)

[Hugging Face: Qwen/Qwen3-4B-Instruct-2507 + LoRA with PA-RA-Benchmark](https://huggingface.co/baicalein/qwen-lora-pa-reasoning)

### Governed Agentic AI Framework for Emergency Care (SMART-on-FHIR + MCP)
<details open> <summary><strong>UVA Health Emergency Medicine Capstone Project (Completed | 2025–2026)</strong></summary>

Sponsored by UVA Health Emergency Medicine. Designed a governance-aware agentic AI framework to support emergency department workflows using LangGraph orchestration, SMART-on-FHIR interoperability, and Model Context Protocol (MCP)-based tool governance.

The system enables structured and auditable interaction with FHIR servers while enforcing deterministic validation and scoped data access policies. The architecture combines LLM-based requirement extraction with rule-based validation layers to support safe and policy-aware clinical workflow automation.

Core system components include:

- LangGraph-based deterministic orchestration workflows
- MCP-governed FHIR tool access (search, read, capabilities)
- Validation firewall for policy enforcement and input sanitation
- Audit-ready trace logging across workflow execution
- SMART-on-FHIR integration using least-privilege access principles

Implemented use case:

Emergency department patient snapshot generation (medications, allergies, recent encounters)

Awarded “Most Innovative Analytic Solution” during the UVA MSDS Capstone Showcase.

</details>

[GitHub Link](https://github.com/baicalein/Capstone_ER)

### Machine Learning Predictive Models for Early Adalimumab Discontinuation in Rheumatoid Arthritis
<details open> <summary><strong>Healthcare Predictive Analytics Research (Completed | 2023 – 2025)</strong></summary>

Developed machine learning models to predict early discontinuation of adalimumab therapy among patients with rheumatoid arthritis using real-world specialty pharmacy data.

Using baseline clinical and patient-reported variables available at treatment initiation, multiple predictive approaches were evaluated to identify patients at elevated risk for early therapy discontinuation. Elastic net–regularized logistic regression demonstrated the strongest overall performance while maintaining interpretability appropriate for clinical decision support applications.

Key project components included:

- Predictive modeling using real-world specialty pharmacy datasets
- Feature engineering and preprocessing of longitudinal patient data
- Model evaluation using ROC-AUC, F1 score, calibration, and interpretability analysis
- Comparative evaluation of multiple machine learning approaches for healthcare prediction tasks

The study demonstrated that interpretable machine learning models can effectively identify patients at risk for early biologic therapy discontinuation and may support targeted pharmacist-led interventions in specialty pharmacy practice.

Results from this project were published in the Journal of Managed Care & Specialty Pharmacy (JMCP).

</details>

[GitHub Link](https://github.com/baicalein/ML-Predictive-Models-on-Early-Discontinuation-of-Adalimumab-in-RA)

## Additional Projects
### Agentic AI Assistant for Laboratory Result Communication
<details> <summary><strong>Governance-Aware Clinical Communication Workflow (2026)</strong></summary>

Developed a governance-aware agentic AI system to assist physicians in communicating laboratory results using structured clinical logic and LLM-generated patient messaging.

Implemented modular workflows for abnormality detection, severity scoring, follow-up question generation, message drafting, and safety review validation. Applied strict safeguards to prevent diagnostic overreach, inappropriate medication advice, and unsafe communication patterns.

The project emphasizes clinical safety, auditability, and controlled AI-assisted patient communication.

</details>

[GitHub Link](https://github.com/baicalein/agentic-ai-lab-results-assistant)

### Machine Learning–Driven Comparative Safety Analysis of ALK Inhibitors Using FAERS Data
<details> <summary><strong>Pharmacovigilance & Safety Signal Detection (2026)</strong></summary>

Developing machine learning pipelines for comparative safety analysis of ALK inhibitors in non-small cell lung cancer (NSCLC) using FDA Adverse Event Reporting System (FAERS) data.

The project includes large-scale preprocessing, adverse event normalization, feature engineering, temporal trend analysis, and supervised learning approaches for safety signal detection and comparative risk profiling.

</details>

[GitHub Link](https://github.com/baicalein/faers-alk-safety-ml)

### Melanoma Detection Using Knowledge Distillation for Mobile Deployment
<details> <summary><strong>Edge AI & Mobile Health Application Research (2025)</strong></summary>

Investigated knowledge distillation techniques to enable efficient melanoma detection on resource-constrained mobile devices using the HAM10000 dermoscopy dataset.

Developed compact MobileNetV3-based student models trained from larger teacher architectures while preserving diagnostic performance and calibration quality suitable for edge deployment scenarios.

</details>

[GitHub Link](https://github.com/baicalein/Melanoma-Detection-with-Knowledge-Distillation)

### Interdisciplinary Lifestyle Intervention Platform for Rheumatoid Arthritis
<details> <summary><strong>Exercise Science + Clinical Pharmacy + Data Science Collaboration (Planned)</strong></summary>

Planned interdisciplinary project integrating exercise science, clinical pharmacy, and data science to support personalized lifestyle interventions for patients with rheumatoid arthritis.

The proposed system will incorporate trainer-collected real-world data, individualized exercise programming, and mobile health communication workflows to support long-term patient engagement and care coordination.

</details>

<br>

## Precision Medicine & Biomarker Programs
<details open> <summary><strong>Precision Medicine & Biomarker-Guided Care Programs (2022 – 2023)</strong></summary>

Supported oncology and autoimmune precision medicine initiatives within specialty pharmacy practice through collaboration with healthcare providers, patients, and diagnostic testing programs.

Contributed to oncology precision medicine workflows involving genomic profiling and liquid biopsy applications, including consultation support related to the use of BostonGene molecular testing to inform individualized treatment planning in collaboration with Welldyne Specialty Pharmacy.

Also supported biomarker-guided therapy optimization programs for rheumatoid arthritis and psoriasis using diagnostic platforms including MindPx and PrismRA to assist biologic selection and treatment decision support.

Additional activities included authorship of a congress summary for the International Society of Liquid Biopsy, published through the Hematology/Oncology Pharmacy Association meeting resource program.

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

**Staff Pharmacist @ CareMed Rx**  (_2015 – 2019, part time_)
- Sterile compounding of chemotherapy agents and intravenous antibiotics
- Clinical consultation on pharmacotherapy in home infusion and outpatient infusion settings

**Clinical Pharmacist @ Quality Specialty Pharmacy**  (_2016 – 2019, full time_)
- Clinical management of patients with oncology, autoimmune inflammatory diseases, hepatitis C, and HIV
- Delivery of Medication Therapy Management (MTM) services through OutcomeMTM and Mirixa platforms
- Support of Medicare Star Rating performance initiatives for chronic disease management

**Staff Pharmacist @ MacDill Pharmacy**  (_2014 – 2016_)
- Clinical patient management in oncology and dermatology
- Pharmacotherapy consultation for long-term care and assisted living facilities

**Staff Pharmacist @ Walgreens Pharmacy**  (_2002 – 2007, full time_)

**Pharmacist Intern @ Walgreens Pharmacy**  (_2002 – 2002_)

## License and Certification
**Data Science & Artificial Intelligence**
- Artificial Intelligence in Medicine – Advanced Certificate, American Board of Artificial Intelligence in Medicine (ABAIM)
- Artificial Intelligence in Medicine – Educational Certificate, American Board of Artificial Intelligence in Medicine (ABAIM)

**Pharmacy & Clinical Practice**
- Pharmacist Licensure: Alabama, Arkansas, Florida, Indiana, Kansas, Kentucky, Louisiana, Maryland, Michigan, Mississippi, Nebraska, Oklahoma, Oregon, Tennessee, Texas, Virginia, West Virginia (Active, in good standing)
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
2. Yoon, AH., Gedeck, P., Oelofsen, M. Predicting Early Discontinuation of Adalimumab in Rheumatoid Arthritis Patients Using Machine Learning: A Specialty Pharmacy-Based Approach. Journal of Managed Care & Specialty Pharmacy 2026;32(3):336-347 [Link](https://doi.org/10.18553/jmcp.2026.32.3.336). 
3. Yoon, AH. International Society of Liquid Biopsy Annual Congress 2022 summary, Hematology and Oncology Pharmacy Association (HOPA) [Link](https://www.hoparx.org/resources/summaries-of-allied-organization-meetings/international-society-of-liquid-biopsy-annual-congress-2022/)
4. Yoon, H., Kim, HK., Ma, CJ., Huh, H. Induced accumulation of triterpenoids in _Scutellaria baicalensis_ suspension cultures using a yeast elicitor. Biotechnology Letters 22:1071-1075, 2000. [Link](https://link.springer.com/article/10.1023/A:1005610400511)
