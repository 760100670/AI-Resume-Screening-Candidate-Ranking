# AI Resume Screening & Job Matching System

An AI-powered web application that analyzes resumes against job descriptions and calculates a match percentage using Natural Language Processing (NLP) and machine learning techniques.

## Features

- Upload resumes in PDF or DOCX format
- Enter a job description
- Extract text from PDF and DOCX files
- Text preprocessing using NLTK
- TF-IDF feature extraction
- Cosine similarity-based resume-job matching
- Match percentage calculation
- Candidate match categorization:
  - Great Match (>= 85%)
  - Good Match (>= 70%)
  - Average Match (>= 40%)
  - Poor Match (< 40%)

## Demo

### Home Page

![Home Page](screenshots/Home.png)

### Resume Upload

![Resume Upload](screenshots/ResumeUpload.png)

### Match Result

![Match Result](screenshots/Result.png)

## Tech Stack

- **Programming Language:** Python
- **Backend:** Flask
- **NLP:** NLTK
- **Machine Learning:** Scikit-learn
- **PDF Processing:** PyPDF2
- **DOCX Processing:** python-docx
- **Frontend:** HTML, CSS

## How It Works

1. User uploads a resume in PDF or DOCX format.
2. User enters a job description.
3. Resume text is extracted from the uploaded file.
4. Text is cleaned and preprocessed using NLP techniques.
5. TF-IDF converts the text into numerical features.
6. Cosine similarity calculates the similarity between the resume and job description.
7. The system generates a match percentage.
8. The candidate is categorized as Great, Good, Average, or Poor Match.

## Project Structure

```text
AI-Resume-Screening-Candidate-Ranking/
│
├── sample_resumes/
├── screenshots/
├── static/
├── templates/
│
├── app.py
├── matcher.py
├── resume_parser.py
├── requirements.txt
├── README.md
└── .gitignore