<div align="center">

# 🏫 AdmitSchool
### Online Admission Management System

**v2.6 · Academic Session 2026–27**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS_v3-06B6D4?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript_ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![No Backend](https://img.shields.io/badge/Backend-None_Required-brightgreen?style=for-the-badge)
![Single File](https://img.shields.io/badge/Distribution-Single_HTML_File-blueviolet?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

*A complete, browser-based school admission management system — no server, no installation, just open and go.*

---

</div>

## 📖 Overview

**AdmitSchool** is a fully self-contained, single-file web application that digitizes the entire school admission lifecycle — from online application submission to enrollment confirmation. Built entirely with frontend technologies, it runs directly in any modern browser with zero configuration.

Designed for school administrators, staff, and applicants, AdmitSchool provides a polished, production-ready experience powered by localStorage persistence and a role-based access control system.

---

## ✨ Features

### 🖥️ Admin Dashboard
- KPI summary cards showing real-time application metrics
- Application funnel visualization across status stages
- Quick-access application tracker

### 📝 Multi-Step Application Wizard
- 4-step guided form: **Personal Info → Academic Details → Document Upload → Review & Submit**
- Input validation at each step before progression
- Auto-generated Application ID on submission

### 📋 Application Listing & Search
- Filterable table by status, course, and sort order
- Global search across name, application ID, and course
- Inline status indicators with color coding

### 🔍 Application Review Module
- Side-by-side detailed applicant view
- Full status change workflow with audit trail
- Reviewer comments and notes system

### 📄 Document Verification Center
Track 6 required documents per applicant:
| # | Document |
|---|----------|
| 1 | 📷 Passport Photo |
| 2 | 📜 Birth Certificate |
| 3 | 📊 Previous Marksheet |
| 4 | 🏫 Transfer Certificate |
| 5 | 🪪 Identity Proof |
| 6 | 👨‍👩‍👧 Parent's ID Proof |

### 📅 Entrance Exam Scheduling
- Schedule per-course entrance exams
- Configure date, time, venue, maximum marks, and cutoff scores

### 🏆 Merit List Generation
- Configurable weighted scoring formula
- Adjustable weights for academic percentage vs. entrance exam score
- Downloadable merit table

### 💰 Fee Management
- Fee structure defined per course
- Simulated payment processing
- Printable receipt generation

### 🎓 Admission Confirmation
- Unique enrollment number assignment
- Offer letter generation with full print support

### 📊 Reports & Analytics
- CSV data export
- Printable summary reports

### 🎒 Student Self-Service Portal
Applicant-facing modules:
- My Dashboard · Application Form · Documents · Exam Status · Fee Payment · Offer Letter

### 🔐 Role-Based Access Control (RBAC)
Three distinct roles with scoped permissions

### 📬 Simulated Email Notifications
- In-app toast notifications
- Email outbox simulation for tracking sent communications

### 🌙 Dark / Light Theme
- Fully responsive design
- One-click dark mode toggle

### 💾 LocalStorage Persistence
- All data persists across browser sessions
- One-click demo data reset for fresh walkthroughs

---

## 🖼️ Screenshots

> *Screenshots are captured from the live application. Open the HTML file in your browser to explore all views.*

| View | Description |
|------|-------------|
| 📊 **Dashboard** | KPI cards, funnel chart, quick tracker |
| 🧙 **Application Wizard** | 4-step guided form with validation |
| 📋 **Applications List** | Filterable, searchable table |
| 🔍 **Review Module** | Side-by-side applicant detail & status workflow |
| 📄 **Document Center** | Per-applicant document checklist |
| 🏆 **Merit List** | Weighted score table |
| 💰 **Fee & Receipt** | Payment simulation and printable receipt |
| 🎒 **Student Portal** | Self-service applicant dashboard |

---

## 🛠️ Technology Stack

| Technology | Role |
|---|---|
| **HTML5** | Single-file, self-contained application shell |
| **Tailwind CSS v3** (CDN) | Utility-first styling and responsive layout |
| **Vanilla JavaScript ES6+** | Application logic, state management, routing |
| **Phosphor Icons** (CDN) | Icon library |
| **Google Fonts: Inter + Plus Jakarta Sans** | Typography |
| **Browser localStorage API** | Client-side data persistence |

> **Zero dependencies to install.** All external libraries are loaded from CDN at runtime.

---

## 🚀 Getting Started

### Requirements

- Any modern browser: **Chrome**, **Firefox**, **Edge**, **Safari** (2022+)
- No Node.js, no Python, no server — nothing to install

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/admitschool.git

# Navigate into the project folder
cd admitschool
```

### Running the App

```
Simply open the file in your browser:
```

**Windows:**
```powershell
start admitschool_admission_management_system.html
```

**macOS:**
```bash
open admitschool_admission_management_system.html
```

**Linux:**
```bash
xdg-open admitschool_admission_management_system.html
```

Or just **double-click** the `.html` file in your file explorer. That's it! 🎉

---

## 📚 Usage Guide

### Default Login

When you open the app, you are automatically logged in as:

| Field | Value |
|-------|-------|
| **Role** | Admin |
| **Name** | Dr. S. Radhakrishnan |
| **Title** | Principal |

Switch roles at any time using the **role switcher** in the top navigation bar or via the **Login** button.

---

### 👑 Admin Role

Full access to all modules.

| Task | How To |
|------|--------|
| View KPIs & funnel | Navigate to **Dashboard** |
| Review applications | Go to **Applications → Review** |
| Verify documents | Open **Document Verification Center** |
| Schedule an exam | Go to **Entrance Exam Scheduling** |
| Generate merit list | Navigate to **Merit List**, configure weights, click Generate |
| Manage fees | Open **Fee Management**, select applicant, record payment |
| Issue offer letter | Go to **Admission Confirmation**, assign enrollment number |
| Export data | Navigate to **Reports & Analytics → Export CSV** |
| Reset demo data | Click **"Reset Demo Data"** in the sidebar |

---

### 🧑‍💼 Staff Role

Scoped to verification and scoring tasks.

| Task | Access |
|------|--------|
| Verify uploaded documents | ✅ Full access |
| Enter entrance exam scores | ✅ Full access |
| Review and add comments | ✅ Full access |
| Change application status | ✅ Limited (Submitted → Under Review → Shortlisted) |
| Fee management | ❌ No access |
| Admission confirmation | ❌ No access |
| Reports export | ❌ No access |

---

### 🎒 Applicant Role

Self-service portal for the student/parent.

| Task | Access |
|------|--------|
| Submit new application | ✅ Full access |
| Upload documents | ✅ Full access |
| View application status | ✅ Own application only |
| View exam schedule | ✅ Read-only |
| Pay admission fee | ✅ Simulated payment |
| Download offer letter | ✅ When admitted |
| View other applicants | ❌ No access |

---

## 🎓 Course & Fee Structure

| Course | Board | Annual Fee | Seats |
|--------|-------|-----------|-------|
| Class 1–10 | CBSE | ₹52,000 | 40 |
| Class 1–10 | ICSE | ₹56,500 | 40 |
| Class 1–10 | State Board | ₹29,000 | 50 |
| 11th Science | — | ₹77,000 | 35 |
| 11th Commerce | — | ₹62,000 | 35 |
| 11th Arts | — | ₹49,500 | 30 |

---

## 🔄 Application Status Workflow

```
                        ┌─────────────┐
                        │  Submitted  │  ← Applicant submits form
                        └──────┬──────┘
                               │
                               ▼
                        ┌─────────────┐
                        │ Under Review│  ← Staff begins review
                        └──────┬──────┘
                               │
                               ▼
                        ┌─────────────┐
                        │ Shortlisted │  ← Meets eligibility criteria
                        └──────┬──────┘
                               │
                               ▼
                        ┌─────────────┐
                        │  Merit List │  ← Ranked by weighted score
                        └──────┬──────┘
                               │
                    ┌──────────┴──────────┐
                    │                     │
                    ▼                     ▼
             ┌──────────┐         ┌──────────────┐
             │ Admitted │         │   Rejected   │
             └──────────┘         └──────────────┘
                    │
                    ▼
        Enrollment Number Assigned
        Offer Letter Generated & Sent
```

---

## 🔐 RBAC Permissions Table

| Module | Admin | Staff | Applicant |
|--------|:-----:|:-----:|:---------:|
| Dashboard | ✅ | ✅ | ✅ (own) |
| Application Form | ✅ | ✅ | ✅ |
| Application List (all) | ✅ | ✅ | ❌ |
| Application Review | ✅ | ✅ | ❌ |
| Status Change (full) | ✅ | ⚠️ Limited | ❌ |
| Document Verification | ✅ | ✅ | ❌ |
| Document Upload | ✅ | ✅ | ✅ (own) |
| Exam Scheduling | ✅ | ❌ | ❌ |
| Exam Score Entry | ✅ | ✅ | ❌ |
| Merit List Generation | ✅ | ❌ | ❌ |
| Fee Management | ✅ | ❌ | ❌ |
| Fee Payment | ✅ | ❌ | ✅ (own) |
| Admission Confirmation | ✅ | ❌ | ❌ |
| Offer Letter | ✅ | ❌ | ✅ (own) |
| Reports & CSV Export | ✅ | ❌ | ❌ |
| Reset Demo Data | ✅ | ❌ | ❌ |

> ⚠️ Staff can move status from **Submitted → Under Review → Shortlisted** only.

---

## 📁 Project Structure

```
ADMIT/
└── admitschool_admission_management_system.html   # Entire application (~208 KB, ~3,600 lines)
```

The single HTML file contains:

```
admitschool_admission_management_system.html
├── <head>          CDN imports (Tailwind CSS, Phosphor Icons, Google Fonts)
├── <style>         Custom CSS, dark mode overrides, print styles
└── <body>
    ├── #app        Root mount point
    └── <script>    Entire application (~3,400 lines of Vanilla JS)
                    ├── State management (localStorage)
                    ├── RBAC engine
                    ├── Router / view renderer
                    ├── Dashboard module
                    ├── Application wizard
                    ├── Applications list & search
                    ├── Review module
                    ├── Document verification
                    ├── Exam scheduling
                    ├── Merit list generator
                    ├── Fee management
                    ├── Admission confirmation
                    ├── Reports & export
                    ├── Student portal
                    ├── Notification / email outbox
                    └── Demo data seed
```

---

## 🧪 Demo Data

The application ships with **12 pre-loaded demo applicants** from across India, spanning all available courses and status stages. This lets you explore the full workflow immediately.

To reset to the original demo state at any time:
> Click **"Reset Demo Data"** in the sidebar menu.

---

## 🤝 Contributing

Contributions are welcome! Since this is a single-file application, please keep changes self-contained.

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/your-feature-name`
3. **Commit** your changes: `git commit -m "feat: add your feature"`
4. **Push** to your branch: `git push origin feature/your-feature-name`
5. **Open** a Pull Request

### Guidelines

- Keep the app **single-file** — do not split into separate JS/CSS files
- Maintain **Tailwind CDN** usage (no build step)
- Test across **Chrome, Firefox, and Edge** before submitting
- Add demo data entries if the feature requires new data structures
- Document any new localStorage keys in the PR description

---

## 📄 License

This project is licensed under the **MIT License**.

```
MIT License

Copyright (c) 2026 AdmitSchool

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

<div align="center">

Made with ❤️ for schools embracing digital admissions

**[⭐ Star this repo](https://github.com/your-username/admitschool)** if you find it useful!

</div>
