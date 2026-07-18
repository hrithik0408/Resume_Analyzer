# Resume Analyzer

Resume Analyzer is a Python project that leverages AI to parse resumes (PDF/DOCX) and evaluate them against job descriptions.  
It extracts structured information such as skills, education, and experience, calculates match scores, highlights missing skills, and ranks candidates.  
This tool helps recruiters shortlist faster and job seekers benchmark their resumes.

## 🧠 Architecture Mind Map

```mermaid
mindmap
  root((Resume Analyzer))
    Job Description Parser
      Extract role
      Required skills
      Education
      Responsibilities
    Resume Parser
      PDF parsing
      DOCX parsing
      Skills extraction
      Experience extraction
    Matching Engine
      Compare resume vs job
      Calculate match %
      Identify missing skills
      Rank candidates
    Output
      Top candidates
      Lowest candidates
      Final verdict
