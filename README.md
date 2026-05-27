# Customer Churn Analysis

## Project Overview
This repository contains a customer churn analysis project built with Power BI. It includes a dataset of customer account details, a report file, and the underlying report definition and semantic model used by Power BI.

## Repository Contents
- `Customer Data.csv` — the customer dataset used by the report
- `Churn Analysis for customer data.pbip` — the packaged Power BI report file
- `Churn Analysis for customer data.Report/` — extracted report definition files for the Power BI report
- `Churn Analysis for customer data.SemanticModel/` — the semantic model containing tables and relationships used by the report

## Dataset Summary
The primary dataset is `Customer Data.csv`, and it contains the following fields:
- `customer_id`
- `credit_score`
- `country`
- `gender`
- `age`
- `tenure`
- `balance`
- `products_number`
- `credit_card`
- `active_member`
- `estimated_salary`
- `churn`

The dataset tracks customer demographics, account information, membership status, and whether each customer churned.

## Report Structure
The Power BI report is built from the `Customer Data` table and includes supporting tables for segmentation such as:
- Age groups
- Account balance groups
- Credit score groups

The report files under `Churn Analysis for customer data.Report/definition/` include:
- `report.json` — main report configuration
- `pages.json` — page metadata
- `version.json` — schema version
- `diagramLayout.json` — visual layout
- Visual configuration files under `pages/.../visuals/`

The semantic model files under `Churn Analysis for customer data.SemanticModel/definition/` include the model definition and table metadata used by Power BI.

## How to Open the Report
1. Open `Churn Analysis for customer data.pbip` in Power BI Desktop.
2. If using the extracted report files, open the report definition from the relevant Power BI project folder.
3. Make sure the `Customer Data.csv` file is available as the data source if the report uses a file-based connection.

## Key Analysis Goals
The report is designed to help answer questions such as:
- Which customer segments are most likely to churn?
- How do churn rates vary by age, balance, and credit score?
- What demographic or product attributes are related to customer retention?

## Notes
- The dataset is based on bank customer profile and churn status data.
- The report can be updated by editing the `report.json` and semantic model definitions.

## License
This repository contains sample analysis files and dataset contents for customer churn exploration.
