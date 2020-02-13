# Comparing Percentage of Foreign Born Residents in Baltimore and Miami 
Exploring the Opportunity Atlas (https://www.opportunityatlas.org/) data comparing fraction of all residents who were born outside of the United States in 2012-2016.
* A repository name that is descriptive of the analysis conducted

## Brief Description of Findings 
* README that summarizes findings (less than 250 words)
* Data Interpretation: What do your findings mean and why might this be important for you as a student and as you progress in your career? Highlight the similarities and differences in your city data analysis. Optional: tie-in examples of programs, initiatives, or policies that may work in one city but not in another.
* Compare any outcome data results and/or visualizations at the census tract level from Baltimore City with your hometown (or city where you’ve spent or would like to spend time) 
* Evaluate and interpret what the differences and similarities in your data analysis show and how you might want to monitor your own biases if you were to develop some sort of solution for Baltimore City.

## Background Data 
### Relevant Links
[Opportunity Atlas website](https://www.opportunityatlas.org/)

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

---

# Public GitHub Repo should also include:
* Original Excel documents
* Analyzed Excel documents with Excel formulas and data visualizations
  * Excel Data Analysis: Use general Excel data analysis tools to compare outcome measurements in Opportunity Atlas data such as Pivot Tables, VLOOKUP, data reorganization, and/or logic statements
  * Apply Excel or Google Sheets data analysis tools discussed in class (including, but not limited to Pivot Tables, VLOOKUP, chart generation, basic calculations, IF and other logic statements, and data reorganization) to data downloaded from the Opportunity Atlas.
