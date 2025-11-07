Here’s a well-structured README file content for the workflow shown in the screenshot:


---

🧾 Zomato Data Analysis Workflow

📘 Overview

This project represents a Sales Data Analysis Workflow built to explore, prepare, model, and analyze sales data.
The workflow uses a combination of data preprocessing, partitioning, and CHAID (Chi-squared Automatic Interaction Detector) modeling to predict sales categories and generate analytical outputs for decision-making.


---

📂 Workflow Components

1. Data Input

Node: zomato_data.csv

Description:
The workflow starts by importing the sales_data.csv file, which contains the raw sales information.
The dataset is connected to:

Fields: To inspect metadata such as variable names and data types.

Table: To preview raw data and ensure correct loading.




---

2. Data Preparation

This stage ensures the dataset is clean, structured, and ready for analysis.

Node	Function

Sorted Data	Sorts the dataset for consistent data order and indexing.
Type	Defines or corrects data types for each variable (numeric, categorical, string).
Filler	Handles missing or null values (imputation or removal).
SALES_CATEGORY	Creates a derived categorical variable (e.g., Low, Medium, High) based on sales values.



---

3. Data Partitioning

Node: Partition

Purpose:
Splits the dataset into training and testing subsets.
This ensures that model evaluation is unbiased and performance metrics reflect real-world predictive ability.



---

4. Modeling: CHAID Algorithm

Node: CHAID

Description:
The CHAID algorithm builds a decision tree model to predict SALES_CATEGORY.

Purpose:
Identify the key predictors influencing sales categories.

Steps:

The first CHAID node creates the initial model.

The second CHAID node refines or validates the first model for improved accuracy.




---
5. Analysis

Node: Analysis

Purpose:
Evaluates the CHAID model output by examining:

Tree structure and splits

Predictor importance

Statistical metrics (p-values, chi-squared statistics)




---

6. Post-Processing

Node	Function

Filter	Removes unnecessary records or isolates relevant subsets for analysis.
Aggregate	Summarizes model results (e.g., counts, averages, totals) by group or category.



---

7. Output Tables

Multiple Table nodes are connected throughout the workflow.

Each represents an intermediate or final result:

Raw data previews

Sorted or filtered datasets

Aggregated model summaries




---

🧠 Workflow Summary

This workflow demonstrates a complete data mining pipeline:

1. Importing sales data


2. Preparing and cleaning datasets


3. Creating a target variable (SALES_CATEGORY)


4. Partitioning data for training/testing


5. Building CHAID models for prediction


6. Analyzing results with performance metrics


7. Generating outputs for reporting and decision support




---

📊 Outcome

Identifies key drivers behind sales performance.

Classifies sales into meaningful categories.

Produces structured tables for business analysis.

Provides an interpretable, rule-based decision tree output.



---

🧩 Technologies / Tools

Data Mining & Modeling Environment (e.g., IBM SPSS Modeler or similar)

CHAID Algorithm for classification

CSV dataset as input
