# Day 6 — ATS Resume Optimization & Prompt Engineering Case Study

## What I Did Today

Built and optimized a professional ATS-ready resume and explored how context changes the quality of AI-generated outputs through a side-by-side prompt engineering comparison.

---

## Tasks Completed

### 1. Resume Built & ATS Optimized
- Created a full ATS-optimized resume from scratch using Python (ReportLab)
- Scored and improved the resume from **28/100 → 87/100**
- Structured sections: Summary, Education, Projects, Skills, Certifications
- Documented real projects with proper tech stack keywords

### 2. Projects Documented
- **Face Recognition Attendance System** — Python, OpenCV, face_recognition library
- **Phishing Detection System** — Python, Machine Learning, NLP, scikit-learn
- Both presented at **Smart India Hackathon (SIH) 2025**

### 3. Prompt Engineering Case Study
- Compared **Prompt A (no context)** vs **Prompt B (with context)** for a 30-day learning roadmap
- Visualized the comparison as an interactive HTML page and a PNG infographic
- Key finding: adding context (role, skills, goal, time, style) improved output quality by ~5x

---

## Key Learnings

- **ATS systems** parse resumes as plain text — no tables, icons, or columns
- **Keyword density** matters: listing exact library names (OpenCV, scikit-learn) beats generic terms
- **Context in prompts** acts as a filter — each field eliminates irrelevant AI output
- Formula: `Situation + Skills + Goal + Constraints + Style = Personalised Output`
- Real projects with named tech stacks are worth more than certifications alone on a fresher resume

---

## Tools & Tech Used Today

| Tool | Purpose |
|------|---------|
| Python | Resume PDF generation, project work |
| ReportLab | PDF creation (ATS-safe formatting) |
| OpenCV | Face Recognition project |
| scikit-learn | Phishing Detection ML model |
| face_recognition | Face encoding & detection |
| HTML / CSS / JS | Interactive prompt comparison UI |
| Pillow (PIL) | Infographic image generation |

---

## ATS Score Progress

| Version | Score | What Changed |
|---------|-------|--------------|
| Original | 28/100 | Raw bullet points, no structure |
| After formatting | 71/100 | Sections, keywords, plain text |
| After adding projects | 87/100 | Real projects with tech stacks |

---

## Files Generated

- `Mohd_Faizan_Resume_v2.pdf` — Final ATS-optimized resume
- `prompt-ab-comparison.html` — Interactive Prompt A vs B comparison
- `prompt-ab-comparison.png` — Infographic version

---

## Next Steps

- [ ] Upload resume projects (Face Recognition + Phishing Detection) to GitHub
- [ ] Add GitHub links to resume project entries
- [ ] Push ATS score above 90 by linking live repos
- [ ] Start Day 7 learning module

---

*Day 6 of #100DaysOfAI | #PromptEngineering #Python #MachineLearning #ATS #ResumeBuilding*
