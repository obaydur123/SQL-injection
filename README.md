# Automated SQL Injection & Database Reconnaissance using SQLMAP

## 📌 Project Overview
The objective of this project was to identify SQL Injection vulnerabilities on a target login page and perform advanced database reconnaissance. It includes simulating a standard SQLi attack and performing Blind SQL injection to retrieve backend database information without direct visual feedback.

## 🛠️ Tools Used
* **Automated Scanner:** SQLMAP
* **Environment:** Kali Linux / Pentesting Lab

## ⚡ Methodology & Key Steps
1. **Target Scanning:** Used SQLMAP to automatically detect parameter vulnerability on the target login form
2. **DBMS Fingerprinting:** Identified the underlying Database Management System (DBMS) and version.
3. **Blind SQL Injection:** Configured SQLMAP payloads to extract database schemas, table names, and columns through time-based/boolean-based blind techniques
4. **Data Dumping:** Successfully extracted sample dummy user credentials in a safe sandbox environment.

## 🛡️ Mitigation Strategies
* **Use WAF (Web Application Firewall):** Deploy a WAF to detect and block automated SQLMAP scanning signatures.
* **Stored Procedures:** Use parameterized stored procedures for database interactions.
* **Disable Detailed Errors:** Prevent the database from displaying raw SQL error messages to the end-user.
