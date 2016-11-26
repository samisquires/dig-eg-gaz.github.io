---
layout: page
title: Templating instructions
permalink: /how-to/templating-instructions/
author: Will Hanley
header:
  image_fullwidth: masthead.jpg
---
## Objectives

While parts of the *Egyptian Gazette* were composed fresh each day, much of each issue consisted of templates reapplied with minor or no modifications from issue to issue. As we produce our marked-up version of the newspaper, we can save efforts by reusing templates in our own work. We must remain alert to minor variations, however.

## Recurring elements

[This table](https://docs.google.com/spreadsheets/d/118Zv13fpHfm67i1k0Sm79OThV4ApD-d1iccvrpw1iYU/edit?authuser=0) lists items commonly present in issues of the *Egyptian Gazette*. For a given date, the page and column number are listed. [This powerpoint presentation](https://docs.google.com/presentation/d/1vMoj-5ktfUAsfXrEbQJqy8vSsKhYiVyGVIZZqefrJW0/edit?authuser=0) displays the content layout of several issues during the month of July 1905. (The main boilerplate is six pages long. On Wednesday and Saturday, when issues are eight pages, the extra pages are the fourth and fifth pages. Pages 6-8 of extended editions correspond to pages 4-6 of regular editions.)

Advertisements and financial reports form the greatest part of the templated content, and each is dealt with in separate sections. The complete catalog of advertisements is [here](https://dig-eg-gaz.github.io/advertisements/). And the complete catalog of financial tables is [here](https://dig-eg-gaz.github.io/financial-tables/). Below we discuss a few other miscellaneous templates.

Once you've identified the relevant template, copy and paste the xml into your own file, then customize the template content to match your issue's content. **Important**: Only copy the material contained within the `<body> </body>` tags--the rest of the file should not appear in your issue file. To do so, select the text like this:

![copy-paste-example](https://github.com/dig-eg-gaz/dig-eg-gaz.github.io/blob/master/images/advertisement-copy-paste.png?raw=true)

Paste only this portion of the text into your issue document.

### 1. Daily Weather Report

![Daily Weather Report](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/daily-weather-report.png?raw=true "Daily Weather Report")

This element typically appears on page 2. A template is [here](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/daily-weather-report.xml). It may be most efficient to use the author view in Oxygen to enter particulars.

### 2. Newspaper Subscriptions

![Subscription and Advertisements](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/subscriptions-advertisements.png?raw=true)
![Publishing Information](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/publishing-info.png?raw=true)

These elements come side by side on page 2, though sometimes material is placed in the middle of them. Templates are [here](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/subscriptions-advertisements.xml) and [here](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/publishing-info.xml).

In the latter pages of the newspaper, we also find a brief item explaining where and when the paper is sold. Template is [here](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/egyptian-gazette-en-vente.xml).

![Egyptian Gazette en vente](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/egyptian-gazette-en-vente.png?raw=true)

### 3. Calendars
These calendars are lightly formatted. The Calendar of the Week ([xml template here](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/calendar-of-the-week.xml), xmlid:"deg-ta-cow01") seems to have been changed only once per week. The Calendar of Coming Events ([xml template here](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/calendar-of-coming events.xml), xmlid:"deg-ta-cce01") changed each day it appears, moving future elements downwards.

![Calendar of Coming Events](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/calendar-of-coming-events.png?raw=true)

![Calendar of the Week](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/calendar-of-the-week.png?raw=true)

### 4. Municipality
Municipal tenders appear in a formulaic fashion; it is necessary to change dates and particulars of the project being tendered. Template is [here](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/municipalite-avis.xml)

![Municipalite Avis](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/municipalite-avis.png?raw=true)

### 5. Claims against the estate
Change name, rank, post, and dates on the [xml template](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/claims-against-the-estate.xml).

![Claims against the estate](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/claims-against-the-estate.png?raw=true)
