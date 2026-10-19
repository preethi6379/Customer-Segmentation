# 🛍️ Customer Segmentation with K-Means & PCA

An end-to-end unsupervised machine learning and business analytics project to segment retail customers based on demographics, annual income, and spending behavior, translating algorithmic clusters into actionable marketing strategies.

---

## 📌 Project Overview
Treating all customers the same leads to wasteful marketing budgets and missed conversion opportunities. By combining **Principal Component Analysis (PCA)** for dimensionality reduction and **K-Means Clustering**, this project groups customers into distinct behavioral segments and builds tailored marketing personas.

---

## 📂 Project Structure

```text
Customer Segmentation/
│
├── data/
│   └── raw/
│       └── Mall_Customers.csv    # Raw dataset (200 customers, 5 features)
│
├── notebooks/
│   └── 01data.ipynb              # EDA, data cleaning, and preprocessing
│
├── outputs/
│   ├── figures/                  # Saved distribution and cluster charts
│   └── reports/                  # Persona briefs and executive summaries
│
├── .gitignore                    # Git ignore file for Python & Jupyter
├── requirements.txt              # Environment dependencies
└── README.md                     # Project documentation
```

---

## 📊 Dataset Features
- **`CustomerID`**: Unique identifier (dropped for modeling).
- **`Gender`**: Customer gender (`Female: 0`, `Male: 1`).
- **`Age`**: Customer age (18 to 70 years).
- **`Annual Income (k$)`**: Annual earnings in thousands of dollars ($15k to $137k).
- **`Spending Score (1-100)`**: Spending propensity score assigned by mall behavior analytics.

---

## 🚀 Progress & Workflow

### Completed:
- [x] **Project Architecture & Setup**: Structured repository with data, notebooks, and output directories.
- [x] **Data Ingestion & Integrity Checks**: Confirmed 0 null values, 0 duplicates, and validated column types.
- [x] **Exploratory Data Analysis (EDA)**: Analyzed feature distributions and identified initial clustering patterns in Income vs. Spending Score.
- [x] **Data Preprocessing & Scaling**: Encoded categorical features and standardized numerical attributes using `StandardScaler` ($\mu = 0, \sigma = 1$).

### Coming Up (Day 2):
- [ ] **PCA Dimensionality Reduction**: Analyze explained variance ratio, scree plot, and component loadings.
- [ ] **Optimal Cluster Evaluation**: Determine optimal $k$ using the Elbow Method (WCSS) and Silhouette Analysis.
- [ ] **K-Means Modeling & 2D Projection**: Segment customers and visualize distinct clusters in PCA space.
- [ ] **Customer Persona Profiling**: Calculate mean statistics per cluster and assign descriptive personas (e.g., *VIP Spenders*, *Frugal Savers*).
- [ ] **Executive Business Storytelling**: Formulate tailored marketing campaigns and ROI projections for each segment.

---

## 🛠️ Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone <your-repo-url>
   cd "Customer Segmentation"
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter:**
   ```bash
   jupyter notebook
   ```
