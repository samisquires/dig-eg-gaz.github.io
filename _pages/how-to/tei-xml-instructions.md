---
layout: page
title: TEI-XML instructions
permalink: /how-to/tei-xml-instructions/
author: Will Hanley
header:
  image_fullwidth: masthead.jpg
---

## Objective
These instructions guide you in transforming your plain text page files into a marked-up xml document that conforms to the standards of [TEI](http://www.tei-c.org) (the Text Encoding Initiative).

## 1. Set up your text editor
You can do the first parts of this work in your Atom text editor. Eventually, as your work becomes more sophisticated, you may wish to try the full-function Oxygen XML Editor, which offers a [free 30-day trial](http://www.oxygenxml.com/xml_editor/register.html). For now, however, learn the basics using Atom. But before you start, go to Packages > Settings View > Install, and install the `language-xml` and the `less-than-slash` packages.

## 2. Create an xml file
Copy and paste [this template](https://raw.githubusercontent.com/dig-eg-gaz/boilerplates/master/empty-issue.xml) into a new document. Name this document using the date of the issue and an xml extension (YYYY-MM-DD.xml). (This document will eventually contain all of the pages of the issue, so it is not necessary to add the page number to the document name.) and save it to a new folder (called "xml-content" or something similar) in your personal repository. When you save your document using the .xml extension in the name, Atom should render the xml code that the template contains in color, and will show "no issues" in green at the bottom of the page.

## 3. Fill in the header and paste in a page of text
Enter your name into the template (under `<editor>`), today's date (under `<edition>`, in text and numeric formats), and the issue date (under `<bibl>`, in text and numeric formats). Save your file. Open a page 3 text file that you've corrected, and copy the contents. Return to the xml file and locate the `<div type="page" n="3"> </div>` pair of tags. Paste page 3 text in between these tags. Atom will immediately tell you that you have many errors and issues. Don't fret--we'll address them in the next step. Save the file.

## 4. Add structural tags
Wrap the text in tags. For now, we'll limit ourselves to three tags:
-  `<div>`, which you can use for articles, items, or any division of the page that makes sense to you
- `<head>`, which indicates a headline
- `<p>`, which indicates a paragraph.

Type the code in the angle brackets at the start of the text you want to tag. Move your cursor to the end and hit alt-command-period, and the tag will automatically complete.

The `<div>` tag requires that you specify the type of division you are indicating. Write it this way: `<div type="item">`.
