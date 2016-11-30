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

<!--- how to deal with case sensitive searches? --->

## Searching the full contents of the digital Egyptian Gazette

To search everything in the [Digital Egyptian Gazette content repository](https://github.com/dig-eg-gaz/content), you will have to use Oxygen's project function. Create a new project, then right click to add a folder--this should be a copy of the content repository on your local computer. (If you don't have one, download it from Github). Then change the icon at the left edge of the query box to search project.

This will return lots of results. It will be useful for you to refine these somewhat, using expressions such as:

- `//placeName[contains(.,'Aden')]`
- `//div/@type[contains(.,'wireReport')]/parent::div//dateline`
- `//div/@type[contains(.,'wireReport')]/parent::div//dateline//placeName`

An example of working your way through table cells, looking at prices for cotton:

- This query will look at all tables and return the value in the fourth cell to the right of the cell containing the word "Cotton": `//table//cell[contains(.,'Cotton')]/following-sibling::cell[4]`
- This query will look at the "Coton" table (which has an xml:id of "deg-ta-cotn01"), and return the value in the cell to the right of the cell containing the word "Russie":  `//table[@xml:id="deg-ta-cotn01"]//cell[contains(.,'Russie')]/following-sibling::cell[1]`

It is possible to combine regular expression and xpath searches by using the find/replace menu. <!--- explain further --->

## How do I search using xml:id?

For elements, use `//div[@xml:id="deg-el-cppa01"]`. For tables, use `//table[@xml:id="deg-ta-cppa01"]`.

## How do I export and manipulate results?

Right click on results, then export file. You can then clean up these results with regular expressions, to remove the parts you don't want. After this, you can work with the results in a spreadsheet.

## Resources

- [XPath functions list](http://www.w3schools.com/xml/xsl_functions.asp)
- [XPath tutorial](http://www.w3schools.com/xml/xpath_intro.asp)
- Got a question or comment? File an issue [here](https://github.com/dig-eg-gaz/dig-eg-gaz.github.io/blob/master/_pages/how-to/query-instructions.md).
