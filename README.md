⚕️ MEDA — Medicine & Data Assistant
AI-Powered Clinical Decision Support System
![Python](https://img.shields.io/badge/Python-3.9+-blue?style=flat-square&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red?style=flat-square&logo=streamlit)
![Accuracy](https://img.shields.io/badge/Benchmark%20Accuracy-90.4%25-green?style=flat-square)
![Records](https://img.shields.io/badge/Clinical%20Records-5%2C000%2B-navy?style=flat-square)
![Live](https://img.shields.io/badge/Status-Live-brightgreen?style=flat-square)
Live Demo → meda-clinical-tool.streamlit.app
---
Overview
MEDA (Medicine & Data Assistant) is an AI-powered clinical decision support tool built to reduce drug lookup time, surface drug interactions, and support clinical reasoning through structured, validated outputs.
Built by Ananya Thathigowdara — Data Engineer & MS Information Systems candidate at Northeastern University (May 2026).
> *"When data is wrong in healthcare, someone gets hurt. There's no 'approximately correct.' That standard changed how I approach every dataset I touch."*
---
Key Metrics
Metric	Result
Benchmark Accuracy	90.4%
Clinical Records Validated	5,000+ anonymized records
Benchmark Scenarios Tested	100+ edge cases
Drug Lookup Time Reduction	60% vs manual process
Classification Error Reduction	30% vs baseline
---
Features
🔍 Drug Interaction Lookup
Cross-references a validated clinical database of drug pairs. Flags interactions by severity:
HIGH — Avoid or monitor intensively
MODERATE — Monitor with dose adjustment consideration
LOW — Awareness advised
Supported drugs: Metformin · Warfarin · Lisinopril · Atorvastatin · Amoxicillin
🩺 Clinical Symptom Assessment
Evidence-based differential diagnosis generation with:
Prioritized differential diagnosis list
Red flag identification (act immediately)
Recommended diagnostic workup
Supported presentations: Chest Pain · Shortness of Breath · Hyperglycemia
⚠️ Contraindication Check
Cross-references patient conditions against known absolute and relative contraindications for a given medication.
💊 Dosing Reference
Standard dosing protocols sourced from FDA labeling and major clinical guidelines (ACC/AHA, ADA, IDSA), with monitoring requirements.
---
Tech Stack
Layer	Technology
Language	Python 3.9+
Framework	Streamlit
AI Engine	GPT-3.5 (OpenAI API)
Data Processing	Pandas · NumPy
Deployment	Streamlit Cloud
Version Control	GitHub
---
Getting Started
Prerequisites
```bash
python >= 3.9
pip
```
Installation
```bash
# Clone the repository
git clone https://github.com/Ananya1ani/meda-clinical-tool.git
cd meda-clinical-tool

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```
The app will open at `http://localhost:8501`
---
Usage
Select a query type from the sidebar (Drug Interaction, Symptom Assessment, Contraindication Check, Dosing Reference)
Click an example query or type your own in the text box
Hit "Run Query" — MEDA processes and returns structured clinical output
Results include severity ratings, monitoring requirements, contraindications, and benchmark validation
Example Queries
"What are the interactions between metformin and contrast dye?"
"Patient presenting with chest pain, diaphoresis, and arm radiation"
"Can metformin be used in a patient with eGFR of 25?"
"Standard dosing for atorvastatin in high cardiovascular risk"
---
Methodology
MEDA was developed using a structured engineering approach applied to a high-stakes clinical domain:
Data Collection — 5,000+ anonymized clinical records sourced for validation
Model Adaptation — GPT-3.5 adapted via prompt engineering for clinical query processing
Validation Framework — 100+ benchmark scenarios covering standard cases and edge cases
Failure Mode Documentation — Every failure mode identified and documented before accuracy was reported
Deployment — Live on Streamlit Cloud with zero-downtime updates via GitHub integration
Why This Approach?
Coming to clinical data as a data engineer — not a clinician — meant asking questions insiders had stopped asking. The outsider advantage: when you have no assumptions, you validate everything. That produced a more rigorous system than domain familiarity would have.
---
Project Structure
```
meda-clinical-tool/
│
├── app.py              # Main Streamlit application
├── requirements.txt    # Python dependencies
└── README.md           # This file
```
---
Clinical Disclaimer
> MEDA provides **decision support only** — not a substitute for clinical judgment. All recommendations must be verified against current guidelines and patient-specific factors including renal function, hepatic status, age, weight, comorbidities, and concurrent medications.
---
About the Builder
Ananya Thathigowdara  
Data Engineer · BI Specialist · AI Builder  
MS Information Systems — Northeastern University, Boston MA (May 2026)
🌐 Portfolio: [deployed on Vercel]
💼 LinkedIn: linkedin.com/in/ananya-n-thathigowdara
✍️ Substack: ananyant16.substack.com
💻 GitHub: github.com/Ananya1ani
📧 Email: ananyant166@gmail.com
---
Built as part of INFO 7375: Branding & AI — Northeastern University, 2026
