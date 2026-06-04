# What is JPEG Frequency Manipulation?

## What Stegmarc found
The chi-square detector found that the statistical patterns inside your JPEG image have been altered in a way that's consistent with hidden data being embedded.

## How JPEG images work
When you save a photo as a JPEG, your camera or software breaks the image into tiny 8×8 pixel blocks and converts each one into a set of numbers called frequency coefficients. These numbers describe the brightness and color patterns in that block — think of them like a fingerprint for each tiny piece of your image.

## What someone did to your image
Someone modified the least significant digits of these frequency coefficients to encode hidden information. This is like changing the last decimal place of thousands of numbers — the image looks identical to the human eye, but the statistical pattern of those digits reveals that they've been deliberately altered.

## What this means for you

**If you're a business owner verifying your watermark:** Your watermark is embedded in the JPEG frequency domain. Stegmarc detected it successfully. This is expected behavior — your watermark is working.

**If you received this image and didn't expect a watermark:** Someone has hidden data inside this image. The payload rate estimate tells you approximately how much of the image's capacity was used. You should investigate who created this image and what the hidden data contains.

## What to do next
- If this is your watermarked image: review the confidence score. Above 90% means strong detection.
- If this is unexpected: consult a digital forensics professional to extract and examine the hidden payload.
