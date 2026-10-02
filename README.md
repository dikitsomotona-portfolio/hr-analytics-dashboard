# HR Analytics Dashboard

## Project Overview

This project focuses on cleaning, analysing and visualising HR data using Microsoft Power BI and Power Query.

The goal was to transform an initially inconsistent HR dataset into a cleaner and more reliable dataset and develop an interactive dashboard that provides insights into employees, salaries, performance and departmental trends.

## Tools Used

* Microsoft Power BI
* Power Query
* Microsoft Excel

## Data Quality Issues Identified

The initial HR dataset contained the following data-quality issues:

* **National ID:** Some National ID values contained only 6, 7 or 8 digits instead of the expected 9-digit format.
* **Age:** Some employee age values were missing (`null`).
* **Monthly Salary:** Some monthly salary values were missing (`null`).
* **Performance Score:** Some employee performance scores were missing (`null`).

## Data Cleaning and Transformation

The identified issues were addressed using Power Query.

### National ID Standardisation and Validation

National ID values were standardised to a **9-digit format** because Botswana Omang numbers consist of 9 digits. Values with fewer digits were padded with leading zeros where necessary.

The National ID was also checked against the employee's recorded gender. In a Botswana Omang number, the **5th digit indicates sex**:

* `1` = Male
* `2` = Female

This validation was used to identify records where the National ID and recorded gender did not correspond. The National ID was then corrected where necessary based on the recorded gender.

### Missing Values

* **Age:** Missing values were replaced using the median age of the dataset.
* **Monthly Salary:** Missing values were replaced using the median salary for the employee's department.
* **Performance Score:** Missing values were replaced using the median performance score.

Separate cleaned fields were created while retaining the original values, allowing the cleaning and validation process to be reviewed.

## Dashboard Features

The dashboard provides an overview of:

* Total number of employees
* Average employee age
* Average monthly salary
* Average performance score
* Employee distribution by department
* Gender composition
* Average salary by department
* Average performance by department
* Relationship between employee age and salary

Interactive filters allow users to explore the data by:

* Department
* Gender

## Key Skills Demonstrated

This project demonstrates practical skills in:

* Data cleaning and transformation
* Power Query
* Data quality validation
* Data analysis
* Data visualisation
* Dashboard development
* Business intelligence
* Handling missing data
* Creating meaningful analytical views from raw data

## Project Files

| [Dikitso Motona IDA Portfolio.pbix](Dikitso%20Motona%20IDA%20Portfolio.pbix) | Power BI dashboard containing the data, transformations and visualisations |

## How to Access the Dashboard

The Power BI dashboard is provided as a `.pbix` file.

To view and interact with the dashboard:

1. Download the `.pbix` file from this repository.
2. Open it using Microsoft Power BI Desktop.
3. Explore the dashboard and its interactive filters.

## Project Outcome

The project demonstrates the process of taking an initially inconsistent HR dataset, applying data-cleaning and validation techniques and transforming it into an interactive business intelligence dashboard.

