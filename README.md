# 🎓 Student Performance Analysis — Complete Data Science Project

## 📌 Project Overview

This project analyzes the **academic performance of students** using a real-world dataset
called `student-mat.csv`. The dataset contains information about **395 students** with
**33 different features** such as age, gender, family background, study habits, alcohol
consumption, and grades.

The goal of this project is to:
- Understand **what factors affect student grades**
- Visualize the data using **34+ charts and graphs**
- Build **7 machine learning models** to predict whether a student will **Pass or Fail**

---

## 📂 Dataset Information

| Detail | Value |
|---|---|
| File Name | student-mat.csv |
| Total Students | 395 |
| Total Columns | 33 |
| Subject | Mathematics |
| Source | UCI Machine Learning Repository |

### 📋 What Each Column Means

| Column | Meaning | Example Values |
|---|---|---|
| school | Which school the student goes to | GP, MS |
| sex | Gender of the student | M (Male), F (Female) |
| age | Age of the student | 15 to 22 |
| address | Where the student lives | U (Urban), R (Rural) |
| famsize | Family size | GT3 (more than 3), LE3 (less than 3) |
| Pstatus | Parents living together or apart | T (Together), A (Apart) |
| Medu | Mother's education level | 0 (none) to 4 (higher education) |
| Fedu | Father's education level | 0 (none) to 4 (higher education) |
| Mjob | Mother's job | teacher, health, services, at_home, other |
| Fjob | Father's job | teacher, health, services, at_home, other |
| reason | Why student chose this school | home, reputation, course, other |
| guardian | Who takes care of the student | mother, father, other |
| traveltime | Time to travel to school | 1 (< 15 min) to 4 (> 1 hour) |
| studytime | Weekly study time | 1 (< 2 hrs) to 4 (> 10 hrs) |
| failures | Number of past class failures | 0 to 4 |
| schoolsup | Extra school support | yes, no |
| famsup | Family educational support | yes, no |
| paid | Extra paid classes | yes, no |
| activities | Extra-curricular activities | yes, no |
| nursery | Attended nursery school | yes, no |
| higher | Wants higher education | yes, no |
| internet | Internet access at home | yes, no |
| romantic | In a romantic relationship | yes, no |
| famrel | Quality of family relationships | 1 (very bad) to 5 (excellent) |
| freetime | Free time after school | 1 (very low) to 5 (very high) |
| goout | Going out with friends | 1 (very low) to 5 (very high) |
| Dalc | Workday alcohol consumption | 1 (very low) to 5 (very high) |
| Walc | Weekend alcohol consumption | 1 (very low) to 5 (very high) |
| health | Current health status | 1 (very bad) to 5 (very good) |
| absences | Number of school absences | 0 to 93 |
| G1 | First period grade | 0 to 20 |
| G2 | Second period grade | 0 to 20 |
| G3 | Final grade ⭐ (Target column) | 0 to 20 |

> ⭐ **G3 is the most important column** — it is the final grade we are trying to predict.
> A student with G3 >= 10 is considered **PASSED**. G3 < 10 means **FAILED**.

---

## 🛠️ Tools & Technologies Used

| Tool | Purpose | Why We Use It |
|---|---|---|
| **Python** | Programming language | Easy to learn, powerful for data science |
| **Pandas** | Data handling | Load and clean CSV data like Excel |
| **NumPy** | Numbers & math | Fast mathematical calculations |
| **Matplotlib** | Basic charts | Create bar charts, pie charts, line graphs |
| **Seaborn** | Advanced charts | Beautiful statistical visualizations |
| **Plotly** | Interactive charts | Zoom, hover, 3D charts in browser |
| **Scikit-learn** | Machine learning | Build and test prediction models |
| **SciPy** | Statistics | T-test, ANOVA, Chi-square tests |
| **WordCloud** | Word clouds | Visual word frequency maps |
| **Missingno** | Missing data | Check for empty/null values visually |
| **Google Colab** | Run environment | Free cloud-based Python notebook |

---

## 📊 Complete List of plots which i have used in this project :
1.Seaborn plots
2.Matplotlib plots
3.Machine learning plots

