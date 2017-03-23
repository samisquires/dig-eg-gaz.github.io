---
layout: page
title: Regular expression instructions
permalink: /how-to/regular-expression-instructions/
author: Will Hanley
header:
  image_fullwidth: masthead.jpg
---
Regular expressions (regex) is a very useful means of working with serial data which repeats similar information using similar formats.

## Using regex in Atom

To put `<persName>` around passenger names in a list: find `Mr. [A-Z][a-z, 0-9]+,` replace with `<persName>$&</persName>`.

To convert `<p>Budapest, January 4.</p>` to `<dateline>Budapest, January 4.</dateline>`: find `<p>[A-Z][a-z]+, [A-Z][a-z]+ [0-9]+\.<\/p>` and replace with `<dateline>$&</dateline>`.

## Using regex in Microsoft word

Say you are trying to make a table of the results that you exported from Oxygen.

Import these results into a Word document. Then use Edit > Find > Advanced Find and Replace.

1. Find two paragraph marks (^p^p), and replace with @@.
2. Find one paragraph mark (^p), and replace with comma.
3. Find @@, and replace with paragraph mark (^p).
4. Select all text, then use Table > Convert > text to table.
