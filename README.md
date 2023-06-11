# US Census Demographic Data Visualization

* [Link to Tableau story](https://public.tableau.com/views/US-Census-Demographic-Data-Viz/USCensusDataStory) - **includes three 
dashboards.**

## 1. Insight no. 1
   * **Link** - inside the story, the first dashboard in the story or see the image below (Viz 1).
   * **Summary** - In order to find the states that have the best transportation, we should consider either **Transit** or **Mean 
   Commute time** column in the dataset. We had to find out the highest percentage of transit use states or, lowest mean commute time 
   usage states. Therefore, we can see that one bar chart represents top 5 states with highest percentage of transit usage and another 
   bar chart shows top 5 states with lowest commute time usage. Additionally, we have added a tree map to see the total population of 
   those states. Certain research shows that both the columns have important impact in the transportation system. Instead of choosing one 
   upon another, we used both of them to analyse the best transportation states. Unfortunately, there is no correlation between these two 
   columns. Therefore, the combination set of states extracted from both columns would represent the best transportation states. To 
   aggregate the data from the county level to the state, we have done a set operations on state column based on top transit values and 
   bottom commute time values.
   * **Design** - We have created a dynamic dashboard that shows the **top transit usage states** and **bottom commute times usage 
   states** in terms of transportation. We have also added area chart which shows the total population for both the filtered states 
   (defined above). Initially, top or botttom 10 values are shown, but it can be changed dynamically by user.
   * **Resources** - **N/A**
   
![alt text](https://github.com/asifsamy/US-census-data-viz/blob/master/images/US%20Census%20Data%20Story1.png "Logo Title Text 1")
<p align="center"><strong>Viz 1: Story 1</strong></p>

## 2. Insight no. 2
   * **Link** - inside the story, the second dashboard in the story or see the image below (Viz 2).
   * **Summary** - Here we have two map charts where one is showing the states from top income and another is showing the states from 
   bottom poverty. A tooltip appears when you hover over a state with data about occupation rates, as well as a pie chart describing 
   the occupation composition. The composition includes percentage of employed, unemployed, self employed, family work, and others.
   We also used a pie chart to show the general occupation composition of the USA so that you could compare the composition of each 
   state with the entire nation. <br />
   Using the default of 10 in the "income" and "poverty" maps, we could see very clearly that the most states of both maps are located 
   in the southeast region of the USA. Both the maps have two distinct state of island (Hawaii from top income states and Puerto Rico
   from top poverty state). As expected that income states has higher employment rates (approx. 50%) and lower unemployment rates 
   (5% to 9%). On the other hand, poverty states has lower employment rates (35% to 40%) and higher unemployment rates (9% to 12%) 
   than income states. The poverty (Puerto Rico) has a severe unemployment rate that is around 19.37% but the the income island Hawaii 
   has only 5.20 % unemployment rate. 
   * **Design** - We have created a dynamic parameter to extract top n states from the column. Thus 2 sets has been created; top states 
   set for income and top states sets for poverty. We have also generated a calculated field to calculate the employment rate from 
   total population. <br />
   Using the map, we searched for clusters of states for income and poverty with similar properties in the same region, and indeed 
   there were. The pie chart has been chosen to illustrate the composition of overall oqqupations percentage for the entire USA.
   * **Resources** - [Land and Region of USA](https://slideplayer.com/slide/8989121/)

![alt text](https://github.com/asifsamy/US-census-data-viz/blob/master/images/US%20Census%20Data%20Story2.png "Logo Title Text 1")
<p align="center"><strong>Viz 2: Story 2</strong></p>
   
## Insight no. 3
   * **Link** - inside the story, the third dashboard in the story or see the image below (Viz 3).
   * **Summary** - Here we have two maps where one shows the top 10 highest income per capita holding states, another shows the bottom 
   10 lowest income per capita holding states with their ratio of ethnicities. Certainly, the top value or bottom value parameter is 
   dynamic. There is also a tree map to show the overall ethnicity rate for the entire USA. The primary goal is to explore the income 
   per capita for top and bottom US states and relate this with the ethnicity. <br />
   Geographically, most of the highest income per capita states showed in the map are situated in the coastal and northeast areas and 
   most of the lowest income per capita states in the map are situated in the southeast area of USA. <br />
   The top income per capita states are populated with vastly majority of white ethnic group and population of other ethnic groups are 
   very insignificant. However, there are two exceptionional states such as Hawaii that has a huge number of Asian people and Alaska 
   that has significant ratio of Native American. <br />
   On the other hand, some states of lowest income per capita (such as Alabama, Mississippi, Georgia, South Carolina, Maryland, etc) 
   have significant number of other ethnic group (Black).
   * **Design** - We have created a dynamic parameter to extract top n states of income per capita from the column. Thus 2 sets has 
   been created to filter top n states and bottom n states set for income per capita. <br />
   A tree map is generated to show the overall ethnicity ratios for entire USA. <br />
   Two maps are created in the same axis one for the top n income states and another for the bottom n income states. A worksheet is 
   creates to show the ethnicity as a pie chart for each state and that sheet is used as a tooltip later in the map sheet.
   * **Resources** - [Land and Region of USA](https://slideplayer.com/slide/8989121/)
   
   ![alt text](https://github.com/asifsamy/US-census-data-viz/blob/master/images/US%20Census%20Data%20Story3.png "Logo Title Text 1")
   <p align="center"><strong>Viz 3: Story 3</strong></p>
   
