# Five Star Feedback Writeup

## Challenge Description
Get rid of all 5-star customer feedback.

## Solution
1. I logged in as admin using the previous techniques.
2. I went to the administration panel at `/#/administration`.
3. I found the customer feedback section.
4. I deleted all the 5-star reviews one by one using the delete button.

## Steps
- Log in as admin (using SQL injection or weak password)
- Navigate to `/#/administration`
- Find the "Customer Feedback" section
- Delete all feedback with 5-star ratings

## Reflection
This challenge showed me how admins can manipulate reviews and feedback. In real life, this could be used to hide negative reviews or promote fake positive ones. Pretty unethical!

## OWASP Top 10 Category
**A01:2021 - Broken Access Control**
This challenge involves using elevated privileges to manipulate data that should have proper access controls and audit trails.