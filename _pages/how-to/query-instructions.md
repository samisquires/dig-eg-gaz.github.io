---
layout: page
title: Querying the digital Egyptian Gazette
permalink: /how-to/query-instructions
header:
  image_fullwidth: front-page.jpg
---
## Searching your own files

Open the file(s) that you wish to search in the Oxygen XML editor. Locate the XPath query box near the top left. You can return a list of elements using simple queries:

- `//persName`
- `//placeName`

## Searching the full contents of the digital Egyptian Gazette

This approach works for the file that is currently open. But if you create a project using your fork of the [Digital Egyptian Gazette content repository](https://github.com/dig-eg-gaz/content), you can perform the same search on everything. To do so, just change the icon at the left edge of the query box.

This will return lots of results. It will be useful for you to refine these somewhat, using expressions such as:

- `//placeName[contains(.,'Aden')]`

## Resources

- [XPath functions list](http://www.w3schools.com/xml/xsl_functions.asp)
- [XPath tutorial](http://www.w3schools.com/xml/xpath_intro.asp)
