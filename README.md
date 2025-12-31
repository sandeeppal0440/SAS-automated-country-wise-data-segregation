# SAS-automated-country-wise-data-segregation


Project Overview
This project demonstrates an end-to-end SAS macro automation solution designed to process Uber operational data and generate country-wise datasets and reports automatically.The program imports raw Excel data, dynamically creates datasets for each country, and exports them as CSV files with time-based naming conventions.
The solution is built using SAS Macros, PROC SQL, DATA steps, and system functions, making it scalable, reusable, and suitable for production-level analytics pipelines.


Project Objective
The primary objectives of this project are:
•Automate country-level data segregation from a single source file
•Eliminate manual intervention in monthly reporting
•Generate dynamic dataset names using the previous month (Year-Month logic)
•Create clean, standardized output files for downstream analytics or dashboards
•Capture logs for audit and debugging purposes


Key Features & Functionality 
•Macro-driven automation for scalability
•Dynamic log redirection using PROC PRINTTO
•Excel to SAS import using PROC IMPORT
•Date-driven reporting with INTNX() and macro variables 
•Dynamic macro variable creation using CALL SYMPUTX
•Country-wise looping using %DO %TO
•Automated CSV exports using PROC EXPORT
•Data-safe naming conventions using COMPRESS()


Key Insights from the Program
Scalable Design
 •The macro dynamically adapts to any number of countries using PROC SQL and &SQLOBS.
 •No hardcoding required for country values.
 
Production-Ready Automation
•Monthly execution is automated using system date functions.
•Output files are clearly labeled with Year-Month and Country.

Data Governance & Debugging
•Logs are redirected to external files for traceability and audits.
•%PUT statements help track macro variable values during execution.

Clean & Standardized Outputs
•Country names are cleaned using COMPRESS() to avoid invalid dataset names.
•Each country receives a separate, analytics-ready CSV file.

Real-World Business Use Case
•Ideal for Uber-like operations, risk analytics, regional reporting, and MIS automation.
•Can easily integrate with BI tools (Power BI / Tableau) or downstream SQL processes.

Skills Demonstrated
•SAS Base Programming
•SAS Macros (Parameterized, DO-Loop Macros)
•PROC SQL
•Data Automation & Reporting
•Log Management
•Real-world Analytics Workflow Design
