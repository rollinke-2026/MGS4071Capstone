# MGS4071Capstone
This project takes a data-driven approach to talent acquisition, prioritizing candidates’ qualifications over potentially biasing background details. By using natural language processing to analyze resumes alongside a custom bias-mitigation layer, it promotes objective screening while aligning with ethical AI standards.
Project Mission
Traditional AI recruitment tools often unintentionally mirror human bias. This project is a merit-first screening engine designed to strip away demographic identifiers and focus exclusively on the intersection of candidate competencies and job requirements.

## Key Functionality
PII Scrubbing: Utilizes NLP to sanitize resumes by removing names, contact info, and demographic proxies.

Weighted Skill Matching: Maps candidate experience to job descriptions using a customized similarity scoring algorithm.

Transparency First: Built with a "White-Box" philosophy, providing clear data points on why a candidate was ranked for review.

Healthcare & Finance Optimized: Tailored to identify high-level certifications (e.g., Six Sigma, Clinical Core, Analytics) across complex industries.

## Tech Stack
Language: Python

Libraries: Pandas, NumPy, Scikit-learn, Spacy (NLP)

Visualization: Streamlit for the recruiter-facing audit dashboard

Database: SQL for structured competency mapping
