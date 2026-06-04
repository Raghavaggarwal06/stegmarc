# What is Adaptive Steganography?

## What Stegmarc found
The SRNet neural network detector found evidence of sophisticated, content-adaptive steganography — a technique specifically designed to be undetectable by statistical methods.

## What makes this different
Basic steganography hides data by modifying pixels uniformly across an image. Adaptive steganography is smarter: it analyzes the image content first, then hides data specifically in the areas with the most visual complexity — textured regions, edges, and noisy areas where changes are hardest to see and hardest to detect statistically.

## Why this matters
Adaptive steganography algorithms (WOW, S-UNIWARD, HILL) are the current state of the art in covert communication research. They are:
- Undetectable by chi-square and RS/SPA statistical tests
- Designed to minimize the statistical footprint of embedding
- Used in academic research and increasingly in real-world covert channels

SRNet is a deep learning model trained specifically to detect these advanced algorithms by learning the subtle patterns they leave behind — patterns invisible to classical statistical methods.

## What this means for you

**If you're a compliance officer:** This is a sophisticated embedding technique. Detection by SRNet at this confidence level indicates deliberate, technically advanced data hiding. This warrants escalation to a digital forensics team.

**If you're a business owner:** Adaptive steganography would not be introduced by a standard watermarking tool. If this fires unexpectedly, the image may have been modified by a technically sophisticated actor after leaving your control.

## What to do next
- Note the stego probability score. Above 70% is high confidence.
- Preserve the file in its current state.
- Consult a digital forensics professional for payload extraction.
