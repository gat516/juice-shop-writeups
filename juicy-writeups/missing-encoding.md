# Missing Encoding Writeup

## Challenge Description
Retrieve the photo of Bjoern's cat in "melee combat-mode".

## Solution
1. I found references to photos in the photo wall or gallery section.
2. I looked at the image URLs and noticed they had encoded names.
3. I found an image with an unusual filename that wasn't displaying properly.
4. The image URL had special characters that weren't encoded correctly.
5. I accessed the raw image URL directly to see Bjoern's cat photo.

## Steps
- Go to the photo wall section
- Inspect image URLs in the Developer Tools
- Look for images with encoding issues in their names
- Access the problematic image directly

## Reflection
This challenge taught me about URL encoding and how special characters can cause problems in web applications. It's important to properly encode all user input and file names.

## OWASP Top 10 Category
**A05:2021 - Security Misconfiguration**
This challenge demonstrates improper handling of file names and URL encoding, leading to accessible content that should be properly managed.