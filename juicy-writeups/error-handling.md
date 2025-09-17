# Error Handling Writeup

## Challenge Description
Provoke an error that is neither very gracefully nor consistently handled.

## Solution
1. I tried to cause various errors in the application.
2. I submitted invalid data in forms, tried broken URLs, and invalid API calls.
3. I found that certain error conditions reveal sensitive information.
4. I triggered an error that showed stack traces or internal server details.
5. This revealed information about the server technology and file paths.

## Steps
- Try submitting invalid data in forms
- Access non-existent pages or API endpoints
- Send malformed requests to the server
- Look for error messages that reveal too much information

## Reflection
This challenge taught me that error messages can leak sensitive information about a system. Good applications should show user-friendly error messages without revealing internal details that attackers could use.

## OWASP Top 10 Category
**A05:2021 - Security Misconfiguration**
This challenge demonstrates poor error handling that can lead to information disclosure, revealing sensitive system details to attackers.