---
layout: page
title: Digital Egyptian Gazette Schema
permalink: /schema/
header:
  image_fullwidth: front-page.jpg
---

# `<div>` attributes

# Type
- masthead
- page
- section
- subsection
- article
- item
- wireReport
- advert

# Scope
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

# Site
- Alexandria
- Cairo
- Suez
- Port Said
- Suakin

# Source
- local
- wire

# Element
- weather: Daily Weather Report
- wire: Telegrams
- local: Local and General
- sport: Sport and Play
- social: Personal and Social
- coce: Calendar of Coming Events
- pass: Passenger List
- visit: Visitors' List
- letter: Letters to the Editor
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

# `<measure>` attributes

## Units
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

## Commodity
- currency

## Type
- indexNo: number corresponding to indexing system for newspaper elements, especially paid advertisements

# Columns
- cols: Specifies the number of columns in a given section
- colSpan: Used to specifies the width of a div which spans multiple columns and cannot be accurately described using the cols and cb elements.
