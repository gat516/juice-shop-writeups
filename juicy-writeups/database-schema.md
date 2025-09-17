# Database Schema Writeup

## Challenge Description
Exfiltrate the entire DB schema definition via SQL Injection.

## Solution
1. I found a SQL injection point in the application (like the login form).
2. I used UNION-based SQL injection to extract database schema information.
3. I crafted payloads like: `' UNION SELECT table_name,column_name FROM information_schema.columns--`
4. I systematically extracted all table and column names from the database.
5. This revealed the complete database structure.

## Steps
- Find a SQL injection vulnerability
- Use UNION SELECT to query information_schema tables
- Extract table names, column names, and data types
- Map out the complete database schema

## Reflection
This was a more advanced SQL injection challenge! Learning about information_schema was really useful. It shows how SQL injection can be used not just to bypass login, but to completely map out a database's structure. Very dangerous!

## OWASP Top 10 Category
**A03:2021 - Injection**
This challenge demonstrates advanced SQL injection techniques used for data exfiltration and reconnaissance of database structures.