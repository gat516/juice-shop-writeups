# CSRF Writeup

## Challenge Description
Change Bender's password through a Cross-Site Request Forgery attack.

## Solution
1. I logged in as Bender first to understand the password change process.
2. I found the password change endpoint and analyzed the request.
3. I noticed there was no CSRF token protection.
4. I created a malicious HTML page with a form that submits to the password change endpoint.
5. When someone visits my page while logged in as Bender, their password gets changed.

## Steps
- Log in as Bender and go to password change page
- Analyze the form submission using Developer Tools
- Create an HTML page with a hidden form that auto-submits
- Host the page and trick Bender into visiting it

## Reflection
CSRF attacks are sneaky! They trick users into performing actions they didn't intend to do. This is why websites should use CSRF tokens to verify that requests are legitimate and not coming from malicious sites.

## OWASP Top 10 Category
**A01:2021 - Broken Access Control**
This challenge demonstrates Cross-Site Request Forgery (CSRF), where malicious websites can perform unauthorized actions on behalf of authenticated users.