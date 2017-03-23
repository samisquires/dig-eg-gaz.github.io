---
layout: page
title: Digital Egyptian Gazette Schema
permalink: /schema/
header:
  image_fullwidth: front-page.jpg
---
This page describes the schema used in the Digital Egyptian Gazette project, which lives [here](https://github.com/dig-eg-gaz/resources/blob/master/egSchema.odd) in [ODD (‘One Document Does it All’)](http://www.tei-c.org/Guidelines/Customization/odds.xml) format.

The schema expressed in relaxNG compact (made from .odd files using the [Roma tool](http://www.tei-c.org/Roma/) at [TEI-c.org.](http://www.tei-c.org/Roma/)) is [here](https://github.com/dig-eg-gaz/resources/blob/master/egSchema.rnc). It can be validated against by using the URL [https://raw.githubusercontent.com/dig-eg-gaz/resources/master/egSchema.rnc](https://raw.githubusercontent.com/dig-eg-gaz/resources/master/egSchema.rnc) in an XML editor.

In addition to the tags offered by the [TEI P5 guidelines](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/index.html), the customized schema employs the following terms.

## `<div>` attributes

### Type
- masthead
- page
- section
- subsection
- article
- item
- wireReport
- advert

### Scope
- advertisement
- international
- local
- financial
- weather
- newspaper
- social
- sporting
- official
- maritime
- classifieds
- letters
- calendar
- measurements
- announcements
- municipality

### Site
- Alexandria
- Cairo
- Suez
- Port Said
- Suakin

### Source
- local
- wire

### Element
- weather: Daily Weather Report
- wire: Telegrams
- local: Local and General
- sport: Sport and Play
- social: Personal and Social
- coce: Calendar of Coming Events
- pass: Passenger List
- visit: Visitors' List
- letters: Letters to the Editor
- khedive: The Khedive
- army: Army and Navy / Army of Occupation / Egyptian Army / Naval Notes
- londonLetter: Our London Letter
- parisLetter: Our Paris Letter
- notesPortSaid: Notes from Port Said
- notesSuez: Notes from Suez
- notesSuakin: Notes from Suakin
- notesKhartoum: Notes from Khartoum
- notesConstantinople: Notes from Constantinople
- notesCyprus: Notes from Cyprus
- notesSudan: Notes from the Sudan
- notesFayoum: Notes from Fayoum
- notesOther: Notes from other places

## `<measure>` attributes

### Units
- tal: Talari
- cantar: qantar
- £: British Pounds Sterling
- fcs: francs
- sh: shillings
- LE: Egyptian pounds (livres égyptien)
- balles: bales of cotton
- ton: tonnes
- dC: degrees celsius
- mm: millimeters
- pt: piasters tarif
- min: minutes
- LE M: Egyptian pounds and millimes
- ard: ardeb
- $: US dollars
- sack: sacks

### Commodity
- currency

### Type
- indexNo: number corresponding to indexing system for newspaper elements, especially paid advertisements

## Columns
- cols: Specifies the number of columns in a given section
- colSpan: Used to specifies the width of a div which spans multiple columns and cannot be accurately described using the cols and cb elements.
