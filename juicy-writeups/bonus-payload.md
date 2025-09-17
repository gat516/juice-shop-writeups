# Bonus Payload Writeup

## Challenge Description
Use a deprecated B2B interface that was not properly shut down.

## Solution
1. I looked for old or deprecated API endpoints in the application.
2. I found references to B2B (Business-to-Business) functionality.
3. I discovered the old endpoint was still accessible at `/b2b/v2/orders`.
4. I was able to access the deprecated interface and place B2B orders.
5. This showed that old interfaces weren't properly decommissioned.

## Steps
- Look for API documentation or old endpoint references
- Try accessing `/b2b/v2/orders` or similar B2B endpoints
- Test the deprecated functionality
- Successfully use the old interface

## Reflection
This challenge taught me about the importance of proper decommissioning. When companies update their systems, they should make sure old versions are completely removed, not just hidden. Leaving old interfaces running creates security risks.

## OWASP Top 10 Category
**A05:2021 - Security Misconfiguration**
This challenge demonstrates how improperly decommissioned legacy systems can create unintended access points and security vulnerabilities.