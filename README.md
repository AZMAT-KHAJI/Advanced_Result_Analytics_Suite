# Advanced Result Analytics Suite

An academic result analysis platform built with Django that helps institutions process, analyze, and visualize student performance data through interactive dashboards and automated reports.

**🏆 Winner - Build for Campus, Django Semi-Hackathon 2026**
*Department of Computer Science and Engineering, SJB Institute of Technology, Bengaluru*

---

## Table of Contents

- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [System Design](#system-design)
- [Installation](#installation)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Contributors](#contributors)
- [Roadmap](#roadmap)
- [Acknowledgements](#acknowledgements)

## About

Manually analyzing semester-wise student results is slow and error-prone, and it rarely surfaces the patterns that matter — which students are at risk, which subjects are underperforming, and how branches or batches compare over time.

This project was built to solve that problem. It ingests raw result data, processes it with Pandas, stores it in MySQL, and exposes it through a Django-powered dashboard so faculty and administrators can query performance trends without touching a spreadsheet.

## Features

- Interactive dashboards for semester-wise and subject-wise performance
- Branch and batch-level comparison views
- Backlog tracking and early-risk flagging for at-risk students
- Category and parameter-based comparative analytics
- One-click report generation and export
- Role-based access for faculty and admin views

## Tech Stack

- **Backend:** Django, Python
- **Data Processing:** Pandas
- **Database:** MySQL
- **Frontend:** HTML, CSS, JavaScript
- **Charts:** Chart.js

## System Design

```
Raw Result Data (CSV/Excel)
        │
        ▼
  Data Ingestion Layer
        │
        ▼
  Preprocessing (Pandas)
        │
        ▼
   MySQL Database
        │
        ▼
  Django Backend (Analytics Logic)
        │
        ▼
  Chart.js Dashboards + Reports
```

## Installation

```bash
git clone https://github.com/AZMAT-KHAJI/Advanced_Result_Analytics_Suite.git
cd Advanced_Result_Analytics_Suite

python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate

pip install -r requirements.txt
```

Update your MySQL credentials in `settings.py`, then:

```bash
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

Visit `http://127.0.0.1:8000` to access the application.

## Usage

1. Log in as admin and upload result datasets.
2. The system automatically cleans and structures the data.
3. Navigate to the dashboard to view performance trends, backlog reports, and comparative charts.
4. Export reports directly from the dashboard as needed.

## Screenshots



## Contributors

| Name | Role |
|---|---|
| Azmat Khaji | Backend (Django), Deployment |
| @Chaithanya | *Add role* |
| @Veena reddy | *Add role* |

## Roadmap

- [ ] Additional performance prediction models
- [ ] PDF export for reports
- [ ] Improved role-based permissions
- [ ] Deployment to production environment for department use

## Acknowledgements

Built as part of the Build for Campus – Django Semi-Hackathon 2026, organized by the Department of Computer Science and Engineering, SJB Institute of Technology, Bengaluru. Thanks to our faculty and the organizing committee for the opportunity.
