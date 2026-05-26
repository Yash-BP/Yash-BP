# Yash Bhusari

Data Analyst — Python · SQL · Power BI · ETL Pipelines

I build automated data pipelines that connect raw, messy sources to clean, queryable outputs. Every project here solves a specific business problem: wasted software spend, manual invoice entry, or technology demand intelligence. The focus is always on pipelines that are production-ready, not just demo-grade.

LinkedIn: [yash-bhusari](https://www.linkedin.com/in/yash-bhusari)

---

## Projects

### [SubScan — SaaS Subscription Waste Analyzer](https://github.com/Yash-BP/subscan-saas-analyzer)

Identified $35,064 in annualised wasted software spend across a simulated 75-employee company.

The pipeline audits SaaS billing data using Python and SQL, flags zombie licenses (paid seats with no logins in 30 days) and terminated employee accounts still being billed, then exports the findings to a Power BI dashboard and Excel report. Finance teams get a prioritized cut-list with zero manual work.

**Stack:** Python · SQLite · Pandas · Power BI · python-dotenv  
**Highlights:** Relational database design, `.env`-driven business rules, timestamped execution audit logs, fully automated end-to-end run

---

### [Invoice OCR Automation Pipeline](https://github.com/Yash-BP/invoice-ocr-pipeline)

End-to-end ETL pipeline that eliminates manual invoice data entry for Indian SMEs.

Reads raw PDF invoices using pdfplumber, extracts structured fields (invoice ID, vendor, GST, grand total) via regex with built-in validation, loads the output into a SQLite database, and serves a live Streamlit + Plotly analytics dashboard. The pipeline is idempotent — safe to re-run at any time without data duplication.

**Stack:** Python · pdfplumber · Pandas · SQLite · Streamlit · Plotly · ReportLab · Faker · pytest  
**Highlights:** `run_pipeline.py` single-command orchestrator, `schema.sql` for explicit DB schema, unit tests, `failed_invoices.csv` for error tracking, `validation_passed` column per record

---

### [IBM Data Analyst: Automated ETL Pipeline](https://github.com/Yash-BP/IBM-Data-Analyst-Project)

Automated pipeline for collecting and visualizing global programming language demand and salary data.

Scrapes live salary data from IBM-hosted HTML datasets using BeautifulSoup, pulls real-time job posting counts for major technologies via JSON API endpoints, cleans and aggregates the data with Pandas, and generates production-ready demand charts. Includes persistent `pipeline.log` for execution health monitoring.

**Stack:** Python · Pandas · BeautifulSoup4 · Requests · Matplotlib · Seaborn  
**Highlights:** Live web scraping + API integration in a single pipeline, currency string cleaning, automated chart output

---

## Skills

| Area | Tools |
|---|---|
| Languages | Python 3.13, SQL |
| Data & ETL | Pandas, pdfplumber, BeautifulSoup4, Regex, Faker, ReportLab |
| Databases | SQLite, SQLite3 |
| Visualization | Power BI, Streamlit, Plotly, Matplotlib, Seaborn, Excel |
| Engineering | python-dotenv, pytest, Git, VS Code |

---

All projects are built around the same principle: automate the pipeline, surface the insight, make it repeatable.
