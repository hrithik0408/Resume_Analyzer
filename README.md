# Resume Analyzer

Resume Analyzer is a Python project that leverages AI to parse resumes (PDF/DOCX) and evaluate them against job descriptions.  
It extracts structured information such as skills, education, and experience, calculates match scores, highlights missing skills, and ranks candidates.  
This tool helps recruiters shortlist faster and job seekers benchmark their resumes.

---

## 📐 Architecture Overview

The project is divided into clear modules:

1. **Job Description Parser**  
   - Converts raw job descriptions into structured JSON using LLMs.  
   - Captures role, required skills, education, and responsibilities.

2. **Resume Parser**  
   - Reads resumes in PDF/DOCX format using `pypdf` and `python-docx`.  
   - Extracts candidate details (skills, education, experience, projects).  
   - Normalizes data into a consistent schema.

3. **Matching Engine**  
   - Compares resume data against job requirements.  
   - Calculates match percentage, identifies missing skills, and generates verdicts.  
   - Outputs top and lowest candidates.

4. **Error Handling**  
   - Skips corrupted/unreadable files gracefully.  
   - Ensures batch processing continues without interruption.

---

## ⚙️ Tech Stack
- Python  
- `python-docx` → DOCX parsing  
- `pypdf` → PDF parsing  
- `python-dotenv` → API key management  
- `groq` → LLM-powered analysis  
- `pydantic` → Data models & validation  

---

## 🚀 Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/hrithik0408/Resume_Analyzer.git
cd Resume_Analyzer
pip install -r requirements.txt
