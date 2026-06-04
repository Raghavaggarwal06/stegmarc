# What is a C2PA Watermark?

## What Stegmarc found
Stegmarc detected and decoded an Adobe TrustMark watermark in this image. The decoded payload is shown in your report.

## What is C2PA?
The Coalition for Content Provenance and Authenticity (C2PA) is a standard created by Adobe, Microsoft, Google, the BBC, and others to help people verify the origin of digital content. It answers the question: "Where did this image actually come from?"

## What TrustMark does
TrustMark embeds an invisible, robust watermark directly into the image pixels using a neural network. Unlike a visible logo or caption, this watermark:
- Is completely invisible to the human eye
- Survives JPEG compression, resizing, cropping, and color adjustments
- Can be decoded to reveal who created the image and when
- Is used by AI image generators to identify AI-generated content

## What this means for you

**If you're a business owner who embedded this watermark:** The watermark was successfully detected and decoded. The payload matches what you embedded. Your content provenance system is working correctly.

**If you received this image:** This image carries a TrustMark watermark. The decoded payload in your report identifies the original creator or distributor. This is most commonly used by AI image generation platforms to label their output.

## What to do next
- The decoded payload is shown in your report. This is the identifier the creator embedded.
- Visit [contentauthenticity.org](https://contentauthenticity.org) to learn more about the C2PA standard and how to verify content authenticity.
