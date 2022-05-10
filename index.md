# Social Data Final Project

[Link for the Explainer Notebook repository](https://github.com/vonScholten/social-data-project.git)
[Link for the data files](https://github.com/vonScholten/social-data-project/tree/main/data)

## Introduction

The seventh UN goal is “Affordable and Clean Energy”, and aims to [ensure access to affordable, reliable, sustainable, and modern energy for all](https://sdgs.un.org/goals/goal7). But with the increasing high power consumption and pricing affected by the ever-changing climate how could such a goal be accomplished?

This project seeks to analyze power consumption, production, and pricing with the goal of predicting the best time to consume power in terms of the cheapest sustainably (green) produced power. This is not only interesting for making the transition from non-green power more affordable and thus combating climate change by incentivizing consuming power when more green power is available but also to the current geopolitical situation with rising prices on energy across the board. In other words, this project seeks to bridge environmental sustainability with socio-economic sustainability.

This project is a collaboration between three MSc. students as a part of the Social Data Visualizations course of Spring 2022 at DTU. 

## Consumption

In the bar charts below, we see the average consumption of power presented on a monthly, daily, and hourly basis.

<p align="center">
<iframe src="\socialdatawebsite\consumption_bar.html"
    sandbox="allow-same-origin allow-scripts"
    width="700px"
    height="700px"    
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

For the average monthly power consumption, we see that the individuals consume more power in the colder months with Santa’s month (December to be clear) being the highest at 4033.07 MWh/h, and less in the warmer months when the national blueberry month (aka. July) is the lowest at 3016.42 MWh/h. While heat doesn't come only from power production, this makes sense as we in Denmark experience winters lower than 0°C, and despite being vikings, we need a little more power to warm us up, and vice versa for the warmer months where we need less. Furthermore, the sun sets earlier during the winter months so we would need more light which inevitably increases the power consumption.

Now, looking at the daily average power consumption, we generally seem to consume more during the beginning of the week and less at the end. A key assumption is that companies, who are major power consumers, are usually not running during the weekend, thus a decrease during these days is seen. 
For hourly power consumption, a sensible pattern is seen as we consume more power during day hours and less when we sleep (unless you have [a curious furry baby](https://www.youtube.com/watch?v=9p6X9sEwRT4)). Around 6-7 o'clock in the morning, when most individuals wake up to start their day, the power consumption rises until around midnight when they sleep again. This aligns with working versus free hours where we consume more during work hours (8-18 o'clock).  

The choropleth map seen below shows the consumption of power per municipality in 2020.

<p align="center"> 
<iframe src="\socialdatawebsite\consumption_map.html"
    sandbox="allow-same-origin allow-scripts"
    width="1000px"
    height="800px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

It is seen that a stronger red intensity denotes a higher power consumption. Here, it is clearly seen that the major population cities of Denmark i.e. Copenhagen, Aarhus, Odense, and Aalborg have the highest consumption. These municipalities are where most Danes live, and perhaps even more important in the sense of power consumption, where they work. 

Furthermore, it is seen that agricultural areas and low population municipalities also have lower power consumption. It is likewise interesting to see that the Roskilde municipality has a relatively low power consumption compared to the population size of the municipality. This might be explained by the municipality of Roskilde having a lower day population (workplace municipality) than the night population (municipality of residence) while municipalities like Copenhagen are the opposite with a [large margin](https://www.statistikbanken.dk/PEND101). If one were to take a look at a choropleth map showing the [day population of the municipalities](https://www.statistikbanken.dk/statbank5a/Graphics/MapAnalyser.asp?maintable=PEND101&lang=0&dataclasses=linear(3230,60605)&BRANCHE07=TOT&PENDLING=DAG&K%C3%98N=M) one would see almost the same patterns as the map we have created above.

Finally, the size of a municipality i.e. Samsø or Læsø, as well as the strangely detached enclave of Frederiksberg, which is relatively small while consisting mostly of housing, is also worth mentioning, as they naturally have a low power consumption. While at the first glance the island of Anholt (the small island in the middle of Kattegat) seems to contribute to rather large power consumption. However, a second glance reveals that Anholt is part of the much larger Jutlandic municipality Norddjurs.


## Production

On the bar charts below, we see the average power production once again on a monthly, daily, and hourly basis.

<p align="center"> 
<iframe src="\socialdatawebsite\production_bar.html"
    sandbox="allow-same-origin allow-scripts"
    width="700px"
    height="700px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

The production of power seems to follow the power consumption on average, but we produce more than we consume which makes sense since we can’t use what we don’t have. Also in regards to electricity, it’s an issue to overproduce as it is hard to manage the excess electricity as it would have to be exported. 
What’s interesting to look at on these charts are the differences between green power production (consisting of off & on-shore wind power and solar power) and  “general” power production (green power plus production less than 100MW & production greater than or equal to 100MW). For the monthly production, we see that the green power production is higher during January and February in comparison to any other month. One could assume that this is the wind power that is more dominant, as the wind is more present during these colder months. The same for solar power where there is a rise during the sunny month of July. For daily and hourly green vs “general” production, we see that there’s a common tendency for green power to fill around half of the total energy production. This might excite politicians as they had a goal stating that [green energy should amount to at least 30% of the total energy consumption/production in 2020](https://kefm.dk/media/6788/regeringens_energi_og_klimapolitiske_maal.pdf).  

The choropleth map shown below gives a geographical overview of the total power (electricity) production per municipality and the green fraction of the power production per municipality respectively in 2020. 

<p align="center"> 
<iframe src="\socialdatawebsite\production_map.html"
    sandbox="allow-same-origin allow-scripts"
    width="1000px"
    height="800px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

If you are not initiated into the marvelous magical world of data visualization, a choropleth map is a geographical map divided into i.e. municipalities using the intensity of color to correspond with an aggregate summary of a geographic characteristic within spatial enumeration units. You can interact with the layers so feel free to play around with them.

It is important to note that power production outside a specific municipality isn’t shown on the choropleth maps. In addition, some municipalities are strangely detached e.i. the small municipality of Frederiksberg within the municipality of Copenhagen is producing almost no power. Whilst small islands like Anholt are integrated as small colonies of a far away municipality (Anholt is part of Norddjurs in Jutland) with relatively high power production from offshore wind farms.

Looking at the choropleth map layer of the total power production a few municipalities stick out. Firstly, the Esbjerg municipality produces way more power than any other municipality. This makes sense as Esbjerg can boast of having Denmark's largest offshore wind farm (Horns Rev 1, 2, and 3) including some of the largest wind turbines in the world - as well as having the central power plant Esbjergværket which is not small either. Secondly, high population municipalities like Copenhagen, Aarhus, Odense, and Aalborg are producing relatively low amounts of power with most of the power being produced by central and decentral power plants.

Now looking at the choropleth map layer showing the green fraction of the total power production, it is seen that low population density municipalities have a high green fraction while the high population density and highly industrialized municipalities i.e. Copenhagen, Aarhus, Odense, Aalborg, and Fredericia have nearly no green power production. Part of the explanation for the low fraction of green power production is that green power production i.e. wind turbines (onshore and offshore) and solar farms require space which is a shortage for all the aforementioned municipalities - so much so, that Copenhagen has been creating artificial islands and draining the sea to get more space. Secondly, these municipalities (excl. Fredericia) are housing the majority of the central power plants - both for historical and practical (space) reasons.


## Price

On the pricing visualizations below, the price of consuming power during the month, day, and hour is seen.

<p align="center">
<iframe src="\socialdatawebsite\price_bar.html"
    sandbox="allow-same-origin allow-scripts"
    width="700px"
    height="700px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

It’s seen that September especially has a high price at 290.404 DKK. This could be connected with supply and demand. It was seen that there is a relatively low power production in September at 3653.13 MW/h, on the production bar chart above, and compared to the other months, the difference between the power production and consumption is very little, so this might have an effect on the overall price of power consumption.

For the days of the week, we see that there is a tendency in terms of pricing to be lower during the weekend and higher during the workweek. This is the same tendency seen in the consumption and production bar charts above, and as mentioned it might have something to do with people being at work in a company, and inevitably, companies consume more power than a standard household. 

Talking about households, chores can be annoying during the day, so sometimes we do them while we sleep instead, and why not take advantage of the lower prices. During midnight and 5 o'clock in the morning, we see that the prices are ranging between 120.933 DKK to 148.092 DKK. Another household chore is cooking dinner which apparently happens for many around 18 or 19 o'clock, so here the price is higher. 
Furthermore, around 15 o'clock, we see that there’s a suspicious dip in pricing. When looking at the power production and consumption from earlier, there’s a relatively high difference in energy production versus the amount of consumption, as there’s more than 1000MW produced than consumed. In order to balance things out, as the exporting of energy is expensive, one might think that the prices are lowered which encourages higher consumption once again triggered by supply and demand.
This also shows that price might be more dependent on consumption rather than production.

To dive into the relationships of the aforementioned variables, we have created a scatter plot that shows the correlations between power production, consumption, and price, including a regression line, which can be seen below. 

<p align="left">
<iframe src="\socialdatawebsite\cor1.html"
    sandbox="allow-same-origin allow-scripts"
    width="450px"
    height="300px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

<p align="center">
<iframe src="\socialdatawebsite\cor2.html"
    sandbox="allow-same-origin allow-scripts"
    width="450px"
    height="300px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

<p align="right">
<iframe src="\socialdatawebsite\cor3.html"
    sandbox="allow-same-origin allow-scripts"
    width="450px"
    height="300px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

In the plots, we see a very strong positive correlation between power production and consumption, with a regression line slope almost equal to 1. There is also a significant positive correlation between power price and production. From the relationship between the two, an interesting conclusion can be drawn: the more power is produced or consumed, the higher the price tends to be. This conclusion is drawn because we found that the slopes of the two regression lines are positive, and the P-values obtained by calculating the Pearson correlation coefficients are 6.9E-284 and 5.9E-310, which are far less than 0.05, which means that the price and consumption were significantly correlated.

## Prediction

In order to get started with the prediction, we divide all hours into two categories according to the price of power and the proportion of green power: the time that is suitable for purchasing energy, which is a “good” time, and the time that is not suitable for purchasing energy, which is a “bad” time. Here, we define an hour when the price is less than 300 DKK per MWh and the proportion of green energy is greater than 60% as “good”, and vice versa.

The data in 2020 is randomly divided into a training set and a testing set according to the ratio of 7:3. We hope to judge whether it is suitable to buy energy only using the information of time. According to the bar plots, we extract three characteristics from each specific time: month of the year, day of the week and hour of the day.
 
With these three features as independent variables and “good”/”bad” as dependent variables, the decision tree is constructed as follows.

<p align="center">
<iframe src="\socialdatawebsite\tree.html"
    sandbox="allow-same-origin allow-scripts"
    width="1000px"
    height="800px"
    scrolling="yes"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

The following table compares the performance metrics of the decision tree and that of the baseline. The decision tree presents a significant performance boost in accuracy, precision and recall.

|             | Baseline    | Decision Tree |
| ----------- | ----------- | ------------- |
| Accuracy    | 0.52        | 0.66          |
| Precision   | 0.59        | 0.67          |
| Recall      | 0.54        | 0.73          |

The confusion matrix below shows the performance more intuitively. In the decision tree, “good” time is marked as positive and “bad” time are marked as negative. Compared with the false-positive rate and false-negative rate, the true-positive rate and true-negative rate have larger values, which means the decision tree has a better performance. In addition, the decision tree performed better on samples that are actually positive than on samples that are actually negative.

<p align="center">
<iframe src="\socialdatawebsite\metrix.html"
    sandbox="allow-same-origin allow-scripts"
    width="450px"
    height="300px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

From plotting the feature importance as seen below, we can draw the conclusion that the month of the year is the most important factor affecting the suitability of purchasing energy, followed by the day of the week. This reminds us that it is important to plan power purchases on an annual basis.

<p align="center">
<iframe src="\socialdatawebsite\importance.html"
    sandbox="allow-same-origin allow-scripts"
    width="450px"
    height="300px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

We then plot the ROC curve as follows.

<p align="center">
<iframe src="\socialdatawebsite\ROC.html"
    sandbox="allow-same-origin allow-scripts"
    width="450px"
    height="300px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

The orange solid line is the ROC curve, and the blue dotted line is the baseline for comparison, which is the curve in the case of completely random judgment (false-positive rate equals to true-positive rate). There is a significant gap between the two curves, indicating that the improvement brought by our decision tree is obvious.
In practical problems, true-positive rate and false-negative rate are of different importance. If we want to grab as many good times as possible to buy power, we want the true-positive rate to be larger, i.e. more towards the upper-right corner of the plot. If we care about not buying power at bad times as much as possible, then we want the false-negative rate to be smaller, i.e. more towards the lower-left corner of the plot.

Following is the Precision-Recall curve. 

<p align="center">
<iframe src="\socialdatawebsite\PR.html"
    sandbox="allow-same-origin allow-scripts"
    width="450px"
    height="300px"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

In the decision tree, different thresholds can be selected, and each selection leads to different precision and recall. The precision and recall corresponding to each specific threshold are marked as a point in the image, and the Precision-Recall curve connects these points together. The overall curve is down, but there are also partial upswings. In practice, if we want to find a balance point, i.e. Precision = Recall, then precision and recall are both around 0.7, which is a relatively good performance in general sense.

Three factors are extracted from the time data, and a decision tree is constructed to judge whether an hour is a good time to buy power. Compared with the baseline, the improvement brought by our decision tree is obvious, and its performance on positive samples is better than that on negative samples. According to feature importance, planning power purchases in the dimension of year is important. If it is clear what we care about in the actual problems, then the ROC curve and Precision-Recall curve can provide more reference for decision-making, especially the selection of thresholds.

## Conclusion
  
The project which sought to analyze power consumption, production, and pricing with the goal of predicting the best time to consume power in terms of the cheapest sustainably (green) produced power has concluded with a more or less successful output. We see through our analysis, where we created different visualizations (interactive bar charts, choropleth maps, machine learning visuals), we can conclusively say that it is possible to predict the best time to consume power in terms of the cheapest sustainably (green) produced power by using a model based on power consumption, production, and pricing data. 
