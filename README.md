# Churn_Project – HR / People Analytics Simulation

This project simulates a small **People Analytics / HR churn pipeline** using synthetic Workforce HR–style data. It shows how to go from raw HR exports to a **master employee table** and **monthly churn metrics** that could feed a dashboard or predictive model.

---

## 💼 Business Question

> “How is employee churn trending over time by department, and how long do employees typically stay before leaving?”

The repository demonstrates the core data-engineering and analytics steps that a People Analytics Specialist might perform using data from systems like Workday or Workforce HR.

---

## 📂 Repository Structure

```text
Churn_Project/
├── data/
│   ├── workforce_employees.csv          # Employee roster with hire/term dates, dept, job family, etc.
│   ├── workforce_status_history.csv     # Timeline of status changes (Hire, Active, Terminated)
│   ├── workforce_departments.csv        # Department dimension (id → name)
│   └── workforce_employees_api.json     # Mock API metadata with extraction timestamp
├── notebooks/
│   └── 01_data_ingest.ipynb             # Main notebook: builds master employee table + churn metrics
├── src/
│   └── (reserved for reusable Python modules later)
└── .gitignore
