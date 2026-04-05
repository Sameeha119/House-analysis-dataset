 # 🏠 King County House Price Analysis

## 📊 Project Overview

This project explores the **King County housing dataset** to understand the factors that influence house prices. The analysis was performed using **Python in a Jupyter Notebook environment**, focusing on **data cleaning, exploratory data analysis (EDA), and statistical insights**.

The goal of the project is to prepare the dataset for analysis and investigate how features such as **bedrooms, bathrooms, house size, and location** affect property prices.

---

## 📁 Dataset

The dataset contains housing data from **King County, USA**, including information about house sales.

### Dataset Characteristics

* **21,597 rows**
* **21 columns**

### Key Variables

Some important features in the dataset include:

* **price** – Sale price of the house
* **bedrooms** – Number of bedrooms
* **bathrooms** – Number of bathrooms
* **sqft_living** – Living area in square feet
* **sqft_lot** – Lot size
* **floors** – Number of floors
* **waterfront** – Whether the property has a waterfront view
* **view** – Quality of the house view
* **grade** – Overall construction and design grade
* **yr_built** – Year the house was built
* **yr_renovated** – Year the house was renovated
* **zipcode** – Location of the property

---

## 🧹 Data Cleaning

Several preprocessing steps were performed to ensure the dataset was suitable for analysis.

### Handling Missing Values

Some columns contained missing values:

| Column       | Missing Values |
| ------------ | -------------- |
| waterfront   | 2,376          |
| view         | 63             |
| yr_renovated | 3,842          |

These missing values were handled using the following methods:

* `waterfront` → filled with **0** (no waterfront)
* `yr_renovated` → filled with **0** (not renovated)
* `view` → filled with the **mode value**

---

## 🔎 Exploratory Data Analysis (EDA)

The analysis used several **Pandas functions** to understand the dataset:

### Key Pandas Methods Used

* `df.head()` – preview the dataset
* `df.shape` – check dataset size
* `df.describe()` – statistical summary of numerical columns
* `df.describe(include="all")` – summary of all columns
* `df.dtypes` – inspect column data types
* `df.isnull().sum()` – detect missing values
* `value_counts()` – count unique values
* `corr()` – calculate correlation between variables

---

## 📈 Example Analysis Questions

The notebook explores questions such as:

* How many houses exist for each **floor category**?
* Is there a **correlation between bedrooms and house price**?
* Are there **price trends based on the year the house was built**?

Example correlation result:

Correlation between **bedrooms and price**:

```
0.30879
```

This indicates a **moderate positive relationship**, meaning houses with more bedrooms tend to have higher prices.

---

## 🛠 Tools and Libraries

The analysis was conducted using the following tools:

* **Python**
* **Jupyter Notebook**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**

---

## 📌 Key Insights

Some initial insights from the dataset include:

* Houses with **larger living areas** tend to have higher prices.
* **Construction grade** strongly influences property value.
* **Waterfront properties** are typically more expensive.
* Newer houses or renovated homes often have **higher median prices**.

---

## 📂 Project Structure

```
House-Price-Analysis
│
├── data
│   └── kingcounty_house_data.csv
│
├── notebooks
│   └── house_price_EDA.ipynb
│
└── README.md
```

---

## 📚 Future Improvements

Possible extensions for this project include:

* Building **predictive models** for house prices
* Creating **interactive dashboards**
* Performing deeper **feature engineering**
* Applying **machine learning algorithms**

---

## 👩‍💻 Author

[Simiat Ahmed](https://www.linkedin.com/in/simiat-ahmed-bbbb58146?utm_source=share_via&utm_content=profile&utm_medium=member_android)

Data Analysis Project using Python and Jupyter Notebook.
