# Login MC SafeSearch Writeup

## Challenge Description
Log in with MC SafeSearch's original password without SQL injection or any other bypass.

## Solution
1. I found clues about MC SafeSearch being a rapper.
2. I looked up information about this character and found references to "Mr. N00dles".
3. I tried common password variations related to his identity.
4. The password turned out to be "Mr. N00dles" (with zeros instead of o's).

## Steps
- Find MC SafeSearch's email address (usually visible in reviews or user lists)
- Try password: `Mr. N00dles`
- Log in successfully

## Reflection
This challenge required some research and thinking about the character. It shows how personal information can be used to guess passwords. People shouldn't use obvious personal details as passwords.

## OWASP Top 10 Category
**A07:2021 - Identification and Authentication Failures**
This challenge demonstrates how predictable passwords based on personal information can be easily compromised.