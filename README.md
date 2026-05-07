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

## Dataset Description
The dataset used in this project was generated within the Ethical AI Resume Screener notebook. Because real hiring datasets frequently contain sensitive personal information, the project used a synthetic candidate dataset designed to simulate realistic applicant profiles while avoiding privacy concerns.
The dataset represents candidates applying for a hypothetical data analytics position. Each candidate includes several structured and text-based variables relevant to hiring decisions.
Variables Included
The dataset contains the following variables:
•	Location
•	Years of experience
•	Degree level
•	Graduation year
•	Primary technical skill
•	Secondary technical skill
•	College name
•	College type
•	Blinded resume text
•	Match score
•	Strong-fit classification label
The target variable for the machine learning model is whether a candidate qualifies as a “strong fit” for the role.




<img width="1072" height="680" alt="image" src="https://github.com/user-attachments/assets/bba23b2e-32cb-4079-b726-6448a502deff" />
This is the distribution of all applicants from the Dataset. More than half of the students are from State Schools, with thre remaining coming from Ivy, HBCU, Womens and Other categories.



<img width="1908" height="955" alt="image" src="https://github.com/user-attachments/assets/bc326d91-e067-4492-a2fb-1abc323d7c1e" />

This is the actual Ai Ethical Screener

## EDA Insights

Dataset Overview: The dataset includes candidates from a variety of college types, such as Ivy League schools, HBCUs, women’s colleges, state schools, and other private universities. State schools make up the largest group, while Ivy League schools are the smallest. This creates a mix of backgrounds that reflects different types of institutions.

Match Scores Overall: Candidate match scores range from 0% to 40%, with an average of about 20%. Most candidates fall near the middle of this range, meaning scores are fairly similar overall rather than widely spread out.

Comparison by College Type: Average scores differ slightly depending on the type of college:

Ivy League candidates have the highest average scores

Candidates from “Other” schools have the lowest

The difference between the highest and lowest groups is less than 3 percentage points

Even though there are small differences, the score ranges for all groups overlap a lot. This means no group clearly stands out as consistently scoring much higher or lower than the others. Still, these small differences shouldn’t be ignored and would need further analysis to fully understand.

Experience vs. Match Score: There is almost no relationship between a candidate’s years of experience and their match score. In simple terms, having more experience does not seem to lead to a higher score in this dataset. This could mean the scoring system focuses more on skills than experience, or that experience is not being used effectively.

Fairness Considerations: At first glance, the scores look fairly similar across different college groups, which is a good sign. However, we cannot fully determine fairness just by comparing average scores. A proper fairness check would require setting a cutoff score (for example, deciding who “passes”) and then comparing how often candidates from each group meet that cutoff.

It’s also important to note that this is a synthetic (artificially created) dataset. Because of that, the results may reflect how the data was designed rather than how a real hiring system would behave.

Overall, the results suggest that scores are fairly consistent across groups and not strongly influenced by experience. However, more detailed analysis is needed before making firm conclusions about fairness.
