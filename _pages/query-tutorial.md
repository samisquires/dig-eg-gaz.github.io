---
layout: page
title: Querying the digital Egyptian Gazette
permalink: /how-to/querying
header:
  image_fullwidth: front-page.jpg
---
Using Oxygen, locate the XPath query box near the top left. You can return a list of elements using simple queries:

- `//persName`
- `//placeName`

This approach works for the file that is currently open. But if you create a project, using your fork of the DEG content, you can perform the same search on everything. To do so, just change the icon at the left edge of the query box.

This will return lots of results. It will be useful for you to refine these somewhat, using expressions such as:

- `//placeName[contains(.,'Aden')]`
