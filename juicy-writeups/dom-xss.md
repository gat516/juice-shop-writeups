# DOM XSS Writeup

## Challenge Description
Perform a DOM-based XSS attack using the search functionality.

## Solution
1. I went to the search box on the main page.
2. I tried entering JavaScript code like `<script>alert('XSS')</script>`.
3. The search term got reflected in the DOM without proper sanitization.
4. The alert box popped up, confirming the XSS vulnerability.

## Steps
- Go to the main page of Juice Shop.
- Click on the search box.
- Enter: `<script>alert('XSS')</script>`
- Press Enter or click search.
- The alert should pop up.

## Screenshot
*(Insert screenshot here if required)*

## Reflection
This was my first XSS attack! It was scary how easy it was to execute JavaScript in someone else's browser. I learned that user input should always be sanitized.

## OWASP Top 10 Category
**A03:2021 - Injection**
This challenge demonstrates Cross-Site Scripting (XSS), a type of injection vulnerability where malicious scripts are injected into trusted websites.