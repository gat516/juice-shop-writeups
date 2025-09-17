# Outdated Whitelist Writeup

## Challenge Description
Let us redirect you to one of our crypto currency addresses which are not promoted any longer.

## Solution
1. I found redirect functionality in the application.
2. I looked for parameters like `redirect`, `url`, or `to` in the URLs.
3. I found an old cryptocurrency address in the whitelist.
4. I crafted a URL with the redirect parameter pointing to the old crypto address.
5. The application redirected me to the deprecated address.

## Steps
- Look for redirect functionality in the app
- Check for URL parameters that control redirects
- Try redirecting to old cryptocurrency addresses
- Use addresses like old Bitcoin or Ethereum addresses

## Reflection
This challenge showed me how outdated security configurations can be dangerous. Even if something is "deprecated", it might still work and create security holes. Companies need to clean up old code regularly.

## OWASP Top 10 Category
**A05:2021 - Security Misconfiguration**
This challenge demonstrates how outdated security configurations and whitelists can create unintended access paths.