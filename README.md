# Take-Home Assessment for Quant Dev Intern - Metals Desk

## Introduction

This take-home assessment is designed to gauge your proficiency in Python, SQL, and asynchronous programming, as these are key aspects of the Quant Dev Intern role on the Metals Desk. The assessment consists of six questions (+1 design task), each increasing in complexity.

## Requirements

- Python 3.8+
- Jupyter Notebook
- Pandas
- SQLAlchemy or any other SQL toolkit
- asyncio library for asynchronous programming

## Instructions

1. Fork this repository to your GitHub account.
2. Clone the forked repository and navigate to the directory.
3. Answer the questions listed below in the Jupyter Notebook under the `.solutions` directory.
4. Ensure that all code is clean, well-commented, and accompanied by explanations of your approach and reasoning.
5. Each question should be answered in a separate Jupyter Notebook.
4. Push the completed Notebook back to your GitHub repository.
5. Share the GitHub link with us by the deadline provided.

## Additional Notes

- You are free to use any Python libraries you wish, the requirements above are purely a suggestion.
- You may find it useful to create an SQLITE database to store the data for the SQL questions.

---

## Questions

---
### Question 1: Python Basics and Data Manipulation
**Objective:** Demonstrate basic Python skills and data manipulation using Pandas.

**Task:**
- Load a given CSV file containing metal prices into a Pandas DataFrame.
- Filter the data to include only 'Copper' and 'Zinc' for the year 2021.
- Calculate the average price per month for each metal and plot it.

---

### Question 2: CRUD Operations in SQL Server
**Objective:** Basic SQL Server interactions.

**Task:**
- Create an SQL table schema to store time-series metal prices. Include fields like `Date`, `Metal`, `Price`.
- Demonstrate basic CRUD operations

---

### Question 3: Data Pipeline and Transformation
**Objective:** Show understanding of creating data pipelines and transformations.

**Task:**
- Using the CSV file from Question 1, filter the data to include only 'Copper' and 'Zinc' for the year 2020 & 2021.
- Demonstrate the use of asynchronous programming to calculate MACD (slow/medium/fast) and RSI for each metal historically.
- Use SQL inserts to populate the SQL table created in Question 2 with this generated data.
- Demonstrate the use of a context manager to handle the connection to the database.
- Demonstrate the use of a decorator to log the execution of the asynchronous SQL inserts.

---

### Question 4: FastAPI and Modularity
**Objective:** Demonstrate understanding of FastAPI and modular code.

**Task:**
- Write a simple FastAPI app that provides an endpoint to fetch the average price of a given metal over a specific time range from your SQL Server database.

---

### Question 5: Advanced Data Storage and Model Serialization
**Objective:** Evaluate understanding of advanced database storage mechanisms and model storage.

**Task:**
- Design a SQL schema for storing machine learning models that can be linked to different metals and their respective trading strategies.
- Serialize a simple Scikit-learn model and store it in the database (HELP: this could be storing the file name of the pickled object, with some metadata about the stored model).
- Write a CRUD function to fetch this model from the database.

---

### Question 6: Code Maintainability
**Objective:** Gauge understanding of maintainable code architecture.

**Task:**
- Take one of your previously written code blocks and refactor it to be more maintainable and modular. Explain your decisions.

---

### Technical Question: Asynchronous Technical Indicators in a Production Environment
**Objective:** Assess the understanding of complex asynchronous operations in Python, particularly in a high-throughput, real-time trading environment.

**Task:**
- You should have gained an initial insight into handling asynchronous operations from Question 3. In this question, the objective is to deepen that understanding within the context of a production environment.
- Imagine a production system that continuously monitors an extensive array of securities and calculates multiple technical indicators with varying parameters for each security.
- Describe how you would design and implement an asynchronous system in Python to efficiently generate these indicators. Consider factors like data availability, computational efficiency, and code maintainability.

---



## Submission Guidelines

1. Ensure that all code is clean, well-commented, and accompanied by explanations of your approach and reasoning.
2. Commit your Jupyter Notebook and any auxiliary files to your forked GitHub repository.
3. Submit the GitHub repository URL by the deadline.

---

Good luck!
