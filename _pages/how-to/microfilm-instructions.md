---
layout: page
title: Microfilm instructions
permalink: /how-to/microfilm-instructions/
author: Will Hanley
image:
  image_fullwidth: masthead.jpg
---
1. Get film NP 486 for the appropriate month and year from the reserve desk in the basement in Strozier. You can sign it out for two hours.
2. Log on to one of the six microfilm-enabled computers, and open the "Microform PowerScan" program. Indicate that you are using microfilm. Thread the film into the microfilm reader (a "ScanPro 1000"), carefully following the threading route mapped on the machine itself. Run a bit of film through the machine until you begin to see page images--the first foot of film is only black.
3. Familiarize yourself with the controls at the bottom of the program. The "Motorized Roll Film Control" allows you to move through the film and find the issue you need. The larger "Adjust Image" menu has numerous controls. If your image is only displaying as half screen, click the "Film Orientation" button and it will shift to full screen. You can play with the zoom until you see a whole page on the screen--you may have to move the carriage in the microfilm reader itself to center the image. You can focus, change the brightness, and so on, to give you a more readable result.
4. When you're happy with what you see, save what's on your screen. Under the Scan/Print tab, change the scan resolution to 600dpi. Press "Scan to Drive #1." Name your file following the standard dating format plus page number (YYYY-MM-DD-p1). Choose file type jpg.
5. Find the image files you've created on the computer's hard drive, and copy them to a USB key, save them to Dropbox, or save them some other way. Do not simply leave them on the microfilm computer.
6. Return the microfilm to the checkout desk--your classmates will need to find it.
4. The preceding steps produce a human-readable image, but this image will not be good enough for OCR. In order to produce a high-quality, OCR-ready image, it is necessary to scan the page in quarters, then stitch the image together. Zoom in on the image until the screen shows just the top left-hand quarter of the page, thus:

![quarter page example](images/quarter-page-example.jpg)

Make sure that you leave a bit of overlap, so that the image stitching software can do its task. Change the shape of the green box, which shows the part of the image that you will save to a file, so that it contains the edges of the print. Now you are ready to save it as an image file. Under the Scan/Print tab, change the scan resolution to 600dpi. Press "Scan to Drive #1." Name your file following the standard dating format plus page number plus a suffix for the top left hand corner (YYYY-MM-DD-p1a). Choose file type jpg. Then proceed to scan the bottom left hand corner (p1b), the top right (p1c), and the bottom right (p1d).
4. Stitch the four quarters into a single high-resolution file using the [Microsoft Image Composite Editor](http://research.microsoft.com/en-us/um/redmond/projects/ice/). The program is loaded on all of the scanning computers at Strozier. If you use a Windows computer, it is free to download for your own computer. When you open the program, click "New Panorama," import the four quarter images you just produced, click "Stitch," then click "Export." Choose image quality "superb," and save the file with the name "YYYY-MM-DD-p1.jpg". This is the file that you will use for subsequent work--save it to your hard drive.
4. Go ahead and do the same for all the pages of the issue. **Note:** You may find that certain pages (often page 1) are doubled on the microfilm. When this is the case, you only need scan one version of the doubled page.
7. Once you are satisfied with your images, upload them directly to the appropriate subfolder within the [page-images repository](https://github.com/dig-eg-gaz/page-images) repository on GitHub. There are four subfolders (one for each quarter of the year). Make doubly sure *before you upload* that your images are named exactly according to this format: `YYYY-MM-DD-p1.jpg` (substitute .png or .pdf if using those format).
