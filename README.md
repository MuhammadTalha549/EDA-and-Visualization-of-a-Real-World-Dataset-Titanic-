# EDA-and-Visualization-of-a-Real-World-Dataset-Titanic-

# Titanic Dataset EDA & Visualization

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Used-orange.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-Used-blueviolet.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Used-yellowgreen.svg)
![Status](https://img.shields.io/badge/Status-Complete-success.svg)

## 📋 Project Overview

This project explores the Titanic dataset using Exploratory Data Analysis (EDA) techniques to extract meaningful insights. The dataset is loaded using the `seaborn` library and analyzed using Python tools such as `pandas`, `matplotlib`, and `seaborn`. The project involves data cleaning, handling missing values, removing outliers, and generating visualizations to better understand patterns in survival rates and passenger demographics.

## 🎯 Objectives

* Load and inspect the Titanic dataset.
* Clean and preprocess the data (handle missing values, outliers, duplicates).
* Perform EDA using bar charts, histograms, and correlation heatmaps.
* Draw insights from visual patterns in the data.
* Prepare the dataset for potential further analysis or modeling.

## 🧠 Key Questions Addressed

* What factors influenced passenger survival?
* How does age, sex, class, and fare impact survival chances?
* Are there any outliers or missing values that need handling?
* Which features are most correlated?

## 📊 Dataset

The dataset is loaded from `seaborn`'s built-in Titanic dataset:

* **Samples**: 891 passengers
* **Target Variable**: `survived` (0 = No, 1 = Yes)
* **Features**: `pclass`, `sex`, `age`, `fare`, `embarked`, `class`, `who`, `alone`, and others

## 🧼 Data Preprocessing

### ✔️ Cleaning Steps:

1. **Missing Values**:

   * `age` filled with median
   * `embarked` filled with mode
   * `deck` column dropped due to many missing values
   * Remaining null rows dropped

2. **Duplicates**:

   * Checked and removed (none found)

3. **Outliers**:

   * `fare` column cleaned using IQR method with 2.5 multiplier

### Result:

* **Cleaned Dataset Shape**: `(889, 14)`

## 📈 Visualizations & Analysis

### 1. **Bar Charts for Categorical Variables**

* Countplots for `sex`, `class`, `embarked`, `who`, and `survived`
* Help understand population distribution and survival patterns

### 2. **Histograms for Numerical Features**

* Histograms of `age` and `fare` to understand data spread

### 3. **Correlation Heatmap**

* Shows relationships between numeric columns (e.g., `fare`, `pclass`, `age`, `survived`)

## 💡 Summary of Insights

| Feature             | Insight                                                                              |
| ------------------- | ------------------------------------------------------------------------------------ |
| **Survival Rate**   | More **females** and **1st class** passengers survived.                              |
| **Passenger Class** | Higher class correlated with higher survival.                                        |
| **Age**             | Majority of passengers were **20-40 years old**.                                     |
| **Fare**            | Most fares were low; high-fare outliers removed.                                     |
| **Embarkation**     | Most passengers boarded from **Southampton (S)**.                                    |
| **Correlation**     | `fare` positively correlates with `pclass`, and `pclass` negatively with `survived`. |

## 🛠️ Installation & Setup

### Prerequisites

```bash
Python 3.8+
Jupyter Notebook or any Python IDE
```

### Required Libraries

Install using pip:

```bash
pip install pandas numpy seaborn matplotlib
```

### Clone Repository

```bash
git clone https://github.com/yourusername/titanic-eda-visualization.git
cd titanic-eda-visualization
```

## 📁 Project Structure

```
titanic-eda-visualization/
├── README.md                     # Project documentation
├── titanic_eda_visualization.ipynb  # Main notebook
└── requirements.txt              # Python package dependencies
```

## 🏃‍♂️ How to Run

### Option 1: Jupyter Notebook

```bash
jupyter notebook
```

Then open `titanic_eda_visualization.ipynb` and run all cells.

### Option 2: Python IDE

Open the notebook in VS Code or any IDE with Jupyter support.

## 🔍 Technical Details

* Data loaded using `seaborn.load_dataset("titanic")`
* Cleaning handled using `pandas` methods (`fillna`, `drop`, `duplicated`)
* Outlier handling via **Interquartile Range (IQR)**
* Visualizations created using **Seaborn** and **Matplotlib**

## 🚧 Limitations & Future Work

### Current Limitations

* Basic EDA only; no predictive modeling
* `deck` column dropped instead of imputed
* Simplified outlier removal

### Future Enhancements

* Perform classification modeling (Logistic Regression, Random Forest, etc.)
* Explore feature engineering (title extraction from names, family size)
* Build a dashboard using Streamlit or Dash

## 🤝 Contributing

Contributions are welcome! You can help by:

* Improving data visualizations
* Adding predictive modeling
* Enhancing preprocessing steps


**Your Name**

* GitHub: [@https://github.com/MuhammadTalha549](https://github.com/MuhammadTalha549)
* Email: [talhamuhammad549@gmail.com](talhamuhammad549@gmail.com)

---

⭐ **If you found this project helpful, please give it a star!** ⭐
