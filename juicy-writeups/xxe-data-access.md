# XXE Data Access Writeup

## Challenge Description
Retrieve the content of C:\Windows\system.ini or /etc/passwd via XXE.

## Solution
1. I found an XML upload feature or API endpoint that processes XML.
2. I crafted an XXE (XML External Entity) payload to read system files.
3. I used a payload like: `<!DOCTYPE foo [<!ENTITY xxe SYSTEM "file:///etc/passwd">]><foo>&xxe;</foo>`
4. I uploaded or sent this XML and the application processed it.
5. The response contained the contents of the system file.

## Steps
- Find XML upload or processing functionality
- Create XXE payload to read system files
- Upload/submit the malicious XML
- Check response for file contents

## Reflection
XXE attacks are really dangerous! They can read any file on the server that the application has access to. This could include passwords, configuration files, or other sensitive data. XML processing should always disable external entities.

## OWASP Top 10 Category
**A03:2021 - Injection**
This challenge demonstrates XML External Entity (XXE) injection, where malicious XML can be used to read arbitrary files from the server filesystem.