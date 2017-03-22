---
layout: page
title: Structure
permalink: /structure/
header:
  image_fullwidth: front-page.jpg
---

# Page 1
Advertisements

# Page 2
Advertisements, one column of content, masthead

### Daily Weather Report
xml:id="deg-el-dawr01" [xml text](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/daily-weather-report.xml) tables xml:id="deg-ta-dawr01" xml:id="deg-ta-dawr02" xml:id="deg-ta-dawr03" xml:id="deg-ta-dawr04"

# Page 3
Miscellaneous articles, and

## Sections
Each of these sections (ought to) contain sub-items, most of them with headlines, often also bylines and datelines. <!-- I should make it a requirement that all sections contain xml:id -->
- Wire reports (international news) `xml:id="deg-el-intl01"`: treat wire reports as individual divs (`type="wireReport"`), each with its own `<dateline>` and `<title>`.

- Notes from: Port Said `xml:id="deg-el-nf-port01"`, Suez `xml:id="deg-el-nf-suez01"`, Suakin `xml:id="deg-el-nf-suak01"`, Khartoum `xml:id="deg-el-nf-khrt01"`, Constantinople `xml:id="deg-el-nf-cnst01"`(also including Constantinople Notes), Wadi Medani `xml:id="deg-el-nf-wame01"`, Assiout `xml:id="deg-el-nf-assi01"`, Luxor `xml:id="deg-el-nf-luxr01"`, Cyprus `xml:id="deg-el-nf-cypr01"`, Minet el Gamh `xml:id="deg-el-nf-miga01"`, Fayoum / Fayoum Notes `xml:id="deg-el-nf-faym01"`, the Sudan `xml:id="deg-el-nf-sudn01"`, Kafr Zayat `xml:id="deg-el-nf-kfrz01"`, Mena `xml:id="deg-el-nf-mena01"`, Helouan `xml:id="deg-el-nf-hlwn01"`, Keneh `xml:id="deg-el-nf-kena01"`

Section name|xml:id|Usual page|Notes
Local and General|`xml:id="deg-el-locl01"`|3|treat individual paragraphs as individual divs (`type="item"`), each with its own `<head>`
Sport and Play|`xml:id="deg-el-spor01"`|3|
Personal and Social|`xml:id="deg-el-pers01"`|3|
Calendar of Coming Events|`xml:id="deg-el-coce01"`||see template
Passenger List|`xml:id="deg-el-plst01"`||
Visitors' List|`xml:id="deg-el-vlst01"`||
Letters to the Editor|`xml:id="deg-el-lett01"`||
Native Press Comments|`xml:id="deg-el-napc01"`||
The Khedive|`xml:id="deg-el-khed01"`||
Steamer Movements|`xml:id="deg-el-stmr01"`||
Army and Navy / Army of Occupation|`xml:id="deg-el-army01"`||
Egyptian Army|`xml:id="deg-el-egar01"`||
Our London Letter|`xml:id="deg-el-lonl01"`||
Our Paris Letter|`xml:id="deg-el-parl01"`||
Egyptian Share Market|`xml:id="deg-el-egsh01"`
Bulletin de la bourse|`xml:id="deg-el-bdlb01"`
Chronique Financiere|`xml:id="deg-el-chrf01"`|4|
Chronique Judiciare|`xml:id="deg-el-chrj01"`|4|
Shipping Movements|`xml:id="deg-el-ship01"`|4|
Mouvement Maritime|`xml:id="deg-el-moma01"`|4|
Council of Ministers|`xml:id="deg-el-cmin"`|4|

Others:
- To-day's telegrams
- Legal Notes
- Questions municipales
- Pith of the Press Comments
- Esbekieh Gardens

# Page 5
- Matters of Moment
