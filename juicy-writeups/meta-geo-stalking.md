# Meta Geo Stalking Writeup

## Challenge Description
Determine the answer to Emma's security question by looking at an upload of her.

## Solution
1. I found Emma's profile or uploaded photos.
2. I downloaded one of her uploaded images.
3. I checked the image metadata using tools or by viewing file properties.
4. The EXIF data contained GPS coordinates showing where the photo was taken.
5. I used the location information to answer her security question about her birthplace or favorite place.

## Steps
- Find Emma's uploaded photos
- Download an image file
- Check EXIF metadata for GPS coordinates
- Use coordinates to determine location
- Use location info to answer security question

## Reflection
This challenge was creepy! It showed how photos can contain hidden location data that reveals where they were taken. This is called "geotagging" and it's a privacy risk. People should remove metadata from photos before sharing them online.

## OWASP Top 10 Category
**A01:2021 - Broken Access Control**
This challenge demonstrates how metadata in user uploads can leak sensitive information that can be used to bypass security questions.