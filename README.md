# 10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-

**INTERACTIVE DATA VISUALIZATION ON GLOBAL TERRORISM USING PYTHON AND BOKEH**

**ASSIGNMENT -2

MODULE: DATA VISUALIZATION

MSc Data Analytics

DUBLIN BUSINESS SCHOOL

**AUTHORS / TEAM MEMBERS / Student Names: ** ------------------------------------------------------------------------------------------

Swapnil Chaudhari -10505342

Ashish Bharadwaj -10396445

Rakesh Pattanad - 10390582

------------------------------------------------------------------------------------------------------------------------------------
**TOOLS FOR VISUALIZATION: PYTHON , JUPYTER , ANACONDA**

**LIBRARIES : PANDAS, NUMPY, MATPLOTLIB , BOKEH (FOR INTERACTIVE VISUALIZATIONS) , FOLIUM **

 
Everyday,  world has faced several terrorism activities and threats jeopardizing peace of the socity in different nooks. Hence, with the 
Global Terrorism dataset which contains rich information regarding attacks and targetd cities along with their geospatial cordinates, attack time, 
we can visualize and see the surprising insights. The richness of the dataset has convinced us to achieve fruitful visualizations.

**Contribution:**
Each team member has contributes and fulfild the following tasks.

SWAPNIL CHAUDHARI (10505342) ----------------------------------------------------------------------------------------------------

1.Environment set setup (installation of packages / libraries) 

2.Data Preprocessing (Data cleaning ,shaping ,Working with pandas, numpy)

3.Interactive Choropleth Map to show casualties indifferent countries (Working with shapefiel, geopandas)

4.Interactive map with all targeted lpcations across the globe (Working with shapefiel, geopandas) 

5.Top 100 most terror targeted city/locations across the globe. ( Folium Map)  

6.interactive line plot visualization (Attack Counts and casualties by year)

7.Wordcloud visualization on Motive behind Terror attacks

ASHISH BHARADWAJ.(10396445)--------------------------------------------------------------------------------------------------------

1.DATA FINDING, DATA UNDERSTANDING

2.Attack Counts By Regions (Line Plot)

3.ATTACK TYpe and Counts

RAKESH PATTANAD (10390582)---------------------------------------------------------------------------------------------------------

1.Determining initial questions for analysis

2.Death , Casualties and wounded By Regions

3.Top 20 terror groups by attack counts


**Dataset: Global Terrorism Database **------------------------------------------------------------------------------------------------

More than 180,000 terrorist attacks worldwide, 1970-2017

The Global Terrorism Database (GTD) is an open-source database including information on terrorist attacks around the world from 1970 through 2017. The GTD includes systematic data on domestic as well as international terrorist incidents that have occurred during this time period and now includes more than 180,000 attacks. The database is maintained by researchers at the National Consortium for the Study of Terrorism and Responses to Terrorism (START), headquartered at the University of Maryland.

This dataset contains 100 variables on location, tactics, perpetrators, targets, and outcomes
 records of 180,000 records . Data can be found on https://www.kaggle.com/START-UMD/gtd


**Initial Analysis Questions **:------------------------------------------------------------------------------------------------------

1.	How many distinct regions exist in the dataset? What are the regions containing the highest and the lowest casualties?.Compare casualties, death toll and counts wounded in each region.

2.	Compare the terror attack trend in each regions.

3.	Use the geographic information from the dataset to create a map. And visualize the top countries affected by the terror attacks. Identify the top 5 countries with the highest casualties . And also mention countries with the least casualties and terror attacks?

4.	Highlite the top 100 terror targeted cities on map. 

5.	Which are the 5 years with the highest terror attacks? What are the total casualties in the same years?

6.	What are the top 20 active terror groups ?

7.	Discuss the counts of terror attack by its type.

8.	What kinds of weapons are used in terror attacks?

9.	What is the most common motive behind the terror attacks?

-------------------------------------------------------------------------------------------------------------------------------
**1.	How many distinct regions exist in the dataset? What are the regions containing the highest and the lowest casualties?.Compare casualties, death toll and counts wounded in each region.**

![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/death_wounded_casualties_by_Region.png)

From the graph it is clear that in Middle East and North Africa counts of death ,wounded and casualties all are the highest.
That is almost 14000,  200,000 and more than 300000 respectively. Middle East and North Africa is followed by South Asia and
Sub-Sahran Africa.  Interestingly, Central Asia , East Asia and Australia & Oceania have almost 0 or below 100 casualties. In other words,
seems like nations in these regions like Australia and Israel have the most active counter-terror units to protect their citizens.  

