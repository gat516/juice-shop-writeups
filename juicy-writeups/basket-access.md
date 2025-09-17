# Basket Access Writeup

## Challenge Description
Access someone else's basket.

## Solution
1. I logged in with my own account and added items to my basket.
2. I noticed the basket API calls use a basket ID in the URL.
3. I went to `/#/basket` and checked the Network tab in Developer Tools.
4. I saw requests to `/rest/basket/1` where 1 was my basket ID.
5. I changed the URL to `/rest/basket/2` to access someone else's basket.

## Steps
- Log in and add items to your basket
- Open Developer Tools and go to Network tab
- Go to your basket page and observe the API calls
- Change the basket ID in the URL to access other baskets
- Try `/rest/basket/1`, `/rest/basket/2`, etc.

## Reflection
This is called an Insecure Direct Object Reference (IDOR). It's dangerous because you can access other users' private data just by changing numbers in the URL. Websites should check if you're authorized to see that data.

## OWASP Top 10 Category
**A01:2021 - Broken Access Control**
This challenge demonstrates Insecure Direct Object References (IDOR) where users can access resources by manipulating object identifiers.