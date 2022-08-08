# An Analysis of Kickstarter Campaigns

Performing analysis on Kickstarter data to uncover trends.

# Kickstarting with Excel

## Overview of Project

Client's play, ***Fever***, barely made it's fundraising goal in a short amount of time. Now the client would like to see if there is a correlation between different play campaigns based on their launch dates and funding goals.

### Purpose

To find out how other play campaigns fared by making comparisons between their launch dates and funding goals.  

## Analysis and Challenges

In order to analyze the ***Kickstarters*** Dataset to determine crucial differences between a campaign's launch date and funding goal there are two different graphs generated:

1. Outcomes Based on Launch Date
2. Outcomes Based on Goals

The first analysis of Outcomes Based on Launch Date, the data was filtered to show campaigns that are in the "play" subcategory, with the measure being the launch date month for all years vs the count of outcomes in the columns "successful", "failed", and "canceled".  For the second analysis Outcomes Based on Goals the data was filtered to display only campaigns in the "play" subcategory, with the measure being different specified ranges of goal outcomes vs the number of "successful", "failed", or "canceled" plays that fail in the specified range. Both new filtered datasets have used line charts to display the results of the data. 

### Analysis of Outcomes Based on Launch Date

A PivotTable was generated with the Kickstarters dataset, the filters used were "subcategory" and "years", the Rows column was filled with the "Date of Conversion", the columns/legned was "Outcomes" and the measure for the table was count of "Outcomes". After setting up the correct parameters for the table "play" and "all years" was selected for the filters to display the different amounts of succesful, failed and canceled plays throughout the years based on what months they decided to launch their campaigns.

See Chart below for Outcomes Based on Launch Date:
<picture>
![Theaters_Outcomes_vs_Launch_Date](C:\Users\neang\OneDrive\Desktop\Data Analysis Project\Crowdfunding Analysis\PNGs\Theaters_Outcomes_vs_Launch_Date.png)
</picture>

### Analysis of Outcomes Based on Goals

Manually inputted the column names and first row with various goal ranges, then proceeded to use IFCOUNTS function to filter data based on criteria in the Kickstarters dataset. The filters used to populate the cells were based on only cells that were in the "play" subcategory, then filtered to three different categories "successful", "failed", or "canceled", then further filtered to include specific goal ranges. After this total outcomes in each ranges for the three different outcome categories were made in order to determine the percentage of each based on the specified goal ranges, i.e. percent of successful projects that reached less than $1000 of their goal. 

See Chart below for Outcomes Based on Goals
<picture>
![Outcomes_vs_Goals](https://github.com/vanessaneang/kickstarter-analysis/blob/main/PNGs/Outcomes_vs_Goals.png)
</picture>

### Challenges and Difficulties Encountered
The first analysis was fairly straightforward and utilized Excel's PivotTable function to generate the data chart. By doing so it was fairly easy to filter out the data and create a graph to coincide with the new PivotTable I generated for the analysis. The only initial challenge I had was taking out the extra information from the Date Created Conversion rows so it would show only the Months for all the years instead of the Quarters, but after I checked the Rows section for the Pivot Table I saw I could remove the unneeded information of the Date Created Conversion, so a more succint Month value was left.

However, in the second analysis the IFCOUNTS function was a bit tricky at first since I needed to edit the cells to ensure that each one had the right criteria to find the data based on the criteria I set. It took me a few tries to make sure all criteria was met and the ranges for the goals either included the initial and final goal numbers or excluded them. After painstakingly going through the formulas a few times and reviewing the videa I saw that I needed to include certain numbers and then my graph displayed the correct data as the example. For future projects that need to use this IFCOUNTS function it will be important to make sure to include all criteria the client may need, since checking with larger datasets may be too difficult to do, attention to details is definitely needed for this funtion to work and fill out the rest cells needed for a data sheet.

## Results

- **What are two conclusions you can draw about the Outcomes based on Launch Date?**

It appears that the most successful plays launch in May to June since the number for these two months are a lot higher than the others even including the other outcome categories. Also, the month of December has the least amount of plays that are produced as well as the least amount of successful plays that are produced. 

- **What can you conclude about the Outcomes based on Goals?**

Play campaigns with goals in the $45000 to $49999 ranges are highly likely to fail, but play campaigns that exhibit goals with ranges less than 5000 seem to have a higher success rate. 

- **What are some limitations of this dataset?**

There are not enough data points for plays, so many of the points specifically for the Outcomes vs Goals can be skewed since not all of the Goal ranges specified have many projects that are in that range so it can skew the percentage of successes and failures greatly since they can be based on one to two points. In order to minimize this error it may be bettter to make the goal ranges into larger and fewer categories to give a better estimate of since there will be more points per range rather than two to six points. 

- **What are some other possible tables and/or graphs that we could create?**

For the Outcomes vs Goals we could make stacked column graph and create two other data tables one for Outcomes vs Percentage Funded and another for Goals vs Percentage Funded, then make this table into a stacked column chart or line graph. This way we could see how much successful play campaigns make and whether it is better to have smaller goals to reach a higher success rate or if larger goals that are successful funded more.  
