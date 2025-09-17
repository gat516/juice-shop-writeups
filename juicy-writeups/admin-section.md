# Admin Section Writeup

## Challenge Description
Access the admin section of Juice Shop.

## Solution
1. I tried to find an admin page by changing the URL to `/admin`.
2. The page exists but is protected by a login.
3. I tried default credentials like `admin`/`admin` but it didn't work.
4. Later, I found that you can access the admin page after logging in as an admin user (if you find or create one).

## Steps
- Go to `/#/admin` in the browser.
- If not logged in as admin, it will redirect or show an error.
- Try to find a way to log in as admin (maybe through other challenges).

## Screenshot
*(Insert screenshot here if required)*

## Reflection
This challenge was a bit harder because you need to find admin credentials or exploit another vulnerability. I learned to always check for hidden or protected pages in web apps.

## OWASP Top 10 Category
**A01:2021 - Broken Access Control**
This challenge involves bypassing access controls to reach an administrative interface.
