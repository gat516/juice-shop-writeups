# Zero Stars Writeup

## Challenge Description
Give a devastating zero-star feedback to the store.

## Solution
1. I went to the customer feedback page.
2. I noticed the star rating system only goes from 1 to 5 stars.
3. I opened the browser developer tools and inspected the rating elements.
4. I found the hidden radio button for 0 stars and enabled it.
5. I submitted feedback with 0 stars.

## Steps
- Go to `/#/contact`
- Open Developer Tools (F12)
- Find the rating input elements
- Look for the 0-star option that's disabled
- Enable it and select 0 stars
- Submit the feedback

## Reflection
This was a fun challenge! I learned how to manipulate HTML elements using browser tools. It shows that client-side validation isn't enough - you need server-side validation too.

## OWASP Top 10 Category
**A04:2021 - Insecure Design**
This challenge demonstrates how client-side controls can be bypassed, showing the need for proper server-side validation.