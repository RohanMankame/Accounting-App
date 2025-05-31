# Accounting Capstone

This repository contains the CMPSC Capstone Project, an internal financing application designed to help companies efficiently manage their finances.

## Problem Statement

In the real world, documentation and economics are crucial for companies. This project connects computer science to these concepts through the development of internal financing software. Compared to traditional paper-based methods, software offers enhanced security, speed, and accessibility.

Our application aims to provide a comprehensive solution for managing budgets, expenses, income, payables/receivables, cash flow, taxes, audits, and other document handling matters, such as Profit/Loss statements. The system utilizes an external database to store confidential information, including user credentials, user data, and financial documents like PDF statements.

## Features

The application includes a wide range of features to streamline financial management:

### **Core Functionalities**
* **User Authentication:** Secure user login with username and password, authenticated against a dedicated database.
* **Modular Dashboard:** The main homepage features summary graphs for key financial aspects, including:
    * Profit Calculation vs. Cost Calculation
    * Monthly Revenue, with comparisons to previous months
    * Projected Cashflow Expenses
    * Sales Summaries and Projections
* **CRUD Operations:** Each module supports Create, Read, Update, and Delete functionalities.

### **Financial Management Modules**
* **Budget Management:** Create, modify, and track budgets, with reports categorized by fiscal quarter.
* **Expense and Income Tracking:** View and manage expected expenses and income in a tabular format.
* **Cash Flow Management:** A backend module that provides a real-time overview of a business's cash flow, displayed on the dashboard.
* **Invoicing:** Manage receivable and payable invoices, with support for standard, retainer, and recurring types.
* **Treasury:** Add, manage, and track bank accounts and credit cards, with detailed transaction histories.
* **Payroll:** A comprehensive employee management system that handles payroll details, payment status, and historical payment data.

## Tech Stack

* **Frontend:** JavaFX
* **Backend:** Java, Python
* **Data Visualization:** Seaborn, Matplotlib
* **Database:** Azure SQL Database
* **Build Tool:** Maven

## Database Schema

The application's database is structured into several key tables:

* **userLoginInformation:** Stores user authentication details.
* **userInformation:** Contains user profile information.
* **userDocuments:** Manages user-uploaded financial documents.
* **financialData:** Stores data parsed from the financial documents.
* **Invoice Tables:** Separate tables for managing receivable and payable invoices.
* **Treasury Tables:** Tables for bank accounts, credit cards, and their associated transactions.
* **Payroll Tables:** Tables for employee information, payment status, and payment history.

## Setup and Installation

To run the application and generate graphs, please follow these steps:

1.  **Install Python:** Make sure you have the latest version of Python installed.
2.  **Install Dependencies:** Run the following command to install the required Python packages:
    ```bash
    pip install seaborn matplotlib pandas pypyodbc
    ```
3.  **Install ODBC Driver:** Download and install the [ODBC Driver 18 for SQL Server](https://learn.microsoft.com/en-us/sql/connect/odbc/download-odbc-driver-for-sql-server?view=sql-server-ver16).
4.  **Verify Driver Installation:**
    * Open "ODBC Data Sources" from the Windows search bar.
    * Navigate to the "Drivers" tab and verify that "ODBC Driver 18 for SQL Server" is listed.
5.  **Configure Database Connection:** The database connection details are located in the `application.properties` file.

## Contributors

* Danny Le
* Aman Sahu
* Andrew Miller
* Rohan Mankame

**Advisor:** Kabir

**Orignal Link:** https://github.com/Adraxone/AccountingCapstone

