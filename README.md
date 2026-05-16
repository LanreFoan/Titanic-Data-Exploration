#  Titanic Dataset — Exploratory Data Analysis

A clean, well-documented data exploration of the classic Titanic passenger dataset.  
The project walks through data cleaning, feature engineering, and visualisation to uncover the social and demographic patterns that determined survival.

---


##  What's Inside

### Data Cleaning

### Feature Engineering

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

##  Key Insights

1. Female passengers had a higher survival rate than males. We can suggest that the 'women and children first' evacuation protocol was rigorously followed.

2. 1st class Passengers had a higher survival rate. We can suggest they had better physical access to lifeboats and may have received preferential treatment.

3.  A 3rd-class woman ⁓50% survival had a higher chance of survival than a 1st-class man ⁓37%. Gender was an overriding factor of survival rather than class.

4.  Survivors paid higher fares on average than non-survivors. Since fare directly maps to passenger class, this reinforces finding #2.

5.  Passengers with family had a ~50% survival rate, compared to ~30% for solo travellers. Families, especially those with young children, may have been prioritised at lifeboats.

6. Survivors were only marginally younger on average ⁓28 years, than non-survivors ⁓30 years

---

##  Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| pandas | Data loading, cleaning, aggregation |
| NumPy | Numerical operations |
| Matplotlib | Custom plots and scatter charts |
| Seaborn | Statistical visualisations |
| Jupyter Notebook | Interactive analysis environment |

---


---

##  Dataset

The Titanic dataset is sourced from [Kaggle](https://www.kaggle.com/c/titanic).  

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).
