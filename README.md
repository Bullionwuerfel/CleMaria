Mental Health DA by Clemens and Maria 



https://en.wikipedia.org/wiki/List_of_countries_by_alcohol_consumption_per_capita

https://www.theglobaleconomy.com/rankings/happiness/

We chose the mental health dataset mainly for secondary reasons, 
clean data and it seemed easier to combine with scraping sources 
Original dataset with 300.000 rows and 17 columns has datapoints of interest: 
Therapy care recieved, family history of mental helat care, mood swings etc

Scraped two websources containing tables of average alcohol consumption per 
country and happiness index per country to enrich our dataset and test additional 
hypotheses

We dropped some missing values and grouped certain data by country, calculated 
percentages based on the nationality of the single data rows(survey respondents)

No significant data cleaning challenges encountered 
(due to limited number of missing values  etc.) 

Practiced pivot tables, groupby functions, .map and other DataFrame methods
Looking trough available data, Wikipedia and theglobaleconomy sources, we formulated 
initial hypothyses about what data patterns we would expect to see in the analysis. 

Initial Hypotheses:
Expected higher treatment percentages in western countries
Treatment percentage and happiness index
Treatment percentage and alcohol consumption 
Average amount of days per year spent indoors and happiness index
Family history and likelyhood of receiving treatment
Connections between alcohol consumption and happiness index 

Major Obstacles:
After aggregating and analysing the data we saw some concerning patterns emerge. 
A lot of the data seemed unreasonable and unlikely to be real/realiable
When we found out, we tried to look up how this could have happened but 
there was no information given on how the author even came up with the data
Learned for the future: choose dataset more carefully and with patience - 
check sources etc. 

Conclusions:

Graph shows an overview of the percentage of individuals in the dataset by country 
which receive psychotherapy  - half of the countries in the dataset had values of 
zero (filtered out in this graph), which is extremely unlikely given the high number 
of rows in the dataset. And there are also 4 countries where all of the multiple hundred 
or thousand respondents in the dataset receiving therapy and little variation in between. 
This indicates that the dataset was most likely artificially constructed. 

Our initial hypothesis that Western countries have higher treatment percentages in 
comparison to non-western countries cannot be confirmed due to the poor data quality. 
But solely from the graph it is visible that Western countries tend to have high treatment 
rates. 


2nd graph is a scatterplot of the relationship between the happiness index per country and 
the percentage of individuals receiving therapy per country. A slight correlation between a 
higher happiness index of a country and a higher treatment rate is visible. However, so many 
countries having a zero treatment rate is highly unrealistic and we can again assume that the 
data set was artifically constructed. 

3rd graph is a scatterplot of the relationship between the average alcohol 
consumption per country and the percentage of individuals receiving therapy 
per country. A slight correlation between higher alcohol consumption of a 
country and a higher treatment rate is visible. However, the zero treatment 
rate countries are again an indication for the artificial dataset. 

We tried showing a relationship between the average days spent idoors per year 
and the Happiness Index of a country, but as this plot shows us, there is something 
wrong with the data. Every country seems to have approx the same value on the 
avarage days spent indoors scale, which points to a synthetic dataset, and a 
sloppiily done one at that.

Lastly, we put each datapoint into four groups using a stacked bar chart:

group one: people who have received treatment and have a family history of mental 
health issues(bottom right)

group two: no treatment and a family history(top right)

group three: No family history and treatment( bottom left)

group four: no family history and no treatment.

it looks on first review like there is a connection between the fact that a  
family member with mental health history seems to increase your chances of 
undergoing psychotherapy yourself, but the fact that other data were 
faked can only let us discard any and all insights into the data

Garbage in Garbage out!

None of our insights are well founded. Even if the data on family 
history affecting likelyhood of treatment seams plausible, the other 
analyses and the lack of sources show that it is not a reliable dataset