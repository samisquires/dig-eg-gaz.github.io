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

## 1. Set up your XML editor
Download the full-function Oxygen XML Editor, which offers a [free 30-day trial](http://www.oxygenxml.com/xml_editor/register.html). After 30 days, you might find [ways](https://10minutemail.com/) to renew your trial access, or simply purchase Oxygen using their [academic and educational discount](http://oxygenxml.com/academic/)).

## 2. Create an xml file
Copy and paste [this template](https://raw.githubusercontent.com/dig-eg-gaz/boilerplates/master/empty-issue.xml) into a new document. **Important**: the new document will have `<?xml version="1.0" encoding="UTF-8"?>` as its first line, and it's also the first line of the template; delete one of them, otherwise your document will be ill-formed. Name this document using the date of the issue and an xml extension (YYYY-MM-DD.xml). (This document will eventually contain all of the pages of the issue, so it is not necessary to add the page number to the document name.) Save this document on your hard drive.

## 3. Fill in the header and paste in a page of text
Enter your name into the template (under `<editor>`), today's date (under `<edition>`, in text and numeric formats), and the issue date (under `<bibl>`, in text and numeric formats). (Currently, these areas have entries in the comment format (`<!-- -->`)--replace these with your text). Save your file. Open a page 3 text file that you've corrected, and copy the contents. Return to the xml file and locate the `<div type="page" n="3"> </div>` pair of tags. Paste page 3 text in between these tags. Atom will immediately tell you that you have many errors and issues. Don't fret--we'll address them in the next step. Save the file.

## 4. Add structural tags
Wrap the text in tags. For now, we'll limit ourselves to three tags:
-  `<div type="item">`, which you can use for articles, items, or any division of the page that makes sense to you,
- `<head>`, which indicates a headline (the headline must be the first element in the item),
- `<p>`, which indicates a paragraph.

Oxygen offers many shortcuts to make this work go faster. Highlight the text you wish to wrap, then hit `command-E`. You will be offered a menu of tags. Choose the one you want. If you want to add more tags of the same type, hit `command-slash`.

## 5. Make sure that your document is well-formed
At the top right hand corner of your editing window in Oxygen, there is a square that will be either red or green. If it's green, your document is well-formed, which means that it conforms to TEI XML standards and will be searchable and useable. If it's red, the file contains errors that you must fix before you submit it. The errors appear as red lines on the right hand scrolling column. Click on a line to see the error described at the bottom of your editing screen.

## 6. Fork the organization content repository and save to GitHub

Once you've completed some of the structural tagging of your page, it's time to save it to GitHub. We're going to use the "fork" and "pull" functions of GitHub to do this. First, "**fork**" the [dig-eg-gaz/content](https://github.com/dig-eg-gaz/content) repository by clicking on the "fork" icon on the top right. You will be offered the chance to fork the repository under your own username--do so. This will make a copy of the repository in your own GitHub account, in which you should save your .xml page files. Later, when your page files are complete, you can fold them back into the organization content repository by sending me a **pull request**. You do this by clicking the "new pull request" button the top left above your list of files. I will then see the pull request and either merge your files into the organization's content or request that you change something before doing so.

## 6. Common errors
- **&**: the ampersand is represented as `&amp;` in xml. `&` alone will create an error.
- **>** or **<**: the OCR process produces stray angle brackets. The editor thinks these are part of a xml tag, and it causes an error.
- anything not in a `<div>`
- doubled `<?xml version="1.0" encoding="UTF-8"?>` lines at the opening of the xml document.

## 7. Add more complex tags
There are more tags that you can add:
- If the article or item is in French, add the attribute `xml:lang="fr"` to the `<div>` tag.
- **`<cb/>`** for column breaks. Be sure to put this tag at the *beginning* of the column. Add the number of the column, as well, thus: `<cb n="1"/>` For mixed columns, see [this guidance](http://dcs.library.virginia.edu/digital-stewardship-services/tei-encoding-guidelines/#cb).
- **`<div type="section">`** to wrap multiple items that belong together, for instance in the international or local news sections.
- **`<dateline>`** for datelines. There can only be one dateline per division. In the international news section, this means that you must make a new `<div type="item">` for each newswire report.
- **`<byline>`** for authors. There can only be one byline per division.
- **`<gap/>`** for holes in the text, **`<unclear>`** for illegible text (you can supply an attribute explaining why), and **`<supplied>`** for something that was illegible but which you figured out by finding the same thing in a different issue.
- pieces of articles that are continuous texts broken up by ads or between issues should be connected using xml:id and the next and prev elements, thus: if the articles are in the same issue, make their tags `<div type="item" xml:id="item1" next="item2">` and `<div type="item" xml:id="item2" prev="item1">`. If the articles are in different issues, make their tags `<div type="item" xml:id="item1" next="YYYY-MM-DD.xml#item2">` and `<div type="item" xml:id="item2" prev="YYYY-MM-DD.xml#item1">`.
- the **`<figure>`** element will be useful for the *Egyptian Gazette*, but I have not yet worked out how to use it.

## Resources
- “[A Gentle Introduction to XML](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/SG.html),” TEI Consortium.
