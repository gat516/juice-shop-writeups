# Upload Size Writeup

## Challenge Description
Upload a file larger than 100 kB.

## Solution
1. I found the file upload feature in the application.
2. I noticed it had a client-side restriction on file size (100 kB limit).
3. I used browser developer tools to modify or remove the size restriction.
4. I uploaded a file larger than 100 kB successfully.
5. Alternatively, I intercepted the request and modified it before sending.

## Steps
- Find the file upload feature
- Try uploading a large file and note the error
- Open Developer Tools and inspect the upload form
- Remove or modify the size restrictions in the HTML
- Upload a file larger than 100 kB

## Reflection
This challenge showed me that client-side validation can always be bypassed. If an application really needs to limit file sizes, it must check on the server side too. Never trust the client!

## OWASP Top 10 Category
**A04:2021 - Insecure Design**
This challenge demonstrates the weakness of client-side only validation and the need for proper server-side controls.