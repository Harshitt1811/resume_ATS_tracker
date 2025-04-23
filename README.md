# ATS Resume Checker

## Overview
ATS Resume Checker is a Streamlit-based web application designed to evaluate resumes against job descriptions for roles in Data Science, Full Stack Web Development, Big Data Engineering, DevOps, Data Analyst, and Project Management. Powered by Google's Gemini AI, the application provides two key functionalities:
1. **Resume Feedback**: Offers a professional evaluation of the resume, highlighting strengths and weaknesses relative to the job description.
2. **Percentage Match**: Calculates a percentage match between the resume and job description, identifying missing keywords and providing final thoughts.

## Features
- Upload resumes in PDF format.
- Input job descriptions via a text area.
- ATS-like evaluation with percentage match and keyword analysis.
- Professional HR-style feedback for resume alignment with job requirements.
- User-friendly interface with a centered layout and responsive design.
- Powered by Gemini AI for intelligent resume analysis.
- Styled with a clean, professional look using Streamlit's markdown and CSS.

## Tech Stack
- **Python**: Core programming language.
- **Streamlit**: Framework for building the web application.
- **Google Gemini AI**: For resume evaluation and ATS scanning.
- **PyMuPDF (fitz)**: For processing PDF resumes.
- **Pillow (PIL)**: For converting PDF pages to images.
- **Base64**: For encoding images to send to Gemini AI.
- **python-dotenv**: For managing API keys securely.
- **HTML/CSS**: For custom styling in Streamlit.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ats-resume-checker.git
   cd ats-resume-checker


python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

pip install -r requirements.txt


GOOGLE_API_KEY=your-google-api-key

streamlit run app.py
