# Resume Keyword Checker 📝

This Python script checks whether a resume (in `.docx` format) contains specific **keywords** that are often important for job applications, especially in the AI/ML and software domains.  

---

## 🔑 Features
- Reads a **Word (.docx)** file using `python-docx`.
- Extracts all text from the resume into a single string.
- Searches for a list of **predefined keywords** using `regex` (case-insensitive).
- Reports which keywords are **found ✅** and which are **missing ❌**.
- Provides a final decision:
  - **Resume Passed ✅** → All keywords are present.
  - **Resume Rejected ❌** → Some keywords are missing.

---

## 📂 Keywords Checked
| Category             | Keywords                                                                 |
|----------------------|--------------------------------------------------------------------------|
| **AI & ML**          | Artificial Intelligence, Machine learning, TensorFlow, PyTorch           |
| **Frameworks**       | Python flask framework                                                   |
| **Experience**       | Internship, Research, Capstone Project, Hackathon                        |
| **Collaboration**    | Open Source, Freelance, Github                                           |
| **Soft Skills**      | Leadership, Teamwork, Problem Solving, Communication, Presentation, Innovation |

---

## ⚙️ How It Works
1. Load the resume file:
2. Extract all paragraph text into a single string.

For each keyword in the list:

If found → mark as FOUND.

If not found → mark as MISSING.

Print summary:

Missing keywords (if any).

Resume status (Passed/Rejected)

python resume_checker.py

Then, enter the path of your resume when prompted:
Enter path of your resume (.docx): my_resume.docx
FOUND: Artificial Intelligence
MISSING: Hackathon
FOUND: Python flask framework
...
Resume Rejected ❌
Missing: ['Hackathon', 'Freelance']

   ```python
   doc = Document(file_path)
