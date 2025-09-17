# Upload Type Writeup

## Challenge Description
Upload a file with a forbidden extension.

## Solution
1. I found the file upload feature and tested what file types are allowed.
2. I noticed it only accepts certain extensions like .jpg, .png, etc.
3. I tried uploading a .php or .exe file but it was blocked.
4. I used techniques like double extensions (.jpg.php) or modified the MIME type.
5. I successfully uploaded a file with a forbidden extension.

## Steps
- Find the file upload feature
- Try uploading files with various extensions
- Use techniques like double extensions or MIME type manipulation
- Successfully upload a forbidden file type

## Reflection
This challenge taught me about file upload security. Applications should check file types properly on the server side, not just by looking at the file extension. Attackers can easily fake file extensions to upload malicious files.

## OWASP Top 10 Category
**A04:2021 - Insecure Design**
This challenge demonstrates insufficient file type validation that could allow malicious file uploads, potentially leading to remote code execution.