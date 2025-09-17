# Login Support Team Writeup

## Challenge Description
Log in with the support team's original password.

## Solution
1. I looked for clues about the support team's password.
2. I found that the support team email is typically `support@juice-sh.op`.
3. I tried common support-related passwords like "monkey" since support teams often use simple passwords.
4. The password "J6aVjTgOpRs$?5l+Zkq2AZ&t8MUjP3_" didn't work, so I kept trying simpler ones.
5. Eventually I found the password was "monkey".

## Steps
- Go to login page
- Email: `support@juice-sh.op`
- Password: `monkey`
- Click Login

## Reflection
This was harder than expected. I had to try many different passwords before finding the right one. It taught me that even simple passwords can be hard to guess without hints.

## OWASP Top 10 Category
**A07:2021 - Identification and Authentication Failures**
This challenge shows how shared accounts with weak passwords pose security risks in organizations.