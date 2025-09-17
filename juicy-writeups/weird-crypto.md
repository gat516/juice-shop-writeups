# Weird Crypto Writeup

## Challenge Description
Inform the shop about an algorithm or library it should definitely not use the way it does.

## Solution
1. I looked for cryptographic implementations in the application.
2. I found base64 encoded or hashed values in various places.
3. I discovered that the app uses MD5 hashing which is known to be insecure.
4. I submitted feedback about not using MD5 for security purposes.
5. The challenge was completed when I mentioned the specific crypto weakness.

## Steps
- Look for hash values or encoded data in the app
- Research common cryptographic weaknesses
- Submit feedback mentioning MD5 or other weak crypto
- Specifically mention why the algorithm is insecure

## Reflection
This challenge taught me about cryptographic security. MD5 is old and broken - it can be cracked easily now. Modern apps should use SHA-256 or better algorithms. Security is always evolving!

## OWASP Top 10 Category
**A02:2021 - Cryptographic Failures**
This challenge highlights the use of weak cryptographic algorithms and the importance of keeping cryptographic practices up-to-date.