# Exposed Metrics Writeup

## Challenge Description
Find the endpoint that serves usage data to be scraped by a popular monitoring system.

## Solution
1. I looked for common monitoring endpoints used by systems like Prometheus.
2. I tried accessing `/metrics` endpoint which is standard for Prometheus monitoring.
3. The endpoint was accessible and showed internal application metrics.
4. This revealed sensitive information about the application's performance and usage.

## Steps
- Try accessing `/metrics` in your browser
- Look for other common monitoring endpoints like `/health`, `/status`
- Observe the sensitive data exposed

## Reflection
This was a good lesson about monitoring systems. While metrics are useful for system administrators, they shouldn't be publicly accessible because they can reveal sensitive information about how the application works and performs.

## OWASP Top 10 Category
**A05:2021 - Security Misconfiguration**
This challenge demonstrates how improperly secured monitoring endpoints can expose sensitive operational data to unauthorized users.