---
title: Tableau and Data Visualization Tutorial
author: Zachary Reddick
date: 2017-03-28
---
## Installation:
1. A free trial of Tableau online is available for download [here](https://www.tableau.com/products/trial).

2. But your FSU emails allow you free access to Tableau’s full Desktop suite,
download here: (https://www.tableau.com/academic)

3. At the bottom of the page click “Students” and then follow the steps on the
next page to download your copy of Tableau. **Be sure to use your FSU email address**.


## Overview:

1. Tableau is a powerful tool that can be used to view, manipulate, explore, and
analyze data.

2. For the purposes of this course, Tableau is useful to engage with the results
 from our Xpath queries.

3. After downloading and installing the [software](https://onlinehelp.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-home.html)
, follow along with the video tutorials will help get you up to speed:


## Walkthrough:

1. First, let's gather data to explore in Tableau.

2. Using this query: `//table[@xml:id="deg-ta-cotn01"]//cell[contains(.,'balles')]/following-sibling::cell[1]`, returns the amount of bales of cotton exported. Right click on the results and save to a temporary file.

3. We will want to do more than just explore total cotton exports so let's also run this query:`//table[@xml:id="deg-ta-cotn01"]//cell[contains(.,'Angleterre')]/following-sibling::cell[1]`, along with France, Russie, Autriche, Italie, Allemagne, Espagne, and other countries to acquire the cotton export numbers to each respective destination.

4. The resulting data from each of these queries will be quite raw. We can use [Regular Expressions](https://dig-eg-gaz.github.io/how-to/regular-expression-instructions/) to clean up our data before putting it into Tableau.

5. The ![spreadsheet](cotton-exports.xlsx) we create should contain the following variables: Month, Country, and Total Cotton Export (Bales).

6. Now that we have data representing cotton exports to monthly totals and where they are being shipped to we want to visualize this data.

7. Open Tableau, and click Connect to a File in the upper left corner, and select the datasheet from your system.

8. While in the Data Source interface, change the “Month” column from string to date value by Clicking on the “Abc” icon and selecting “Date” from the drop down menu. Set the “Country” column's geographic role to "Country/Region". At the bottom, click Sheet 1.

9. After dragging and dropping the “Total Cotton Export (Bales)” cell in the row slot, place the “Month” cell in the column slot, under Marks select “Bar”. ![Cotton Exports](1905-cotton-export-total) The resulting visual gives us an annual total of exports, but we can go deeper.

10. In the column slot, click the “Date” cell and select “Month”. This provides a clearer representation of fluctuations in the cotton export value during the year. If we select the second “Month” in the drop down menu it provides a visualization that includes zero value months.![Cotton Exports](1905-monthly-cotton-exports.png)

11. In the "Marks" box select "Label", and click the box next to "Show Mark Labels". Now our data is effectively communicating the monthly totals of cotton exports. Now let's incorporate each destination to further increase the accuracy of the data.

12. Drag and drop the "Country" cell into the Color box. Now we can see that a majority of the cotton exported every month was shipped to England ![Cotton Exports](cotton-exports-by-country).

13. For a simpler comparative drag and drop the "Country" cell into the Filters box, click none, then select which countries you want to compare. For now let's look at the difference between cotton exports to England and France ![Cotton Exports to England and France](cotton-exports-england-france).

14. To create a different kind of visualization clear the Columns and Rows then drag and drop the "Country" cell into the Columns slot and "Total Cotton Export" into the Rows slot. On the right hand side of the interface click "Show Me", and select the Symbol Map option. The resulting image depicts the amount of comparative cotton exported to each location. ![Global Cotton Exports](global-cotton-exports)

15. To save our visualizations, click “Story”, “New Story”. Drag the desired sheet to the designated location. Click “Story”, “Export Image”.


## Conclusion:

Tableau is great for creating visualisations from your data, but it also is useful for data exploration. When we create data visualisations it is important to remember to keep graphics simple and self-explanatory. For independent data exploration, however, we can try simple as well as complex approaches. Experiment with your data in the software to not only create graphics, but to see how different visualisations help you think about your research.
