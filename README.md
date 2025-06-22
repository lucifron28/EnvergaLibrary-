
# 📚 EnvergaLibrary++

EnvergaLibrary++ is a modernized, full-stack, open-source university library management system and student engagement platform. Built with Next.js, Django, and PostgreSQL, it aims to digitize the borrowing process, enhance student interaction through community features, and automate library workflows with intelligent tools like QR-based reservations and AI-powered assistance.

---

## 🎯 Project Vision

Create a centralized and intelligent platform that:
- Simplifies book borrowing with account-based QR codes
- Tracks due dates and handles penalties automatically
- Encourages student engagement with reviews, blogs, and discussions
- Supports librarians in managing books, events, and analytics
- Simulates a real-world open-source project for student contributors

---

## ⚙️ Tech Stack

| Area       | Tech                          |
|------------|-------------------------------|
| Frontend   | Next.js, TailwindCSS, shadcn/ui |
| Backend    | Django + Django REST Framework |
| Database   | PostgreSQL                    |
| Auth       | Django AllAuth or NextAuth.js |
| AI Bot     | OpenAI API (Athena Bot)       |
| Email      | Mailgun / SendGrid / SMTP     |
| QR Codes   | Python `qrcode` lib + token logic |
| Hosting    | Vercel (frontend), Railway/Render (backend) |
| CI/CD      | GitHub Actions                |

---

## 📌 Core Features

### Student System
- Verified registration via student ID
- Profile with borrowing history and penalties
- Login with secure JWT/session management

### Library System
- Add/edit/remove books (admin)
- Real-time availability tracking
- QR reservation (30-min expiration window)
- Borrow and return management

### Due Dates & Fines
- Borrowing deadline notifications via email
- Automatic fine calculation for overdue returns
- Admin overrides and balance tracking

### Athena — AI Librarian
- Book recommendations
- Dewey Decimal explanations
- Intelligent search assistance

### Community Features
- Book reviews & rating
- Blog posts and threaded discussions
- Upvotes & comments

### Event Management
- Contest posting (e.g., Book Spine Poetry)
- RSVP/entry submissions
- Voting and galleries (optional)

### Admin Interface
- Dashboard with statistics: borrowing trends, popular books
- Book and user management
- Event and submission manager
- Export to PDF/CSV for reporting

---

## Database Overview

Main tables include:
- `User` (with roles: student, admin)
- `Book`, `Borrow`, `Reservation`
- `Review`, `Post`, `Comment`
- `Event`, `Submission`
- `PenaltyLog`

---

## 👥 Contributing

EnvergaLibrary++ is a **community-first project**. Students can:
- Learn full-stack development
- Collaborate via GitHub PRs
- Get code reviewed by maintainers
- Simulate a real-world SDLC

> We follow GitHub Flow and use clear labels, milestones, and reviews.

---

## 🧭 Project Setup

### 1. Clone the repo

```bash
git clone https://github.com/your-org/EnvergaLibrary-.git
```

### 2. Frontend (Next.js)

```bash
cd frontend
npm install
npm run dev
```

### 3. Backend (Django)

```bash
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### 4. Environment Files

`.env.example` will be provided for:
- `DATABASE_URL`
- `EMAIL_BACKEND`
- `OPENAI_API_KEY`
- `FRONTEND_URL`
- `SECRET_KEY`

---

## 📌 GitHub Planning Board

| Column             | Description |
|--------------------|-------------|
| 💡 Ideas / Backlog | Feature suggestions or improvements |
| 📋 To Do           | Approved and scoped tasks |
| 🛠 In Progress     | Currently active work |
| 🔍 In Review       | Open pull requests for review |
| ✅ Done            | Completed tasks |
| 🐞 Bugs            | Reported and reproducible issues |

---

## 🏷 GitHub Labels

| Label          | Description |
|----------------|-------------|
| `frontend`     | Next.js / Tailwind tasks |
| `backend`      | Django / PostgreSQL |
| `api`          | REST API issues |
| `bug`          | Errors and regressions |
| `feature`      | New feature requests |
| `documentation`| Docs, readme, setup |
| `good first issue` | Easy, beginner-friendly tasks |
| `needs review` | Needs code review |
| `blocked`      | Waiting on something |

---

## Milestones

- In progress
---

## ✨ Contributors Guide

1. Fork the repo
2. Clone and make your changes
3. Create a feature branch (`feature/feature-name`)
4. Submit a PR and request review

Please follow our [Code of Conduct](./CODE_OF_CONDUCT.md) and [Contributing Guide](./CONTRIBUTING.md).

---

## 📜 License

MIT — Free to use and modify for educational purposes.