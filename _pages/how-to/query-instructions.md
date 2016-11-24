---
layout: page
title: Querying the digital Egyptian Gazette
permalink: /how-to/query-instructions
header:
  image_fullwidth: front-page.jpg
---
## Searching your own files

Open the file(s) that you wish to search in the Oxygen XML editor. Locate the XPath query box near the top left. You can return a list of elements using simple queries, which be displayed at the bottom of the editor. Click on any item in this list to be taken to that location in your file.

- a list of all the "divs" in your file: `//div`
- a list of all the item-type divs in your file: `//div[@type="item"]`
- a list of all the item-type divs in your file containing the word "cotton": `//div[@type="item"][contains(., 'cotton')]`
- all tagged names of persons or places in the files: `//persName` or `//placeName`

## Searching the full contents of the digital Egyptian Gazette

To search everything in the [Digital Egyptian Gazette content repository](https://github.com/dig-eg-gaz/content), you will have to use Oxygen's project function. Create a new project, then right click to add a folder--this should be a copy of the content repository on your local computer. (If you don't have one, download it from Github). Then change the icon at the left edge of the query box to search project.

This will return lots of results. It will be useful for you to refine these somewhat, using expressions such as:

- `//placeName[contains(.,'Aden')]`

## Resources

- [XPath functions list](http://www.w3schools.com/xml/xsl_functions.asp)
- [XPath tutorial](http://www.w3schools.com/xml/xpath_intro.asp)
- Got a question or comment? File an issue [here](https://github.com/dig-eg-gaz/dig-eg-gaz.github.io/blob/master/_pages/how-to/query-instructions.md).

Looking at prices for cotton: //table//cell[contains(.,'Cotton')]/following-sibling::cell[4]

//div/@type[contains(.,'wireReport')]/parent::div//dateline
//div/@type[contains(.,'wireReport')]/parent::div//dateline//placeName

Right click on results, export file, fix with regex.
