**resume JD matcher annotation tool**

a simple project that matches your resume with a job description using jobscan API and shows how small changes impact your ATS score

*files*
- `sample-resume.png` → your updated resume
- `target_jd.txt` → the job description
- `resume_annotator.ipynb` → notebook for code + annotation

*sample code*
```python
from jobscan import ResumeMatcher
matcher = ResumeMatcher()
score = matcher.compare("sample-resume.png", "target_jd.txt")
print(f"ATS score impact: {score}%")
