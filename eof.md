# What is Hidden Data After the Image?

## What Stegmarc found
Data was found appended after the official end of the image file. The image displays normally, but extra bytes are hiding after the point where the image should stop.

## How image files are structured
Every image file format has a defined ending marker. For JPEG files, this is a specific two-byte sequence (FF D9). For PNG files, it's a chunk called IEND. Everything after these markers is ignored by image viewers — but it's still there in the file.

## What someone did
Someone deliberately added data after the image's end marker. Your photo app, browser, and operating system will show the image normally and never reveal this data. Only a tool like Stegmarc or a hex editor would detect it.

## What this means for you

**If you're a business owner:** This is not a watermarking technique. No legitimate watermarking tool appends data after the image end marker. If this fires on one of your images, it means someone modified the file after you distributed it.

**If you're a compliance officer:** This is the simplest and most detectable form of data hiding. The hidden bytes count tells you exactly how much data was appended. This is often used by non-technical actors because it requires no special software.

## What to do next
- Note the hidden bytes count in the report.
- Preserve the original file as evidence — do not resave it.
- A digital forensics professional can extract and decode the appended data.
