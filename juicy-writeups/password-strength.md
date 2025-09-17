# Password Strength Writeup

## Challenge Description
Log in with the original user credentials without SQL injection or similar techniques.

## Solution
1. I tried to guess weak passwords for known users.
2. I used `admin@juice-sh.op` as the email.
3. I tried common passwords like "admin123", "password", "123456".
4. The password "admin123" worked!

## Steps
- Go to the login page.
- Email: `admin@juice-sh.op`
- Password: `admin123`
- Click Login.

## Screenshot
*(Insert screenshot here if required)*

## Reflection
This challenge showed me how dangerous weak passwords are. Admins should never use simple passwords like "admin123". It was way too easy to guess.

## OWASP Top 10 Category
**A07:2021 - Identification and Authentication Failures**
This challenge demonstrates the risks of weak password policies and easily guessable credentials.