# Student Admissions Dashboard (Streamlit)

A lightweight **Streamlit + Plotly** dashboard for exploring **university admissions and student outcomes** over time. The app loads a CSV dataset, normalizes percentage fields, and provides interactive filters and visualizations for admissions, enrollment, retention, and satisfaction.

## What this app includes

### Interactive filters
- Sidebar dropdowns to filter by **Year** and **Term** (Spring/Fall). :contentReference[oaicite:1]{index=1}

### KPI summary
- Key indicators displayed as metrics for:
  - **Fall (all years):** Total Applications, Total Admitted, Total Enrolled
  - **Spring (all years):** Total Applications, Total Admitted, Total Enrolled :contentReference[oaicite:2]{index=2}

### Visual analytics
- **Enrollment Year-over-Year** (bar chart) :contentReference[oaicite:3]{index=3}  
- **Enrollment by Department** (donut chart) :contentReference[oaicite:4]{index=4}  
- **Retention & Student Satisfaction trends over time** (line chart) :contentReference[oaicite:5]{index=5}  
- **Spring vs. Fall trends** for retention & satisfaction (line chart, colored by term) :contentReference[oaicite:6]{index=6}  
- **Department-wise enrollment trends** (grouped bar chart) :contentReference[oaicite:7]{index=7}  

### Built-in “Key Findings”
The dashboard includes a short insights section summarizing observed patterns (e.g., department growth and term-based retention differences). :contentReference[oaicite:8]{index=8}

---

## Tech stack

- Streamlit :contentReference[oaicite:9]{index=9}
- Pandas :contentReference[oaicite:10]{index=10}
- Plotly :contentReference[oaicite:11]{index=11}
- Matplotlib (installed as dependency support) :contentReference[oaicite:12]{index=12}

---

## Project structure

The app expects the CSV and logo to be in the same folder as `Question2.py`. :contentReference[oaicite:13]{index=13}

---

## Dataset schema

The dataset contains admissions + outcomes by year/term, plus departmental enrollment breakdown:

- Year
- Term
- Applications
- Admitted
- Enrolled
- Retention Rate (%)
- Student Satisfaction (%)
- Engineering Enrolled
- Business Enrolled
- Arts Enrolled
- Science Enrolled :contentReference[oaicite:14]{index=14}

**Note:** The app converts Retention Rate and Student Satisfaction from percent to proportions (divides by 100) before plotting. :contentReference[oaicite:15]{index=15}

---

## Setup & Run locally

### 1) Create and activate a virtual environment (recommended)
```bash
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate
