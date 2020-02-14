# Comparing Percentage of Foreign Born Residents in Baltimore, Maryland and Miami, Florida 
Exploring the Opportunity Atlas (https://www.opportunityatlas.org/) data comparing fraction of all residents who were born outside of the United States in 2012-2016.

## Brief Description of Findings
The US has the largest foreign-born population of any country. In 2016, foreign-born residents made up 13.5% of the total US population [(1)](https://www.reuters.com/article/us-usa-immigration-data/u-s-foreign-born-population-swells-to-highest-in-over-a-century-idUSKCN1LT2HZ). Immigration have a broadly positive effect on the economy [(2)](https://budgetmodel.wharton.upenn.edu/issues/2016/1/27/the-effects-of-immigration-on-the-united-states-economy), and influence the diversity of culture, food, and art of a region. 

With an average of 10% foreign-born residents per tract, Baltimore has a smaller immigrant population than the country as a whole. Miami, on the other hand has a much higher immigration population with an average 55% foreign-born residents per tract.
In the histagrams below, it is clear that Miami has many more tracts with a higher percentage of immigrants than Baltimore. Baltimore has almost 400 tracts with 0%-25% foreign-born residents, only about 16 tracts have more than that but none exceeding 50%. Comparitively, a majority of tracts in Miami a population of 50%-75% foreign-born residents.

From this we can infer that Miami is more culturally diverse than Baltimore and that Miami might benefit more in the positive economical influence of immigration. This can also influence what political inititatives and policies are seen as important. For example, immigration and path to citizenship policies are much more important in Miami than in Baltimore because the population is more affected by these policies. 
As someone who was not born in the US, understanding the general demographics and level of diversity of a city is helpful because it gives insights into the size and strength of diverse cultural communities and the political leverage they might have. 

## Background Data 
### Relevant Links
[Opportunity Atlas website](https://www.opportunityatlas.org/)

[Census: About Foreign Born](https://www.census.gov/topics/population/foreign-born/about.html)

[Original CSV Document: Baltimore Tract Foreign Born](https://github.com/CamilaCamacho/comparing_baltimore_miami_foreign-born/blob/master/baltimore_shown_tract_foreign_share2016.csv)

[Original CSV Document: Miami Tract Foreign Born](https://github.com/CamilaCamacho/comparing_baltimore_miami_foreign-born/blob/master/miami_shown_tract_foreign_share2016.csv)

[Analyzed Excel Document: Miami vs Baltimore](https://github.com/CamilaCamacho/comparing_baltimore_miami_foreign-born/blob/master/miami_vs_baltimore_tract_foreign_share2016.xlsx)

[Share Foreign Born Variable](https://opportunityinsights.org/wp-content/uploads/2018/10/atlas_paper.pdf):
Share Foreign Born(2010).  The share foreign born variable that is shown in the OpportunityAtlas is constructed as the number of foreign born residents in the 2010 Census divided by the sumof native and foreign born residents (long form SF3a,  table NP021A) obtained from the NHGIS database

### Data Visualization
![alt text](https://github.com/CamilaCamacho/comparing_baltimore_miami_foreign-born/blob/master/Baltimore%20Histogram.png)
![alt text](https://github.com/CamilaCamacho/comparing_baltimore_miami_foreign-born/blob/master/Miami%20Histogram.png)

## Data Analysis Step-by-Step Instructions
### For each city:
1. Isolate fraction of foreign born residents per tracts for each city.
  * Copy and paste **tract** and **Foreign-Born_Share_in_2012-16** data columns into new sheet.
2. Reformat data into table.
  * Place cursor on any cell in data and [Edit -> Select All] (or use [Command+A] keyboard shortcut).
  * [Insert -> Table] and make sure selected data range is correct in dialogue box before clicking *OK*.
3. Change Number Format of **Foreign-Born_Share_in_2012-16** from _General_ to _Percentage_.
4. Because the data is in percentages from 0% to 100%, the bins for the histogram can be divided into 5 equally sized bin ranges: <=0%, 0%-25%, 25%-50%, 50%-75%, >75%.
  * List these _bin range_ as a cell range. 
5. Use the **FREQUENCY** function to count the number of tracts in which percentage of foreign born residents fall in each bin range.
  * Select cell range adjacent to bin ranges. 
  * Array enter formula: [=FREQUENCY(Tract_Foreign_Born_Table[Foreign-Born_Share_in_2012-16], _cell range of bin range_)] then press [Ctrl+Shift+Enter].
  * For Baltimore, it should look something like this: ![alt text](insert baltimore example here)
6. Create histogram.
  * Select bin ranges and frequency data and from Insert tab select **Clustered Column** chart.
  * Right-click on any column, select **Format Data Series...** and change **Gap Width** to zero (0).
