---
layout: page
title: Sections
permalink: /sections/
header:
  image_fullwidth: front-page.jpg
---

Most of the sections listed below (ought to) contain sub-items, most of them with headlines, often also bylines and datelines. These sections are identified using the `element=` attribute.

Section name|element (or deprecated xml:id)|Usual page|Notes
**[Advertisements](https://dig-eg-gaz.github.io/advertisements/)** |various|1,2|Use templates
**[Daily Weather Report](https://dig-eg-gaz.github.io/boilerplates-and-tables/#daily-weather-report)** |`deg-el-dawr01`|2|[xml text](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/daily-weather-report.xml)
**Telegrams / Wire Reports** (international news)|"wire"|2,3|Sometimes appears as "To-day's telegrams", but typically there is no heading for this section. Treat wire reports as individual divs (`type="wireReport"`), each with its own `<dateline>` and `<title>`. This section is sometimes spread over two pages; when this is the case, you can use the `next` and `prev` attributes.
**Local and General** |"local"|3|treat individual paragraphs as individual divs (`type="item"`), each with its own `<head>`.
**Sport and Play** |"sport"|3|Treat contents as items, each with own headline.
**Personal and Social** |"social"|3|Treat contents as paragraphs
**[Calendar of Coming Events](https://dig-eg-gaz.github.io/boilerplates-and-tables/#calendar-of-coming-events)** |`deg-el-coce01`|2-3|see [template](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/calendar-of-coming-events.xml) for format
**Passenger List** |"passList"|3,4,5,6,7|Treat arrivals and departures as items.
**Visitors' List** |"visitList"|3|Treat each hotel as an item.
**Letters to the Editor** |"letters"|3|Treat each letter as an item, with `<byline>` and `<dateline>`
**Native Press Comments** |"nativePress"|3|
**Matters of Moment. Pith of the Press Comments.** |"mattersMoment"|5|
**The Khedive** |"khedive"|3|
**Steamer Movements** |"steamerMovements"|3|Treat contents as paragraphs.
**Shipping Movements** |"shippingMovements"|4|
**Mouvement Maritime** |"mouvementMaritime"|4|French language
**Army and Navy / Army of Occupation / Egyptian Army** |"army"|3,4,5,7|
**Naval Notes** |"navalNotes"|3|
**Our London Letter** |"londonLetter"|7|
**Our Paris Letter** |"parisLetter"|7|
**Cheap Prepaid Advertisements** |"prepaidAdvertisements"|2,5,7|Section template [here](https://dig-eg-gaz.github.io/boilerplates-and-tables/#cheap-prepaid-advertisements). Treat each advertisement as an item.
**Egyptian Share Market** |`deg-el-egsh01`||
**Bulletin de la bourse** |`deg-el-bdlb01`||French language
**Chronique Financiere** |`deg-el-chrf01`|4|French language
**Chronique Judiciare** |`deg-el-chrj01`|4|French language
**Council of Ministers** |`deg-el-cmin`|4|

## "Notes from" section:
These notes typically appear on page 3. They are sourced to "Our Own Correspondent". Treat individual stories as `<div type="item">`, each with its own `<head>`. It is not always clear how many stories belong to the section.

Place|xml:id|Notes
Constantinople|"notesConstantinople"|also appears as Constantinople Notes
Port Said|"notesPortSaid"|
Suez|"notesSuez"
Fayoum|"notesFayoum"|also appears as Fayoum Notes
Cyprus|"notesCyprus"
The Sudan|"notesSudan"
Suakin|"notesSuakin"
Khartoum|"notesKhartoum"
Assiout|"notesAssiout"
Luxor|"notesLuxor"|also appears as Luxor Notes
Kafr Zayat|"notesKafrZayat"
Other|"notesOther"|Notes from Akhmin, Keneh, Kafr Zayat, Minet el Gamh, Wadi Medani, and other places in Egypt

Others:
- Legal Notes
- Questions municipales
- Esbekieh Gardens
- Egyptological Notes
- Cheap Advertisements
