# ☀️ Solar Energy Production Zones Clustering
### New York State · Spinnaker Analytics Internship · Project 2

> Unsupervised machine learning pipeline to identify strategic solar energy production zones across New York State counties — using K-Means, Hierarchical, and DBSCAN clustering.

---

## 📌 Project Overview

This project applies **unsupervised machine learning** to cluster New York State counties into distinct solar energy production zones based on solar output characteristics. The goal is to support data-driven decision-making for solar energy investment and infrastructure planning.

**Organization:** Spinnaker Analytics  
**Role:** Data Analyst Intern  
**Scope:** End-to-end ML pipeline — data cleaning → EDA → feature engineering → modeling → evaluation → visualization

---

## 🗂️ Repository Structure

```
solar-clustering-project/
│
├── 📓 Solar_Clustering.ipynb       # Main Jupyter Notebook (full pipeline)
├── 📊 solar_dashboard.html         # Interactive HTML dashboard (Plotly)
├── 📁 data/
│   └── ny_solar_data.csv           # Cleaned county-level dataset
├── 📑 Solar_Zones_Report.pptx      # Executive PowerPoint presentation
└── README.md
```

---

## ⚙️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3 |
| Environment | Jupyter Notebook |
| Data Processing | Pandas, NumPy |
| Machine Learning | Scikit-learn |
| Visualization | Plotly, Matplotlib, Seaborn |
| Presentation | pptxgenjs, PowerPoint |

---

## 🔬 Methodology

### 1. Data Preparation
- Loaded and inspected raw New York State solar dataset
- Handled missing values and outliers
- Engineered **county-level aggregate features** for clustering

### 2. Feature Engineering & Normalization
- Selected key solar production indicators per county
- Applied **StandardScaler** normalization to ensure equal feature weighting

### 3. Clustering Algorithms Compared

| Algorithm | Key Parameter | Notes |
|---|---|---|
| **K-Means** | k = 4 | ✅ Best model — clear, interpretable zones |
| **Hierarchical** | Ward linkage | Used dendrogram to inform k selection |
| **DBSCAN** | ε, min_samples | Explored density-based groupings |

### 4. Model Selection
**K-Means with k=4** was selected as the best model based on:
- Silhouette Score comparison across algorithms
- Cluster interpretability and strategic meaningfulness
- Stability across multiple random seeds

---

## 🗺️ Results — 4 Strategic Solar Zones

The final K-Means model identified **4 distinct solar production zones** across New York State counties:

| Zone | Characteristics |
|---|---|
| 🟡 Zone 1 | High solar output — prime production counties |
| 🟠 Zone 2 | Moderate-high output — strong secondary candidates |
| 🔵 Zone 3 | Moderate output — developing potential |
| 🟣 Zone 4 | Lower output — limited solar suitability |

> 📊 Full interactive map and zone breakdown available in `solar_dashboard.html`

---

## 📦 Deliverables

- [x] **Jupyter Notebook** — complete ML pipeline with commentary
- [x] **CSV Dataset** — cleaned and processed county-level data
- [x] **HTML Dashboard** — interactive Plotly visualizations
- [x] **PowerPoint Presentation** — executive summary of findings

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/solar-clustering-project.git
   cd solar-clustering-project
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy scikit-learn plotly matplotlib seaborn jupyter
   ```

3. **Launch the notebook**
   ```bash
   jupyter notebook Solar_Clustering.ipynb
   ```

4. **View the dashboard**  
   Open `solar_dashboard.html` in any browser — no server required.

---

## 📈 Key Learnings

- Applied and compared **three unsupervised learning algorithms** on a real-world energy dataset
- Learned how **feature scaling** significantly impacts clustering outcomes
- Used **Silhouette Scores** and **dendrograms** for model evaluation without ground truth labels
- Translated ML results into **actionable geographic zones** for strategic energy planning

---

## 👤 Author

**Shijan**  
Data Analyst Intern @ Spinnaker Analytics  
📬 [LinkedIn](https://linkedin.com/in/your-profile) · [GitHub](https://github.com/your-username)

---

<p align="center">
  <sub>Built as part of a 6-month Data Analytics Internship at Spinnaker Analytics · Project 2 of 4</sub>
</p>
