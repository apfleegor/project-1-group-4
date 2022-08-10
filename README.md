# Project 1, Group 4: What Makes People Happy?

Team Members: Alexandra Pfleegor, Ken Condit, Eric Zhu, Myles Browne, Drew Blankenbiller, Chuck McManus

## Background
What makes people happy? 

![happiness_banner](Images/happiness-banner.jpg)

Is it Family Structure? Tennis? Weather? Marriage? Crime? The Housing Market? Access to Parks? 

Our group decided to dig deeper into Gallup's 2018 Well-Being Poll of Americans by State. 

# Table of Contents 
* Data Sources
* Data Cleaning and Exploration
* Tennis
* Housing Costs & Weather
* Crime
* Family Structure
* Number of Parks

# Data Sources 
* 2018 Gallup Poll Well-Being Index
* Historical Climate Data from the National Centers for Enivronmental Information
* Housing Data from Realtor.com for 2018
* 2018 American Community Survey from the US Census Bureau
* Tennis courts in the US database from data.world https://data.world/mglobel/tennis-courts
* 2018 State Populations data from census.gov https://www.census.gov/newsroom/press-kits/2018/pop-estimates-national-state.html
* manually gathered by state counts of publicly available tennis courts (via google search engine)
* 


# Data Cleaning and Exploration 

## Tennis Anyone? 
### Inspiration:
In considering the well-being index across the 50 states, why think of tennis as a comparator?  The well-being attributes of tennis are plentiful and multi-dimensional. As a tennis player, I became curious to see if I could find data across the 50 states that could be used as explanatory for the well-being index.  Some of my favorite attributes of tennis:
        - Physically challenging
        - Mentally engaging
        - Can be played competitively or recreationally
        - Is great exercise because  it is so fun, you don't even know you're exercising
        - Builds character and discipline through self-refereeing / line calling
        - Is social and a great way to make new friends
        - Is economical and can be played almost anywere
        - Is available to a wide array of groups across the socio-econimic spectrum
        - Has a positive carryover effect on nearly all other aspects of your life

### Hypothesis:
Developed a working hypothesis once sources found: Because of all of it's positive well-being attributes, tennis has to have a strong positive relationship with the Well-Being Index as captured by Gallup.  Doesn't it??? 

I set out to prove this by looking at data on public tennis court locations as a proxy for the availability and participation of tennis across 50 states.

### Data Discovery:
- 89,000 + locations found in the data
- Max Raw (California): 12,800+ locations
- Min Raw (Delaware): 356 locations

### Data Methodology:
- I deceded to use the prevalence of publicly available tennis courts as an indicator of the level of tennis activity within each state.
- I used raw locational data to group data by state and come up with counts of publicly available tennis courts; concatenated a smaller set of counts of publicly available tennis courts by state to come up with a full dataset for the count of courts by state.
- I used state court data with state population data create base value for an index by which to rank states by availaibilty of public tennis courts.
- I summarized the relationship with a scatter chart; I expected to see low public tennis court availability in conjunction with low well-being index scores, and high public tennis court availabilty index scores with high well-being index scores.  

### Data Limitations:
- Dataset was inclusive of ~ 35 of 50 states; data for the remaining ~ 15 states was found via google search terms around "count of public tennis courts [state name]".


### Data Sources:
https://data.world/mglobel/tennis-courts
https://www.census.gov/newsroom/press-kits/2018/pop-estimates-national-state.html
Gallup 2018 Data
Manually Gathered Public Tennis Court Data from Google

### Conclusions re: Tennis Court data:
- I was surprised to see high and low public court availability scores all along the well-being (x-axis) with no correation to well being at all!!
- I think that having a polling data specifically relating to well-being and sports (including tennis), would have resulted in a higher correlation between a well-being index and public tennis court location data than what we observed between the Gallup well-being index and public tennis court data. 

## Housing Costs & Weather?

Overall, our group concluded that housing costs and weather have some correlation with the happiness index. Specifically, the amount of annual precipitation has an inverse impact on the happiness index: the less it rains, the happier people are. The amount that people have to spend on housing per month is surprisingly positively correlated with happiness. This means that states where people have to spend more on housing per month tend to have higher levels of happiness. There is most likely some confounding factor that should be further researched in this relationship.

## Crime?
One can imagine that the greater the crimes, the more it decreases happiness. So therefore this was a very good factor to explore to see if there was any correlation between crime and happiness level. The dataset used is called state_crime.csv from the CORGIS dataset project (https://corgis-edu.github.io/corgis/csv/state_crime/). The dataset contains crimes like assault, burglary, larceny, motor thefts, murder, rape, and robbery for all 50 states from 1960-2019. However, the happiness dataset used was from 2018 so we had to subset the crime dataset to only include 2018 stats. Then we merged the happiness dataset with the crime dataset. We initially showed bar graphs to generally see the number of crimes that occur in each state for each crime listed. Then we graphed the scatterplots with the correlation for each crime. The correlations were generally weak althpugh murder, assault, and burglary had the highest correlation values among the 7 crimes included in the dataset. All data cleaning, bar graphs, and scatterplots/correlations are included in the crime_analysis_final.ipynb file.

To conclude, the correlations (with highst of -0.22) are too weak to conclude that crime and happiness are related.

## Family Structure?
We asked the question- Does family structure as it relates to being married or not married has any affect on a states well-being ranking? 
Given the sample size and data provided, there is not a coorelation between the well being index of a state and family structure as it realates to being married or not married.  My conclusion is based on comparing the census.gov data of married or not married gathered for 2018. My suspicion is that if the people being polled in the happiness ranking were asked their family structure and the data was recorded, we would be able to uncover some correlation. Without that information of who was polled there is no correlation. 


## # of Parks?

![parks_image1](Images/Parks_WellBeing_Scatterplot_LR.png)

![parks_image2](Images/Ranks_Scatterplot.png)


## Setbacks


