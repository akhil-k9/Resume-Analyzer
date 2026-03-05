# Resume Analyzer



The application uses **semantic similarity with sentence-transformer embeddings** to compare a candidate’s resume with a job description and provide insights such as:

- Resume–Job Match Score
- Matching Keywords
- Missing Keywords
- Overall Match Verdict

This tool helps candidates understand how well their resume fits a specific job role and improve it for better ATS performance.

---

## Features

✔ Upload resumes in **PDF, DOCX, or TXT** format  
✔ Paste **Job Description** for comparison  
✔ AI-based **semantic similarity scoring**  
✔ Extract **matched and missing keywords**  
✔ Provides **match verdict (Strong / Moderate / Weak)**  
✔ Fast backend API built using **Flask**  

---

## How It Works

1. The user uploads a **resume** or pastes resume text.
2. The user enters a **job description**.
3. The system extracts the text from the resume.
4. Both texts are converted into **semantic embeddings using a Transformer model**.
5. **Cosine similarity** calculates the match score.
6. Keywords are analyzed to identify:
   - Matching keywords
   - Missing keywords

The final output includes a **percentage match score and suggestions for improvement**.

---

## Tech Stack

| Technology | Purpose |
|-----------|--------|
| Python | Backend language |
| Flask | Web framework |
| Transformers | NLP model loading |
| PyTorch | Deep learning framework |
| Sentence Transformers | Semantic embeddings |
| Scikit-learn | Cosine similarity |
| PyPDF2 | Extract text from PDF |
| python-docx | Extract text from DOCX |
| NumPy | Numerical operations |

---

## AI Model Used

The project uses the **sentence-transformers model**:

```
sentence-transformers/all-roberta-large-v1
```

This model generates high-quality **semantic sentence embeddings** which allow the system to compare resume and job description meaningfully.

---

## Project Structure

```
Resume-Analyzer/
│
├── templates/
│   └── index.html        # Frontend interface
│
├── static/               # CSS / JS files
│
├── app.py                # Main Flask application
├── requirements.txt      # Dependencies
└── README.md
```

---

## Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/akhil-k9/Resume-Analyzer.git
cd Resume-Analyzer
```

---

### 2️⃣ Create virtual environment (recommended)

```bash
python -m venv venv
```

Activate it:

Windows
```bash
venv\Scripts\activate
```

Mac/Linux
```bash
source venv/bin/activate
```

---

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Run the application

```bash
python app.py
```

The app will run on:

```
http://127.0.0.1:5000
```

---

## Supported Resume Formats

The analyzer currently supports:

- PDF (.pdf)
- Word Documents (.docx)
- Text Files (.txt)

---

## Example Output

The analyzer returns:

```
Match Score: 72.4%

Verdict: Moderate Match

Matched Keywords:
Python
Machine Learning
APIs
Data Analysis

Missing Keywords:
Docker
AWS
Microservices
```

This helps candidates **optimize their resume for the job role**.

---

## Future Improvements

Possible enhancements for the project:

- ATS score breakdown
- Resume improvement suggestions
- Highlight missing skills


---

## Author

**Akhil**


GitHub:  
https://github.com/akhil-k9

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!