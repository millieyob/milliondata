# milliondata

title: "A3: Incarceration"
output: html_document
---

### Introduction

An introduction of the problem domain and a description of the variable(s) you are choosing to analyze (and why!)
Answer:

This incarceration Data Report is a report on population in California state. The goal of this report is about people who were in jail, specially both latinx and black who were in jail. The data set in this report was created by [Vera Institude](https://github.com/vera-institute/incarceration-trends). Which is use some of the data to make this report.

### Summary Information

Write a summary paragraph of findings that includes the 5 values calculated from your summary information R script

These will likely be calculated using your DPLYR skills, answering questions such as: 

1. In california state, there were a total of `r CA_county_total_jail` people in jail.
2. In california state, the county that had highest number of people in jail is `r CA_most_pop_jail`.
3. In california state, the average of latinx and male in jail is `r CA_avg_in_jail`.
4. The median of male and female in jail in california state is `r CA_median_in_jail`.
5. The state that had highest population is `r highest_states_total_pop`.


### The Dataset

Who collected the data?  
How was the data collected or generated?  
Why was the data collected?  
How many observations (rows) are in your data?  
How many features (columns) are in the data?  
What, if any, ethical questions or questions of power do you need to consider when working with this data?  
What are possible limitations or problems with this data?   (at least 200 words)


### Trends Over Time Chart

This chart is made in such a manner that readers may easily recognize the change in the number of people in Washington state (both men and women) detained between 2000 and 2013. Whether the x-axis covers the years 2000 to 2013 and the y-axis depicts the number of male and female detainees. Surprisingly, the pace of change for some of the people imprisoned in Washington state appears to have been quite constant over the past 13 years.


``````{r, echo = FALSE, code = readLines("CA_new_chart")}
```

### In California, there is a comparison chart between the Black and Latinx populations in prison.

The chart is designed to further explore and compare whether an increasing black population is correlated with a higher number of Black in prison. Scatter chart is selected to demonstrate a better correlation.
```{r, echo=FALSE, message=FALSE}
BL_pop_chart
```
### Map Incarcerated latinx and black population in jail in California state

The map is designed to show the number of population detained in each county in Washington. Dark blue is chosen to represent counties with the highest detained populations, light blue represents counties with fewer detained populations, and white means no data is available. This chart shows that most of the detained population is from LA County, California state.

```{r, echo=FALSE, message=FALSE}
new_map
```
