# Repetitive Registration Writeup

## Challenge Description
Follow the DRY principle while registering a user.

## Solution
1. I went to the user registration page.
2. I noticed that the password and repeat password fields both exist.
3. I entered the same password in both fields as required.
4. But I found that if I manipulate the form data, I can bypass the repeat password check.
5. I used the browser developer tools to modify the form before submitting.

## Steps
- Go to the registration page
- Fill in user details
- Use the same password for both password fields
- Or manipulate the form data to bypass validation

## Reflection
DRY means "Don't Repeat Yourself" - a programming principle. This challenge was about not having to type the same password twice. It shows how client-side validation can be bypassed easily.

## OWASP Top 10 Category
**A04:2021 - Insecure Design**
This challenge demonstrates the weakness of relying solely on client-side validation for security controls.