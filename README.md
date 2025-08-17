📄 ATS Resume Expert

An AI-powered Applicant Tracking System (ATS) Resume Analyzer built with Python and Streamlit, leveraging Google Gemini AI.

The tool helps job seekers improve their resumes and recruiters quickly analyze candidates by comparing resumes against job descriptions. It provides evaluations, keyword analysis, and ATS-style match percentages — complete with downloadable reports.

🚀 Features

📋 Resume Evaluation – AI feedback on strengths, weaknesses, and suggested improvements.

🔎 Keyword Analysis – Detects matched and missing keywords between resume and job description.

📊 Match Percentage – Provides ATS-like score and tips to increase it.

👀 PDF Resume Preview – Shows first page preview of uploaded resume.

📥 Downloadable Reports – Generates .docx reports for each analysis option.

📝 Feedback Logging – Saves user feedback into feedback_log.txt.

🛠️ Tech Stack

Frontend / UI: Streamlit

AI Engine: Google Gemini API

File Handling:

PyPDF2 → Extract text from PDF resumes

pdf2image → Convert resume pages to images

Pillow (PIL) → Image processing

python-docx → Generate downloadable reports

Environment Management: python-dotenv

Logging: Python’s built-in logging

📂 Project Structure
.
├── app.py                 # Main Streamlit application
├── assets/                # Static assets (logo, CSS)
│   ├── logo.png
│   └── styles.css
├── feedback_log.txt       # Stores user feedback
├── requirements.txt       # Project dependencies
└── README.md              # Documentation

⚙️ Setup Instructions
1. Clone Repository
git clone https://github.com/yourusername/ats-resume-expert.git
cd ats-resume-expert

2. Create Virtual Environment
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

3. Install Dependencies
pip install -r requirements.txt

4. Add API Key

Create a .env file in the project root:

GEMINI_API_KEY=your_api_key_here


You can get a Gemini API key from Google AI Studio.

5. Run the App
streamlit run app.py


The app will open at: http://localhost:8501

📊 Usage Guide

Enter Job Description – Paste the JD in the provided text area.

Upload Resume – Upload your resume in PDF format.

Choose Analysis – Click one of the options:

📋 Resume Evaluation

🔎 Keyword Analysis

📊 Match Percentage

View Results – AI will generate structured analysis.

Download Report – Save results as a .docx file.

Submit Feedback – Optionally share feedback (saved locally in feedback_log.txt).

📊 Example Output

Keyword Analysis Example:

✅ Matched Keywords

Python

SQL

Machine Learning

❌ Missing Important Keywords

Cloud Computing

Data Engineering

Deep Learning

🔮 Future Enhancements

Multi-format support (DOCX, TXT)

Batch resume screening

Advanced NLP models (embeddings, BERT/GPT for semantic similarity)

Recruiter dashboard with saved history

Deployment on Streamlit Cloud / Hugging Face Spaces

📝 License

This project is licensed under the MIT License.