**2.	Compare the terror attack trend in each regions.**

![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/Attack%20Counts%20By%20Region.png)

From , above graph , it is clear that terror activities East Asia, Central Asia, Australia & Ocenia remain almost negligible 
throughout the time period (1970 – 2017). In remaining regions, it remained at average 0f 50 from 1970 to 2000. However, sudden
hike is observed in the duration of 2000 to 2017.  What should be the reason behind it? Especially, in Middle East - North Africa and South Asia terror activities have drastically increased.

**3.	Use the geographic information from the dataset to create a map. **
**And visualize the top countries affected by the terror attacks. Identify the top 5 countries with the highest casualties .**
And also mention countries with the least casualties and terror attacks?**
![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/worldwide_attack_map.png)

The interactive choropleth map above shows the worldwide casualties. Each country is colored according to the shade the casualties 
counts in terror attacks. The color palette below shows the  casualties with respect to color. As we can see Iraq holds the rightmost
color of the palette , hence with the highest casualties (213279 casualties ).  That is followed by afghanisthan(>85000), 
Pakistan (>65000)and India(>48000). These countries have the highest casualties in terror attacks in the history. Countries with blue
colors like Australia (136 only), Brazil (363),Jordan(393), Canada(511) have the lowest casualties in terror attacks.


Adding coordinates of all targeted locations
![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/worldwide_casualties_targed_location.png)

Pinch in to see the country name with country with highest casualties which has the right most color in the colorbar below.
![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/world_wide_targets_zoom.JPG)

**4.	Highlite the top 100 terror targeted cities on map.** 
**Bubbles show popup city name when clicked.**
![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/top%20targeted%20100%20cities%20map.JPG)

**5.	What are the top 20 active terror groups ?**

![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/Terror%20groupattacks.JPG)

According to data Taliban (Afghanistan) is the most active group in the world with 7478 attacks till 2017. 
It is followed by ISIL(middle east, 5613 attacks) at second rank. Shining path (4555 attacks) at 3rd rank, FMLN(3351 attacks)  4th, 
Al Shabab (3288 attacks) 5th then NPA(2772 attacks) and Irish Republican Army-2671 attacks (active in Ireland, Europe) at 6th Rank.

![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/Top%2020%20Terrorist%20Groups%20by%20attaks%20.png)


**6.	Discuss the counts of terror attack by its type.**

![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/count%20attack%20types.JPG)

The most prevalent type of attacks in all attacks are bombing/ explosion. 
According to data, so far more than 88 thousand bomb attacks are observed. Armed assault stands at 2nd rank with 42669 records. Assassination carried out by terror groups counts for 19312 records. Hostage taking,  Facility attack , unnamed assult, 
hostage taking (barricade) , hijacking are other kind of terror styles. However, attacks types of 7276 records are still unknown.
![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/Attack%20Type%20and%20counts%20.png)


**7.	Which are the 5 years with the highest terror attacks? What are the total casualties in the same years?**
![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/attack%20counts%20and%20casualties%20by%20%20year%20zoom%20and%20box%20selet.JPG)
The line graph articulates the attack counts by year and scatter plot represents the casualties by year.
We can observe the rise in terror activity with the time in 20th century. Attacks were highest in  2014(16903attacks and 
more than 68000 casualties). 2012, 2013,2014,2015,2016,2017 holds the highest terror attacks across the globe, This points are red colored in the graph.

**8.	What kinds of weapons are used in terror attacks?**
We can observe the dominance of explosives in terror attacks from above graph.  
In other words it is very disappointing to say that most of the lives lost or damages , harm is done by means of explosives.
It holds 24,713 records,  Firearms stand at the second rank with 14077 records and Incendiary at third with 3520 records. 
Other weapons like chemical , biological detrimental weapons are less used (<150 records).
![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/Counts%20Weapons%20in%20Attacks.png)

**9.	What is the most common motive behind the terror attacks?**
Using the word cloud visualization on the textual data we can detect most frequent words. As we can see violence is the the largest word. It means violence is the most frequent word in motive column of the dataset. Hence, violence is the most common motive behind all terror activities. 
Other motives behind terror attacks includes “Sunni”,”united states”,”Islamic states” .These are the most common motive as per the dataset.
![](https://github.com/SwapnilChaudhari/10505342.github.io-A2-Interactive-Data-Visualization-on-Global-Terrorism-Python-/blob/master/code/visualization%20outputs/wordclouds.png)












