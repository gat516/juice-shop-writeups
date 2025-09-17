# Reflected XSS Writeup

## Challenge Description
Perform a reflected XSS attack.

## Solution
1. I found that the order tracking page reflects user input.
2. I went to `/#/track-result` and entered a malicious script in the tracking ID field.
3. I used `<iframe src="javascript:alert('XSS')">` as the tracking ID.
4. The script executed when the page loaded, showing an alert.

## Steps
- Go to the order tracking page at `/#/track-result`
- Enter: `<iframe src="javascript:alert('XSS')">`
- The XSS payload executes immediately

## Reflection
Reflected XSS is different from DOM XSS because the malicious script comes from the server response. It's still dangerous because it can steal cookies or redirect users to malicious sites.

## OWASP Top 10 Category
**A03:2021 - Injection**
This challenge demonstrates reflected Cross-Site Scripting where user input is reflected back in the HTTP response without proper sanitization.