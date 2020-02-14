# Comparing Percentage of Foreign Born Residents in Baltimore, Maryland and Miami, Florida 
Exploring the Opportunity Atlas (https://www.opportunityatlas.org/) data comparing fraction of all residents who were born outside of the United States in 2012-2016.

## Brief Description of Findings
In the United States, the 14th Amendment of the Constitution guarantees birthright citizenship, where any child born in the US or one of its territories is granted American citizenship (some exclusions apply). Foreign-born residents can become citizens through the naturalization in process or through their parents by acquisition or derivation [1](https://immigration.findlaw.com/citizenship/u-s-citizenship-through-parents-or-by-birth.html). 

The United States has the largest foreign-born population of any country. In 2016, foreign-born residents made up 13.5% of the total US population [2](https://www.reuters.com/article/us-usa-immigration-data/u-s-foreign-born-population-swells-to-highest-in-over-a-century-idUSKCN1LT2HZ). Immigration not only has a broadly positive effect on the economy [3](https://budgetmodel.wharton.upenn.edu/issues/2016/1/27/the-effects-of-immigration-on-the-united-states-economy), but also influences the diversity of culture, food, and art of a region. 
As major cities, both Miami and Baltimore have a larger immigrant population than the country as a whole. 
Miami, has an average of (---)% foreign-born residents per tract in comparison to Baltimore's (---)%.
Due to this we can infer that Miami has a higher percentage of non-citizens, influencing employment opportunities and overall economy. 


foreign-born residents per tract. 


Due to ... we can infer that this means Miami has a large population of non-citizens which affects the employment opportunities overall economy. 

This means that Miami is more culturally diverse than Baltimore which influences the...  


from: https://www.census.gov/newsroom/pdf/cspan_fb_slides.pdf



from: https://opportunityinsights.org/wp-content/uploads/2018/10/atlas_paper.pdf
Share Foreign Born(2010).  The share foreign born variable that is shown in the OpportunityAtlas is constructed as the number of foreign born residents in the 2010 Census divided by the sumof native and foreign born residents (long form SF3a,  table NP021A) obtained from the NHGIS database

* README that summarizes findings (less than 250 words)
* Data Interpretation: What do your findings mean and why might this be important for you as a student and as you progress in your career? Highlight the similarities and differences in your city data analysis. Optional: tie-in examples of programs, initiatives, or policies that may work in one city but not in another.
* Compare any outcome data results and/or visualizations at the census tract level from Baltimore City with your hometown (or city where you’ve spent or would like to spend time) 
* Evaluate and interpret what the differences and similarities in your data analysis show and how you might want to monitor your own biases if you were to develop some sort of solution for Baltimore City.

## Background Data 
### Relevant Links
[Opportunity Atlas website](https://www.opportunityatlas.org/)

[Census: About Foreign Born](https://www.census.gov/topics/population/foreign-born/about.html)

[Original CSV Document: Baltimore Tract Foreign Born](https://github.com/CamilaCamacho/comparing_baltimore_miami_foreign-born/blob/master/baltimore_shown_tract_foreign_share2016.csv)

[Original CSV Document: Miami Tract Foreign Born](https://github.com/CamilaCamacho/comparing_baltimore_miami_foreign-born/blob/master/miami_shown_tract_foreign_share2016.csv)

[Analyzed Excel Document: Miami vs Baltimore](https://github.com/CamilaCamacho/comparing_baltimore_miami_foreign-born/blob/master/miami_vs_baltimore_tract_foreign_share2016.xlsx)


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
