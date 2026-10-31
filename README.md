# 🏪 Custom Sales Tracking CRM

> A full-stack, custom-built CRM for managing leads, tracking the sales pipeline, and reporting on conversion performance — built from scratch with Python and PostgreSQL.

---

## 🎯 Problem Solved

A sales team was tracking leads in spreadsheets. Deals were being lost, follow-ups missed, and there was zero visibility into pipeline health. Built a lightweight CRM tailored to their exact workflow.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python, FastAPI |
| Database | PostgreSQL |
| Frontend | Streamlit |
| Auth | JWT tokens |
| Reporting | Pandas + Matplotlib |

---

## ⚡ Key Features

- **Lead management** — create, assign, update, close leads
- **Pipeline stages** — New → Contacted → Qualified → Proposal → Won/Lost
- **Activity logging** — every call, email, meeting tracked
- **Follow-up reminders** — auto-flags leads with no activity in N days
- **Sales reports** — conversion rate, avg deal time, rep performance
- **Role-based access** — Admin, Sales Manager, Sales Rep views

---

## 📊 Dashboard Views

- **Pipeline Kanban** — drag-and-drop leads across stages
- **Revenue forecast** — weighted pipeline value by probability
- **Rep leaderboard** — deals closed per salesperson
- **Activity feed** — real-time log of all team actions

---

## 🚀 Setup

```bash
git clone https://github.com/syed-fahad-fazal/sales-crm-custom
cd sales-crm-custom
pip install -r requirements.txt
cp .env.example .env
# Set your PostgreSQL credentials in .env
python -m app.db.init_db     # Initialize database
uvicorn app.main:app --reload # Start API
streamlit run frontend/app.py  # Start UI
```

---

## 📁 Project Structure

```
sales-crm-custom/
├── app/
│   ├── api/          — FastAPI routes (leads, contacts, reports)
│   ├── models/       — SQLAlchemy ORM models
│   ├── services/     — Business logic
│   └── db/           — Database setup + migrations
├── frontend/
│   └── app.py        — Streamlit UI
├── requirements.txt
├── .env.example
└── README.md
```

---

*Built by [Syed Fahad Fazal](https://linkedin.com/in/syed-fahad-fazal) — Freelance AI & Python Developer*
