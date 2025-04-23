ATS Resume Checker
Overview
ATS Resume Checker is a Streamlit-based web application designed to evaluate resumes against job descriptions for roles in Data Science, Full Stack Web Development, Big Data Engineering, DevOps, Data Analyst, and Project Management. Powered by Google's Gemini AI, the application provides two key functionalities:

Resume Feedback: Offers a professional evaluation of the resume, highlighting strengths and weaknesses relative to the job description.
Percentage Match: Calculates a percentage match between the resume and job description, identifying missing keywords and providing final thoughts.

Features

Upload resumes in PDF format.
Input job descriptions via a text area.
ATS-like evaluation with percentage match and keyword analysis.
Professional HR-style feedback for resume alignment with job requirements.
User-friendly interface with a centered layout and responsive design.
Powered by Gemini AI for intelligent resume analysis.
Styled with a clean, professional look using Streamlit's markdown and CSS.

Tech Stack

Python: Core programming language.
Streamlit: Framework for building the web application.
Google Gemini AI: For resume evaluation and ATS scanning.
PyMuPDF (fitz): For processing PDF resumes.
Pillow (PIL): For converting PDF pages to images.
Base64: For encoding images to send to Gemini AI.
python-dotenv: For managing API keys securely.
HTML/CSS: For custom styling in Streamlit.

Installation

Clone the repository:git clone https://github.com/your-username/ats-resume-checker.git
cd ats-resume-checker


Create a virtual environment and activate it:python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


Install the required dependencies:pip install -r requirements.txt


Create a .env file in the project root and add your Google API key:GOOGLE_API_KEY=your-google-api-key


Run the Streamlit app:streamlit run app.py



Usage

Open the app in your browser (typically at http://localhost:8501).
Upload a resume in PDF format.
Enter the job description in the text area.
Click Tell Me About the Resume for detailed feedback or Percentage Match for an ATS-style score.
View the results displayed on the main panel.

File Structure

app.py: Main Streamlit application script.
requirements.txt: List of Python dependencies.
.env: Environment file for storing API keys (not tracked in Git).
README.md: Project documentation (this file).

Dependencies
Listed in requirements.txt:
streamlit
pymupdf
pillow
google-generativeai
python-dotenv

Notes

Ensure your Google API key is valid and has access to the Gemini AI model (gemini-1.5-flash).
The app processes only the first page of the PDF resume for analysis.
No local file I/O is used beyond PDF upload, making it compatible with Streamlit's deployment environment.
The app is designed to run locally or be deployed on platforms like Streamlit Cloud.

Contributing

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit (git commit -m "Add feature").
Push to the branch (git push origin feature-branch).
Open a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgments

Built with Streamlit and Google Gemini AI.
Inspired by the need for better ATS-compatible resume tools for tech professionals.

