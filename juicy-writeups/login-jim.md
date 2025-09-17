# Login Jim Writeup

## Challenge Description
Log in with Jim's Gmail account without previously changing his password, applying SQL Injection, or hacking his Google account.

## Solution
1. I found Jim's email address in the customer reviews or user list.
2. I researched information about Jim's character or background.
3. I tried passwords related to Star Trek since Jim often references it.
4. I found that Jim's password is "ncc-1701" (USS Enterprise's registry number).

## Steps
- Find Jim's Gmail address (usually in reviews)
- Email: `jim@gmail.com` or similar
- Password: `ncc-1701`
- Click Login

## Reflection
This challenge required knowing some Star Trek trivia! Jim clearly loves Star Trek and used a reference from the show as his password. It shows how personal interests can make passwords predictable. Nerdy passwords aren't necessarily secure passwords.

## OWASP Top 10 Category
**A07:2021 - Identification and Authentication Failures**
This challenge demonstrates how passwords based on personal interests or pop culture references can be easily guessed by attackers who research their targets.