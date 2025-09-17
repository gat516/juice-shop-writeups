# Login Admin Writeup

## Challenge Description
Log in as the admin user in Juice Shop.

## Solution
1. I tried to log in with common credentials like `admin`/`admin` and `admin`/`password`.
2. I checked the login error messages for hints.
3. Sometimes, you can find the admin email in the source code or by using password reset.
4. I used the password reset feature with `admin@juice-sh.op` and set a new password.
5. Then I logged in as admin.

## Steps
- Go to the login page.
- Click on "Forgot your password?"
- Enter `admin@juice-sh.op` and follow the reset instructions.
- Set a new password and log in as admin.

## Screenshot
*(Insert screenshot here if required)*

## Reflection
This challenge taught me to look for password reset features and try common admin emails. It was not too hard once I found the right email.

## OWASP Top 10 Category
**A07:2021 - Identification and Authentication Failures**
This challenge exploits weak authentication mechanisms and predictable admin email addresses.
