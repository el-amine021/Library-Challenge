# 📚 Airbus Data Management & Governance Challenge

Welcome to my submission for the Airbus Data Management & Data Governance technical challenge. This project simulates the design of a diverse, high-circulation library catalog for an international English-language school. It leverages public data, strong data governance practices, and visualization tools to deliver an end-to-end solution.

---

## 🌟 Challenge Objective

**Scenario:**  
An international school wants to launch a physical and digital English-language library with **5,000 unique titles**. The primary goal is to **maximize diversity** (genre & author nationality) while ensuring **high circulation potential**.

---

## 🧠 What This Project Demonstrates

- ✅ **Resourcefulness:** Merged & enriched public datasets from Kaggle and Wikipedia API  
- ✅ **Data Governance:** Cleaned, structured, and transformed data with traceability  
- ✅ **Problem Solving:** Multi-objective scoring & quota-based selection strategy  
- ✅ **Proactiveness:** Interactive Streamlit dashboard for visualization & exploration  
- ✅ **Communication:** Clear indicators, visuals, and written explanation of decisions  

---

## 📂 Repository Structure

```
Airbus_Challenge/
│
├── app.py                        # Streamlit dashboard for book selection
├── CHALLENGE_FINAL_VERSION.ipynb# Full notebook with data cleaning, scoring, selection
├── BOOKS_DATASET.csv            # Cleaned & enriched dataset (~9,800 books)
├── BOOKS_DATASET_final.csv      # Final dataset after scoring and filtering
├── selection_books.csv          # Final 5,000 book selection
├── Airbus Data Management & Governance challenge.pdf  # Final report
```

---

## ✅ Success Criteria

### Qualitative Indicators:
- Diversity of genres and author nationalities
- Accessibility of books (physical and digital)
- User satisfaction via feedback or surveys

### Quantitative KPIs:
- ~200–400 borrowings/month
- ≥30 different author nationalities
- ≥10% representation per genre
- ~200 active users/month
- 500 new titles added annually (renewal rate)

---

## 🔢 Scoring System

Each book was scored based on:
- **Popularity Score:** Normalized rating and to-read count  
- **Diversity Score:** Genre and nationality coverage  
- **Price Efficiency Score:** Value per euro spent  
- **Recency Score:** Publication year weighting  

A **weighted average** of these scores was used to rank books.

---

## 📊 Visualizations & Dashboard

Built with **Streamlit** and **Plotly**, the dashboard includes:
- Score distribution
- Genre and nationality diversity
- Score vs. publication year trends
- Budget overview and final selection

💡 Interactive tabs and export options enhance usability.

---

## 💰 Budget Estimate

| Expense Category          | Estimated Cost |
|--------------------------|----------------|
| Physical Books           | €23,000         |
| Infrastructure           | €10,000         |
| Digital Licenses         | €15,000         |
| Staff/Volunteers         | €8,000          |
| Digital Management System| €5,000          |
| Maintenance & Software   | €5,000          |
| **Total**                | **€66,000**     |

---

## 🔗 Data Sources

| Source               | Description                      | Access Method |
|----------------------|----------------------------------|---------------|
| Kaggle Datasets      | Book metadata, ratings, tags     | CSV Download  |
| Wikipedia API        | Author nationality enrichment    | API Call      |

---

## 🔧 Data Transformations

| Transformation       | Description                                         | Tool     |
|----------------------|-----------------------------------------------------|----------|
| Deduplication        | Removed duplicates using ISBN + title + author     | Pandas   |
| Filtering            | Removed non-English books and outliers             | Pandas   |
| Imputation           | Filled missing prices by genre average             | Pandas   |
| Scoring              | Added KPIs and normalized scores                   | Pandas   |
| Grouping             | Applied quotas by genre, nationality, and age group| Pandas   |

---

## 🔁 Retrospective

### ✅ What Worked Well
- Seamless integration of public data and enrichment via API
- Clear scoring system and quota logic
- Engaging dashboard with user-friendly navigation

### 🔁 What I'd Do Differently
- Add simulated stakeholder voting to improve realism
- Further enrich metadata with additional APIs

### 🎓 What I Learned
- Multi-objective selection requires balance and creativity
- Importance of structured preprocessing for governance
- Streamlit + Plotly are powerful tools for storytelling

---

## 🧭 Apprenticeship Expectations

I’m excited to begin my **two-year apprenticeship in September 2025** as part of my Master’s program in Data Science and Engineering. I hope to:

- Apply my skills to real-world challenges
- Grow in data governance, ML, and pipeline development
- Contribute meaningfully to data-driven decision-making at Airbus

---

## 🚀 Run the Dashboard Locally

```bash
# Step 1: Install dependencies
pip install streamlit plotly pandas matplotlib seaborn

# Step 2: Run the app
streamlit run app.py
```

---

Thank you for reviewing my work!

**Author:** El Haitmy Amine  
**Contact:** amineelhaitmy@gmail.com
