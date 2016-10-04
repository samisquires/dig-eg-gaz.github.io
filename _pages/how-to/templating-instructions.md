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

[This powerpoint presentation](https://docs.google.com/presentation/d/1vMoj-5ktfUAsfXrEbQJqy8vSsKhYiVyGVIZZqefrJW0/edit?authuser=0) displays the page content structure of several issues during the month of July 1905. The main boilerplate is six pages long. On Wednesday and Saturday, when issues are eight pages, the extra pages are the fourth and fifth pages. Pages 6-8 of extended editions correspond to pages 4-6 of regular editions. [This table](https://docs.google.com/spreadsheets/d/118Zv13fpHfm67i1k0Sm79OThV4ApD-d1iccvrpw1iYU/edit?authuser=0) lists items commonly present in issues of the *Egyptian Gazette*. For a given date, the page and column number are listed. [Ad boilerplates](https://github.com/dig-eg-gaz/advertisements) are stored on a separate page.

Advertisements and financial reports form the greatest part of the templated content, and each is dealt with in a separate section below. Here we discuss a few other miscellaneous templates.

Once you've identified the relevant template, copy and paste the xml into your own file, then customize the template content to match your issue's content. *Important*: Only copy the material contained within the `<body> </body>` tags--the rest of the file should not appear in your issue file.

### 1. Daily Weather Report

![Daily Weather Report](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/daily-weather-report-1905-07-12.png?raw=true "Daily Weather Report")

This element typically appears on page 2. A template is [here](https://github.com/dig-eg-gaz/boilerplates/blob/master/Daily-Weather-Report.xml). It may be most efficient to use the author view in Oxygen to enter particulars.

### 2. Newspaper Subscriptions

![Subscription and Advertisements](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/subscriptions-advertisements.png?raw=true)
![Publishing Information](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/publishing-info.png?raw=true)

These elements come side by side on page 2, though sometimes material is placed in the middle of them. Templates are [here](https://github.com/dig-eg-gaz/boilerplates/blob/master/subscrptions-advertisements.xml) and [here](https://github.com/dig-eg-gaz/boilerplates/blob/master/publishing-info.xml).

### 3. Calendars

![Calendar of Coming Events](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/calendar-of-coming-events.png?raw=true)

![Calendar of the Week](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-images/calendar-of-the-week.png?raw=true)

These calendars are lightly formatted. The Calendar of the Week seems to have been changed only once per week.

## Advertisements

See complete catalog [here](https://dig-eg-gaz.github.io/advertisements/).

## Financial elements

See complete catalog [here](https://dig-eg-gaz.github.io/financial-tables/).
