# What is Pixel-Level Data Hiding?

## What Stegmarc found
The RS Analysis or Sample Pair Analysis detector found evidence that individual pixel values in this image have been modified to carry hidden data.

## How digital images store color
Every digital image is made up of millions of tiny dots called pixels. Each pixel stores three numbers — one for red, one for green, one for blue — each ranging from 0 to 255. The last digit of each number (called the least significant bit) has almost no effect on how the color looks.

## What someone did to your image
Someone replaced the last digit of thousands of pixel values with bits of their hidden message. Changing a pixel's red value from 128 to 129 is completely invisible to the human eye — but across enough pixels, it creates a detectable statistical pattern.

## What this means for you

**If you're a business owner:** Pixel-level embedding is a different technique from watermarking. If this detector fires on an image you watermarked, it may indicate a secondary hidden payload was added after your watermark — or that your watermarking tool uses spatial pixel embedding.

**If you're a compliance officer:** This type of embedding is commonly used for covert communication. The payload rate estimate tells you what fraction of pixels were modified.

## What to do next
- Check the payload rate. Above 30% suggests significant data was hidden.
- Run the analysis with a cover image (the original) to get PSNR/SSIM quality scores confirming the modification.
