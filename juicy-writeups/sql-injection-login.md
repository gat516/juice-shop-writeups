# SQL Injection Login Writeup

## Challenge Description
Log in without providing valid credentials using SQL injection.

## Solution
1. I went to the login page.
2. In the email field, I entered: `admin@juice-sh.op'--`
3. I put any password (like "password").
4. The SQL injection bypassed the password check and logged me in as admin.

## Steps
- Go to the login page.
- Email: `admin@juice-sh.op'--`
- Password: `anything`
- Click Login.
- You should be logged in as admin.

## Screenshot
*(Insert screenshot here if required)*

## Reflection
This was really cool! The `'--` comment syntax in SQL made the database ignore the password check. I need to learn more about how SQL works to understand this better.

## OWASP Top 10 Category
**A03:2021 - Injection**
This challenge demonstrates SQL injection, where malicious SQL code is inserted into application queries to manipulate database operations.