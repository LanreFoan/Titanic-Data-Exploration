# 🚢 Titanic Dataset — Exploratory Data Analysis

A clean, well-documented data exploration of the classic Titanic passenger dataset.  
The project walks through data cleaning, feature engineering, and visualisation to uncover the social and demographic patterns that determined survival.

---

## 📁 Project Structure

```
├── Titanic-Data-Exploration.ipynb   # Main analysis notebook
├── Titanic-Dataset.csv              # Raw dataset
└── titanic_cleaned.csv              # Cleaned dataset (output)
```

---

## 🔍 What's Inside

### Data Cleaning
- **Missing values handled thoughtfully:**
  - `Age` (~20% missing) → imputed with the **median** to preserve distribution shape
  - `Cabin` (~77% missing) → **dropped** (too sparse to be useful)
  - `Embarked` (~0.2% missing) → two rows **removed** (negligible loss)
- **Duplicate check** confirmed: 0 duplicate rows

### Feature Engineering
- Created `family_size` = `SibSp + Parch + 1`  
- Created `family_group` = `"Alone"` or `"With Family"` for categorical analysis

### Exploratory Analysis & Visualisations
| Analysis | Key Finding |
|---|---|
| Survival by **Gender** | Women: ~74% survival vs Men: ~19% |
| Survival by **Class** | 1st: ~63% → 2nd: ~47% → 3rd: ~24% |
| Survival by **Gender × Class** | 3rd-class women (~50%) outlived 1st-class men (~37%) |
| **Fare** vs Survival | Survivors paid ~2× more on average |
| **Family** vs Solo travel | Families: ~51% survival vs Solo: ~30% |
| **Age** distribution | Minor effect; passengers were mostly young adults (20–40 yrs) |
| **Age vs Fare** scatter | High-fare passengers survived across all ages |

---

## 📊 Key Insights

1. **Gender was the dominant predictor.** The "women and children first" evacuation protocol was closely followed — female passengers survived at nearly 4× the rate of males.

2. **Class determined access to lifeboats.** Upper-deck placement, earlier alarm notification, and crew prioritisation gave 1st-class passengers a survival rate 2.6× higher than 3rd class.

3. **Gender beat class.** Even a 3rd-class woman had better survival odds (~50%) than a 1st-class man (~37%), showing gender overrode socioeconomic advantage.

4. **Fare acted as a proxy for wealth and class.** Survivors paid on average **£48** vs **£22** for non-survivors.

5. **Family presence helped.** Passengers travelling with family survived at ~51% — 21 percentage points higher than solo travellers (~30%).

6. **Age was a weak predictor on its own.** Mean age difference between survivors and non-survivors was less than 2 years.

> *The Titanic disaster was not random. Social hierarchy shaped survival to a striking degree — a sobering illustration of inequality under extreme circumstances.*

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| pandas | Data loading, cleaning, aggregation |
| NumPy | Numerical operations |
| Matplotlib | Custom plots and scatter charts |
| Seaborn | Statistical visualisations |
| Jupyter Notebook | Interactive analysis environment |

---

## ▶️ Getting Started

```bash
# Clone the repository
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# Launch the notebook
jupyter notebook Titanic-Data-Exploration.ipynb
```

---

## 📂 Dataset

The Titanic dataset is sourced from [Kaggle's Titanic competition](https://www.kaggle.com/c/titanic).  
It contains passenger information for 891 of the 2,224 people aboard, including demographics, ticket class, fare, and survival outcome.

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).
