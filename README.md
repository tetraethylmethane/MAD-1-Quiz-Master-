---

# Quiz Master

Interactive quiz application built with Flask that allows users to take quizzes, track their scores, and engage with a variety of quiz categories. The project includes functionality to manage quizzes, users, and leaderboards.

## Features

- Create and manage quizzes
- User authentication and management
- Track quiz scores and display leaderboard

## Installation

1. Clone the repository:

```bash
git clone 
cd quiz-master
```

2. Set up a virtual environment:

```bash
python -m venv .venv
```
- For macOS/Linux
```bash
source .venv/bin/activate
```
- For Windows
```bash
.venv\Scripts\activate
```

3. Install the dependencies:

```bash
pip install -r requirements.txt
```

4. Set environment variables in `.env` file:

```bash
SECRET_KEY= your_secret_key
SQLALCHEMY_DATABASE_URI=sqlite:///quiz_master.db
ADMIN_USERNAME= admin@quiz.com
ADMIN_PASSWORD= admin123
FLASK_APP=app.py
```

5. Create the database:

```bash
flask --app run.py db create
```

6. Seed the database:

```bash
flask --app run.py db seed
```

7. Run the application

```bash
python run.py
```

This will run the app locally on `http://127.0.0.1:5000`.

## Milestones

### Milestone 0: GitHub Repository Setup (Mandatory)
- Create a private GitHub repository for the project.
- Add a README.md file with a basic project description.
- Set up a .gitignore file to exclude unnecessary files.
- Commit and push the initial setup to the repository.
- **Git Commit Message:** Initialized private GitHub repository with README and .gitignore

---

### Milestone 1: Database Models and Schema Setup


- Define tables for User, Admin, Subject, Chapter, Quiz, Question, Score, etc., in SQLite.
- Set up relationships between tables (e.g., Subjects have multiple Chapters, Quizzes belong to Chapters).
- Ensure the database is programmatically created through a Python script/file.
- **Git Commit Message:** Created database schema for users, subjects, quizzes, and scores

---

### Milestone 2: Authentication and Role Management


- Create an Admin login (Admin is predefined, no registration allowed).
- Implement User registration and login with required fields (username (email), password, full name, etc.).
- Users should be redirected to their respective dashboards after login.
- **Git Commit Message:** Implemented user registration and admin login functionality

---

### Milestone 3: Admin Dashboard and Management


- Admin should be able to:
  - Create/Edit/Delete Subjects.
  - Create/Edit/Delete Chapters under a subject.
  - Create/Edit/Delete Quizzes under a chapter.
  - Create/Edit/Delete Questions under a quiz.
- Admin should see a list of all users and their details.
- **Git Commit Message:** Built Admin dashboard with CRUD operations for subjects, chapters, quizzes, and questions

---

### Milestone 4: User Dashboard and Quiz Attempt System


- Users should see a list of available subjects and quizzes.
- Users should be able to attempt a quiz (MCQ format with one correct option).
- Implement a timer for each quiz.
- Users should get feedback on correct/incorrect answers after the quiz.
- Store quiz scores in the database.
- **Git Commit Message:** Developed User dashboard with quiz attempt functionality and timer

---

### Milestone 5: Score Management and Quiz Result Display


- Store quiz scores after submission.
- Users should see past quiz attempts and scores.
- Display a quiz summary report with total scores.
- **Git Commit Message:** Implemented score tracking and quiz result display

---

### Milestone 6: Search Functionality for Admin and Users


- **Admin Search:**
  - Admin can search for users, subjects, quizzes, and questions.
- **User Search:**
  - Users can search for subjects and quizzes.
- **Git Commit Message:** Added search functionality for Admin and Users

---

### Milestone 7: Quiz Time and Duration Management


- Admin should set date and time duration (HH:MM) when creating a quiz.
- Users should only be able to attempt quizzes within the given timeframe.
- **Git Commit Message:** Implemented quiz scheduling with time duration

---

### Milestone 8: API Development for Data Access

- Develop API endpoints to fetch subjects, chapters, quizzes, and scores.
- Ensure APIs return JSON responses.
- **Git Commit Message:** Created API endpoints for subjects, quizzes, and scores

---

### Milestone 9: Summary Charts and Data Visualization

- Display quiz performance charts for users.
- Admin should see summary statistics of quizzes and users.
- **Git Commit Message:** Added summary charts for quiz statistics and user performance

---

### Milestone 10: Frontend Enhancements and UI Improvements

- Improve UI with Bootstrap and CSS.
- Implement frontend validation for forms.
- Ensure the app is mobile-responsive.
- **Git Commit Message:** Enhanced UI with Bootstrap styling and form validation

---

### Milestone 11: Security Enhancements and Final Testing

- Implement backend validation for form inputs.
- Perform final testing to fix any bugs or security loopholes.
- Ensure all routes are protected based on user roles.
- **Git Commit Message:** Enhanced security with backend validation and finalized testing

---