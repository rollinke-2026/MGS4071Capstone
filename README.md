# MGS4071Capstone
This project takes a data-driven approach to talent acquisition, prioritizing candidates’ qualifications over potentially biasing background details. By using natural language processing to analyze resumes alongside a custom bias-mitigation layer, it promotes objective screening while aligning with ethical AI standards.
Project Mission
Traditional AI recruitment tools often unintentionally mirror human bias. This project is a merit-first screening engine designed to strip away demographic identifiers and focus exclusively on the intersection of candidate competencies and job requirements.

## Key Functionality

Dataset Creation: Creation of a Syntehtic Dataset

EDA: Standard EDA to understand the nature of the Dataset

PII Scrubbing: Utilizes NLP to sanitize resumes by removing names, contact info, and demographic proxies.

Weighted Skill Matching: Maps candidate experience to job descriptions using a customized similarity scoring algorithm.

Transparency First: Built with a "White-Box" philosophy, providing clear data points on why a candidate was ranked for review.

Healthcare & Finance Optimized: Tailored to identify high-level certifications (e.g., Six Sigma, Clinical Core, Analytics) across complex industries.

## Tech Stack
Language: Python

Libraries: Pandas, NumPy, Scikit-learn, Spacy (NLP)

Visualization: Streamlit for the recruiter-facing audit dashboard

Database: SQL for structured competency mapping

<img width="1072" height="680" alt="image" src="https://github.com/user-attachments/assets/bba23b2e-32cb-4079-b726-6448a502deff" />
This is the distribution of all applicants from the Dataset. More than half of the students are from State Schools, with thre remaining coming from Ivy, HBCU, Womens and Other categories.
