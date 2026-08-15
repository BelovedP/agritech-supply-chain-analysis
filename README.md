# Agritech Supply Chain & Yield Analysis
## Project Overview
This repository contains a processed and engineered agricultural dataset evaluating 200 farmer records. The goal of this project was to transform raw farm records, engineer operational feature column, and extract core business metrics to optimize supply chain timelines and financial risk assessments.

# Business value and Operational Impact
By transforming this raw agricultural raw data, this project unlocks three critical business capacities:
1. **Risk Management:** Instantly flags delayed harvest to protect downstream supply chain timelines.
2. **Financial Underwriting:** Standardizes credit scoring criteria to automate loan approvals for eligible cooperative farmers.
3. **Data Integrity:** Cleans messy input text to prevent duplicate records and downstream data warehouse reporting errors.

## Processed Data Preview
![Processed Data Dashboard](dashboard.png)

## Repository Structure
* 'agritech_farm_data.xlxs':  The primary processed excel workbook containing engineered feature columns.
* 'README.md' :Project documentation, business logic and execcutive insights.
---
## Data Engineering & Feature Columns
The followings were programmatically engineered using Excel formulars to enhance the raw dataset:

* **Farm Size Classification ("Column N"):** Categorized landholdings into *Smallholder* , *Medium-Scale* , or *Commercial* using nested statements.
*  **Harvest Schedule Flag ("Column O"):** Evaluated operational timelines against target dates to flag distribution delays.
*  **Loan Eligibility Status ("Column P"):** Combined conditional evaluations("AND") checking for strong repayment history and sustainable land sizes($\geg$ 2 hectares).
*  **Days to Harvest ("Column Q"):** Subtracted planting timelines from harvest dates to isolate crop growth durations.
*  **Metadata Extraction ("Column R & S"):** Used text manipulation ("LEFT" and "MID") to cleanly isolate region and crop codes embedded within FarmerIDs.
*  **Data Hygiene Scrubber ("Column T"):** Utilized text trimming functions to permanently eliminate irregular and messy whitespaces.
