# What is Image Metadata?

## What Stegmarc found
The EXIF analysis detector examined the metadata embedded in your image — the invisible information that travels with every photo — and found anomalies that may indicate tampering or steganographic activity.

## What is image metadata?
Every photo taken by a camera or smartphone automatically records hidden information alongside the image: the date and time it was taken, GPS coordinates, camera model, exposure settings, and more. This information is called EXIF data (Exchangeable Image File Format).

## What Stegmarc looks for
- **Editing software fingerprints:** If the metadata shows the image was processed by known steganography tools (like Steghide or OpenStego), that's a direct indicator.
- **Time mismatches:** If the creation time and modification time don't match, the image was edited after it was originally created.
- **Missing metadata:** Images with no EXIF data at all are suspicious — most legitimate images from cameras and phones carry metadata. Stripping it is a common tactic to hide evidence of manipulation.
- **Unusual comment fields:** Hidden text is sometimes stored in metadata comment fields.

## What this means for you

**If you're a business owner:** Your watermarking tool may strip EXIF data as part of the embedding process. Check with your watermark provider whether this is expected behavior.

**If you're a compliance officer:** Missing or stripped metadata combined with other detector hits is a strong indicator of deliberate manipulation.
