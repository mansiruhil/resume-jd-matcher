**resume JD matcher annotation tool**

a simple project that matches your resume with a job description using jobscan API and shows how small changes impact your ATS score

*files*
- `sample-resume.png` 
- `resume_annotator.ipynb` 

*sample code*
```python
from jobscan import ResumeMatcher
matcher = ResumeMatcher()
score = matcher.compare("sample-resume.png", "resume-extracted.csv")
print(f"ATS score impact: {score}%")
