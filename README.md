# Titanic Dataset Analysis and Dashboard Assessment

## Overview
This project analyzes the Titanic dataset using **SQL in Google BigQuery** and visualizes key insights through a **dashboard**. The analysis explores survival rates based on different factors such as **passenger class, gender, fare, age, and embarkation port**. The dashboard provides a visual representation of the findings to enhance data-driven storytelling.

## Dataset
The dataset used in this project is the **Titanic Dataset (train.csv) from Kaggle**. It contains essential details about the passengers, including their **survival status, age, gender, class, and fare**.
[Dataset Link](https://www.kaggle.com/competitions/titanic)

### Key Fields:
- `PassengerId`: Unique identifier for each passenger.
- `Survived`: 0 = Did not survive, 1 = Survived.
- `Pclass`: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd).
- `Name`: Passenger's name.
- `Sex`: Gender of the passenger.
- `Age`: Age of the passenger.
- `SibSp`: Number of siblings and spouses aboard.
- `Parch`: Number of parents and children aboard.
- `Ticket`: Ticket number.
- `Fare`: Fare paid for the ticket.
- `Cabin`: Cabin number (if available).
- `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

---

## Project Workflow
### 1. Data Preparation
- **Import Data into BigQuery**: Upload **train.csv** into a BigQuery project.
- **Data Cleaning**:
  - Handle missing values in `Age`, `Fare`, and `Embarked` columns.
  - Ensure correct data types (e.g., `Pclass` and `Survived` as integers, `Fare` and `Age` as numeric values).

### 2. Data Analysis (SQL Queries in BigQuery)
The following questions were answered using SQL queries:

1. **Overall Survival Rate**: What percentage of passengers survived?
2. **Survival by Passenger Class**: What is the survival rate for each class (1st, 2nd, 3rd)?
3. **Survival by Gender**: How does gender impact survival rates?
4. **Fare vs. Survival**: What is the average fare paid by survivors vs. non-survivors?
5. **Age vs. Survival**: What is the average age of survivors and non-survivors?
6. **Survival by Embarkation Port**: How does the port of embarkation affect survival rates?
7. **Family Size vs. Survival**: How does family size (sum of `SibSp` and `Parch`) influence survival chances?
8. **Top 10 Survivors by Fare Paid**: Who were the top 10 passengers who paid the highest fare and survived?

## Technologies Used
- **Google BigQuery**: SQL-based data analysis.
- **Data Visualization**: Google Data Studio.

[Dashboard Link](https://lookerstudio.google.com/reporting/a5ca317c-23c9-45af-a8e2-2ceb80aaaab2)


## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/titanic-analysis.git
   ```
2. Import `train.csv` into **Google BigQuery**.
3. Run SQL queries to analyze survival trends.
4. Use visualization tools to create the dashboard.

## Insights & Conclusion
This analysis provides valuable insights into the factors influencing Titanic passengers' survival. The dashboard effectively visualizes key trends, making data interpretation easier.

