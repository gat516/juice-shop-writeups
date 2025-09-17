# Forged Feedback Writeup

## Challenge Description
Post some feedback in another users name.

## Solution
1. I logged in with my own account and went to the feedback page.
2. I submitted feedback and analyzed the request using Developer Tools.
3. I found that the user ID is sent in the request body or headers.
4. I intercepted the request and changed the user ID to another user's ID.
5. The feedback was posted under the other user's name.

## Steps
- Log in and go to feedback page
- Fill out feedback form but don't submit yet
- Open Developer Tools and go to Network tab
- Submit feedback and capture the request
- Resend the request with a different user ID

## Reflection
This shows another access control issue. The application should verify that you can only post feedback as yourself, not as other users. It's like identity theft but for feedback forms!

## OWASP Top 10 Category
**A01:2021 - Broken Access Control**
This challenge demonstrates insufficient verification of user identity, allowing users to perform actions on behalf of others.