1.
| Plot No. | Plot Type | What It Shows | Why It Is Useful |
|---|---|---|---|
| 1 | **Histplot** | How G1, G2, G3 grades are distributed | Shows if most students score high or low |
| 2 | **KDEplot** | Smooth curve of grade distribution by gender & internet | Compare patterns between groups |
| 3 | **Rugplot** | Small tick marks showing individual data points | See exactly where data points are |
| 4 | **Boxplot** | Min, max, median & outliers of grades | Find unusual/extreme grade values |
| 5 | **Violinplot** | Shape of grade distribution by study time | See how spread out grades are |
| 6 | **Barplot** | Average grade by mother's job & school reason | Which jobs/reasons lead to better grades |
| 7 | **Countplot** | How many students in each category | Understand data balance |
| 8 | **Scatterplot** | Relationship between G1 and G3 | Does first grade predict final grade? |
| 9 | **Lineplot** | Grade trends by study time and age | How grades change with study time |
| 10 | **Heatmap** | Color-coded correlation between all features | Which features are related to each other |
| 11 | **Pairplot** | All features plotted against each other | Quick overview of all relationships |
| 12 | **Regplot** | Regression line on scatter plot | Shows trend direction |
| 13 | **Stripplot & Swarmplot** | Individual student data points | See all actual data without overlap |
| 14 | **Boxenplot** | Enhanced boxplot for parent job categories | More detailed distribution shape |
| 15 | **Pointplot** | Average grade with error bars | Shows average with uncertainty range |
| 16 | **ECDFplot** | Cumulative percentage of grades | What % of students scored below a value |
| 17 | **Clustermap** | Grouped heatmap with hierarchical clustering | Find which features cluster together |
| 18 | **FacetGrid** | Multiple small plots by gender & address | Compare distributions across groups |
| 19 | **Residplot** | Errors in regression predictions | Check if regression model is a good fit |
| 20 | **LMplot** | Regression lines grouped by gender & address | Compare regression across subgroups |

---

2.
| Plot No. | Plot Type | What It Shows |
|---|---|---|
| 1 | **Pie Charts** | Percentage breakdown of 6 categories (gender, address, internet etc.) |
| 2 | **Stacked Bar** | Grade categories (Fail/Average/Good/Excellent) by gender & study time |
| 3 | **Bubble Chart** | Study time vs grade where bubble size = number of absences |
| 4 | **Full Dashboard** | 8 different charts combined into one big overview image |
|---|---|---|---|
| 1 | Plotly | Interactive Scatter | Hover over points to see student details |
| 2 | Plotly | Interactive Box | Compare grade distributions interactively |
| 3 | Plotly | 3D Scatter | G1, G2, G3 in 3D space — rotate and explore |
| 4 | Plotly | Sunburst Chart | Drill down: Gender → Address → Internet |
| 5 | Missingno | Missing Value Chart | Check if any data is missing |
| 6 | WordCloud | Word Frequency Cloud | Visual map of most common jobs/reasons |

---

3.
| Plot No. | What It Shows |
|---|---|
| 1 | **Model Comparison** — bar chart comparing accuracy of all 7 models |
| 2 | **Confusion Matrix + ROC Curves** — how well each model predicts pass/fail |
| 3 | **Feature Importance** — which features matter most for prediction |
| 4 | **Decision Tree** — visual tree showing exactly how the model makes decisions |

---

## 📐 Statistical Tests Explained

| Test | What It Does | What We Found |
|---|---|---|
| **T-test** | Checks if male and female grades are significantly different | Is the difference real or just random? |
| **ANOVA** | Checks if different study time groups have different grades | Does studying more really improve grades? |
| **Chi-Square** | Checks if internet access affects pass/fail result | Does having internet help students pass? |
| **Pearson Correlation** | Measures strength of relationship between study time and grade | How strongly are they connected? |

---

## 🔑 Key Findings from This Project

| Finding | Insight |
|---|---|
| ✅ G1 and G2 strongly predict G3 | First and second period grades are best predictors |
| ✅ More study time → higher grades | Students who study more score better |
| ✅ Past failures → lower final grades | Students with failures tend to get lower G3 |
| ✅ High absences → lower grades | Missing school negatively impacts performance |
| ✅ Urban students perform slightly better | Address (urban/rural) has small effect |
| ✅ Students wanting higher education score better | Motivation matters |
| ✅ High alcohol consumption → lower grades | Dalc and Walc negatively correlate with G3 |

---

## 📁 Output Files Generated

---

## 📞 About This Project

- **Dataset** : UCI Machine Learning Repository — Student Performance Dataset
- **Language** : Python 3.x
- **Platform** : Google Colab

**About te Author:**
Name : Raksihitha V
📌 GitHub  : [https://github.com/rakshitha0112/student-performance-analysis](https://github.com/rakshitha01-a11y/Student-Performance-Analysis/tree/main)
