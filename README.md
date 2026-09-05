# Online Course App — Final Project (with Exam Feature)

## Setup
```bash
python -m venv venv
source venv/bin/activate        # venv\Scripts\activate on Windows
pip install -r requirements.txt
python manage.py makemigrations onlinecourse
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

## App structure (maps to the assignment tasks)

| Task | File |
|---|---|
| 1 — Question, Choice, Submission models | `onlinecourse/models.py` |
| 2 — admin.py (7 imported classes, QuestionInline, ChoiceInline, QuestionAdmin, LessonAdmin) | `onlinecourse/admin.py` |
| 3 — Admin site screenshot | Visit `/admin/` after `createsuperuser`, screenshot as `03-admin-site.png` |
| 4 — course_details_bootstrap.html | `onlinecourse/templates/onlinecourse/course_details_bootstrap.html` |
| 5 — submit / show_exam_result views | `onlinecourse/views.py` |
| 6 — submit / show_exam_result urls | `onlinecourse/urls.py` |
| 7 — Passing exam screenshot | Enroll in a course, answer a question's exam correctly, submit, screenshot the "Congratulations" result page as `07-final.png` |

## Getting your screenshots

1. **03-admin-site**: Log in to `http://127.0.0.1:8000/admin/` as the superuser. The dashboard
   should show both the "Authentication and Authorization" group (Groups, Users) and the
   "Onlinecourse" group (Course, Lesson, Instructor, Learner, Enrollment, Question, Choice).
   Screenshot the whole page and save it as `03-admin-site.png`.

2. **07-final**: In the admin, create a Course → Lesson → Question → Choices (mark the correct
   choice(s) with `is_correct=True`). Then, as a logged-in learner, go to the course details page,
   enroll, check the correct choice(s) in the exam form, and click "Submit Exam." The result page
   will show "Congratulations! You passed the exam." with your score. Screenshot it as `07-final.png`.

## Pushing to GitHub

```bash
git init
git add .
git commit -m "Final project: online course app with exam feature"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

Then submit these GitHub URLs for the assignment:
- `models.py` → `https://github.com/<you>/<repo>/blob/main/onlinecourse/models.py`
- `admin.py` → `https://github.com/<you>/<repo>/blob/main/onlinecourse/admin.py`
- `course_details_bootstrap.html` → `https://github.com/<you>/<repo>/blob/main/onlinecourse/templates/onlinecourse/course_details_bootstrap.html`
- `views.py` → `https://github.com/<you>/<repo>/blob/main/onlinecourse/views.py`
- `urls.py` → `https://github.com/<you>/<repo>/blob/main/onlinecourse/urls.py`
"# projrct1" 
