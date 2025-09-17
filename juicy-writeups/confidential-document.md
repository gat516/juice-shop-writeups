# Confidential Document Writeup

## Challenge Description
Find and download a confidential document from the Juice Shop server.

## Solution
1. I looked for interesting files in the URLs and directories.
2. I found that `/ftp/` has some files.
3. I browsed to `/ftp/acquisitions.md` and downloaded it.

## Steps
- Go to `http://localhost:3000/ftp/acquisitions.md` (or your server URL).
- The file will download or show in the browser.

## Screenshot
*(Insert screenshot here if required)*

## Reflection
This challenge was easy. I just explored the `/ftp/` directory and found the file. It shows why you shouldn't leave sensitive files in public folders.

## OWASP Top 10 Category
**A05:2021 - Security Misconfiguration**
This challenge involves finding sensitive files that are exposed due to misconfigured file permissions.
