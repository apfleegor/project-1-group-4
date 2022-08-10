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
* data.world https://data.world/mglobel/tennis-courts
* census.gov https://www.census.gov/newsroom/press-kits/2018/pop-estimates-national-state.html


# Data Cleaning and Exploration 

## Tennis Anyone? 
### Inspiration:
So when we considered evaluating data against a Well being index, of course I thought of one of the most enjoyable sports in the modern era: Tennis.

It is an incredibly dynamic and enjoyable activity that requires athleticism and strategy.  Skillful players process an inconceivable number of decisions and adjustments in an instant than could be believed.

### Tennis well-being attributes:
        - Physically challenging
        - Mentally engaging
        - Can be played competitively or recreationally
        - Is great exercise because  it is so fun, you don't even know you're exercising
        - Builds Character and discipline
        - Is social and a great way to make new friends
        - Is economical and can be played almost anywere
        - Has a positive carryover effect on nearly all other aspects of your life

### Hypothesis:
Developed a working hypothesis once sources found: Because of all of it's positive well-being attributes, tennis has to have a strong positive relationship with the Well-Being Index as captured by Gallup.  Doesn't it??? 

I set out to prove this by looking at data on public tennis court locations as a proxy for the availability and participation of tennis across 50 states.

### Data Discovery:
- 29,000 + locations found in the data
- Max Raw (California): 12,800+ locations
- Min Raw (Delaware): 356

### Data Limitations:
- Dataset was inclusive of ~ 35 of 50 states; data for the remaining ~ 15 states was found via google search terms around "count of public tennis courts [state name]".
- Set included only sites for major metropolitan areas.

### Data Sources:
https://data.world/mglobel/tennis-courts
https://www.census.gov/newsroom/press-kits/2018/pop-estimates-national-state.html

### Conclusions re: Tennis Court data:
My conclusions were that there was almost no correlation between the by state availability of publicly available tennis courts and gallup's well being index... And that the next survey ought to include individuals walking off of tennis courts.
## Housing Costs & Weather?

Overall, our group concluded that housing costs and weather have some correlation with the happiness index. Specifically, the amount of annual precipitation has an inverse impact on the happiness index: the less it rains, the happier people are. The amount that people have to spend on housing per month is surprisingly positively correlated with happiness. This means that states where people have to spend more on housing per month tend to have higher levels of happiness. There is most likely some confounding factor that should be further researched in this relationship.

## Crime?
One can imagine that the greater the crimes, the more it decreases happiness. So therefore this was a very good factor to explore to see if there was any correlation between crime and happiness level. The dataset used is called state_crime.csv from the CORGIS dataset project (https://corgis-edu.github.io/corgis/csv/state_crime/). The dataset contains crimes like assault, burglary, larceny, motor thefts, murder, rape, and robbery for all 50 states from 1960-2019. However, the happiness dataset used was from 2018 so we had to subset the crime dataset to only include 2018 stats. Then we merged the happiness dataset with the crime dataset. We initially showed bar graphs to generally see the number of crimes that occur in each state for each crime listed. Then we graphed the scatterplots with the correlation for each crime. The correlations were generally weak althpugh murder, assault, and burglary had the highest correlation values among the 7 crimes included in the dataset. All data cleaning, bar graphs, and scatterplots/correlations are included in the crime_analysis_final.ipynb file.

To conclude, the correlations (with highst of -0.22) are too weak to conclude that crime and happiness are related.

## Family Structure?
I asked the question- Does family structure as it relates to being married or not married has any affect on a states well-being ranking?  


## # of Parks?

![parks_image1](Images/Parks_WellBeing_Scatterplot_LR.png)

![parks_image2](Images/Ranks_Scatterplot.png)


## Setbacks


