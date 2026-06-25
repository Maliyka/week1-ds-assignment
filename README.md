# Week 1 Data Science Assignment
## Exploratory Data Analysis — Titanic Passenger Dataset

**Program:** Data Science Internship Program  
**Mentor:** Laiba Sattar (laeba0014@gmail.com)  
**Dataset:** [Titanic Passenger Data — Kaggle](https://kaggle.com/c/titanic/data)  
**Tool:** Google Colab / Jupyter Notebook

---

## 📋 Assignment Overview

This repository contains the complete Week 1 assignment for the Data Science Internship Program. The assignment covers:

- **Part A:** GitHub Setup & Submission *(this repo)*
- **Part B:** Dataset Selection — Titanic Passenger Data
- **Part C:** 7-Command First-Look Protocol
- **Part D:** 20+ Additional EDA Commands with Interpretations

---

## 📁 Repository Structure

```
week1-ds-assignment/
│
├── Week1_EDA_Titanic.ipynb   # Main Jupyter/Colab notebook (complete assignment)
├── README.md                  # This file
└── requirements.txt           # Python dependencies
```

---

## 🗂️ Dataset

| Property | Value |
|----------|-------|
| **Name** | Titanic Passenger Data |
| **Source** | [Kaggle](https://kaggle.com/c/titanic/data) / GitHub Raw |
| **Rows** | 891 |
| **Columns** | 12 |
| **Domain** | History / Social Science |
| **Target Variable** | `Survived` (0 = No, 1 = Yes) |

### Why Titanic?
The Titanic dataset was chosen because:
1. It is large enough for meaningful EDA (891 rows × 12 columns)
2. It contains a **rich mix of data types** (numeric, categorical, text)
3. It has real-world challenges: **missing values, outliers, class imbalance, and skewed distributions**
4. Every statistical finding connects to a **real historical event** — making interpretations meaningful
5. It is freely accessible without a Kaggle account via the GitHub raw URL used in the notebook

---

## 📓 Notebook Structure

The notebook (`Week1_EDA_Titanic.ipynb`) is organized into 4 sections:

### Section 1 — Dataset Introduction
- Which dataset and why it was chosen
- Column descriptions and domain context

### Section 2 — The 7-Command First-Look Protocol
| Command | Purpose |
|---------|---------|
| `df.shape` | Dataset dimensions |
| `df.dtypes` | Data types per column |
| `df.info()` | Non-null counts & memory usage |
| `df.describe()` | Statistical summary |
| `df.isnull().sum()` | Missing value counts |
| `df['col'].value_counts()` | Category frequencies |
| `df.duplicated().sum()` | Duplicate row detection |

### Section 3 — 20+ Additional EDA Commands
**15 Prescribed Commands Used:**
`df.head(10)` · `df.tail(5)` · `df.sample(15)` · `df.columns.tolist()` · `df.nunique()` · `df['col'].unique()` · `df.corr()` · `df['col'].hist(bins=20)` · `df.groupby().mean()` · `df['col'].value_counts(normalize=True)` · `df.select_dtypes(include='object')` · `df['col'].str.contains()` · `df.sort_values().head(5)` · `df[df['col'] > threshold]` · `pd.pivot_table()`

**5 Bonus Commands (Self-Explored):**
`df.skew()` · `df.kurt()` · `df['col'].mode()` · `df.memory_usage()` · `df.cov()`

**Total: 27 commands** with markdown interpretations after every single one.

### Section 4 — 3 Key Findings
1. **Survival was structured by class and gender** — 1st-class women: 97% vs. 3rd-class men: 14%
2. **Serious missing data** — Cabin (77%), Age (20%) require specific imputation strategies
3. **Fare column is severely skewed** — skewness 4.79, requires log transformation before modeling

---

## 🚀 How to Run

### Option 1 — Google Colab (Recommended)
1. Open [Google Colab](https://colab.research.google.com)
2. Click **File → Upload notebook**
3. Upload `Week1_EDA_Titanic.ipynb`
4. Click **Runtime → Run all**

The notebook loads the Titanic dataset directly from a public URL — **no file upload needed**.

### Option 2 — Jupyter Notebook (Local)
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/week1-ds-assignment.git
cd week1-ds-assignment

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook Week1_EDA_Titanic.ipynb
```

---

## 🛠️ Requirements

See `requirements.txt` for full list. Core dependencies:

| Library | Version | Purpose |
|---------|---------|---------|
| `pandas` | ≥ 1.5.0 | Data manipulation & EDA |
| `numpy` | ≥ 1.23.0 | Numerical computing |
| `matplotlib` | ≥ 3.6.0 | Plotting & histograms |
| `seaborn` | ≥ 0.12.0 | Statistical visualization |

---

## 📊 Key Visualizations in the Notebook

- **Missing Values Heatmap** — shows which columns and rows have NaN
- **Correlation Matrix Heatmap** — reveals feature relationships
- **Distribution Histograms** — Age, Fare, SibSp distributions
- **Survival Rate Bar Charts** — by Pclass and by Sex
- **Pivot Table Heatmap** — Survival rate by Sex × Pclass interaction

---

## ✅ Assignment Checklist

- [x] GitHub repository created and set to **Public**
- [x] Jupyter notebook (`.ipynb`) uploaded
- [x] All 7 First-Look Protocol commands implemented
- [x] 27 total EDA commands (exceeds 20+ minimum)
- [x] Markdown interpretation after **every** command
- [x] Notebook has clean section headers
- [x] 3 key findings written in plain English
- [x] `README.md` includes name and dataset
- [x] `requirements.txt` included
- [x] Repository link submitted to mentor

---

## 📬 Submission

Repository link submitted to: **laeba0014@gmail.com**

---

*"Always audit the data before you touch a model."* — Laiba Sattar
