
[editor on GitHub](https://github.com/Iman1997/socialdatawebsite/edit/gh-pages/index.md)

## Introduction

## Consumption

In the plot below we see the average consumption of energy presented on a monthly, daily, and hourly basis.

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

For the average monthly energy consumption, we see that the individuals consume more energy in the colder months with Santa’s month (December to be clear) being the highest at 4033,07 MWh/h, and less in the warmer months when the national blueberry month (aka. July) is the lowest at 3016,42 MWh/h. While heat doesn't come only from energy production, this makes sense as we in Denmark experience winters lower than 0°C, and despite being vikings, we need a little more energy to warm us up, and vice versa for the warmer months where we need less. Furthermore, the sun sets earlier during the winter months so we would need more light which inevitably increases the energy consumption.

Now, looking at the daily average energy consumption, with the exception of Sunday, we seem to consume more during the beginning of the week and less at the end. A key assumption is that companies, who are major energy consumers, are usually not running during the weekend and there’s therefore a decrease during these days. 
For the hourly energy consumption, a sensible pattern is seen as we consume more energy during waking hours and less when we sleep (unless you have a [curious furry baby](https://www.youtube.com/watch?v=9p6X9sEwRT4)). Around 6-7 o'clock in the morning, when most individuals wake up to start their day, the energy consumption rises until around midnight when you sleep again. This aligns with working versus free hours where we consume more during work hours (8-18). 

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

The choropleth map shown above gives a geographical overview of the total power production per municipality and the green fraction of the power production per municipality respectively in 2020. If you are not initiated into the marvelous magical world of data visualization a choropleth map is a geographical map divided into e.i municipalities using intensity of color to correspond with an aggregate summary of a geographic characteristic within spatial enumeration units.

It is important to note that power production not within a specific municipality isn’t shown on the choropleth maps. In addition, some municipalities are strangely detached e.i. the small municipality of Frederiksberg within the municipality of Copenhagen is producing almost no power. Whilst small islands like Anholt are integrated as small colonies of a far away municipality (Anholt is part of Norddjurs in Jutland) with a relatively high power production from offshore wind farms.

Looking at the choropleth map mode of the total power production a few municipalities stick out. Firstly, Esbjerg municipality produces way more power than any other municipality. This makes sense as Esbjerg can boast of having Denmark's largest offshore wind farm (Horns Rev 1, 2 and 3) including some of the largest wind turbines in the world - beside the central power plant Esbjergværket which is not small either. Secondly, high population municipalities like Copenhagen, Aarhus, Odense and Aalborg are producing relatively low amounts of power with most of the power being produced by central and decentral power plants.

Now looking at the choropleth map mode showing the green fraction of the total power production it is seen that low population density municipalities have a high green fraction while the high population density and highly industrialized municipalities e.i. Copenhagen, Aarhus, Odense, Aalborg and Fredericia have nearly no green power production. Part of the explanation of the low fraction of green power production is that green power production e.i. wind turbines (onshore and offshore) and solar farms require space which in all the aforementioned municipalities is in shortage - so much that Copenhagen has been creating artificial islands and draining sea. Secondly, these municipalities (excl. Fredericia) are housing the majority of the central power plants - both for historical and practical (space) reasons.

## Production

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

On the chart(s) above, we see the average energy production once again on a monthly, daily, and hourly basis. The production of energy seems to follow the energy consumption on average, but we produce more than we consume which makes sense since we can’t use what we don’t have. Also in regards to electricity, it’s an issue to overproduce as it would be hard to manage the excess electricity as it would have to be exported. 
What’s interesting to look at on these charts are the differences between green energy production (consisting of off & on-shore wind power and solar power) and  “general” energy production (green energy plus production less than 100MW & production greater than or equal 100MW). For the monthly production, we see that the green energy production is higher during January and February in comparison to any other month. One could assume that this is the wind power that is more dominant, as the wind is more present during these colder months. The same for solar power where there is a rise during the sunny July. For daily and hourly green vs “general” production, we see that there’s a common tendency for green energy to fill around half of the total energy production. This might excite politicians as they had a goal stating that green energy should amount to at least 30% of the total energy consumption/production in 2020 [source](https://kefm.dk/media/6788/regeringens_energi_og_klimapolitiske_maal.pdf). 

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

The choropleth map seen above shows the consumption of power per municipality in 2020. Where a stronger red intensity denotes a higher power consumption. Here it is clearly seen that the major population centers of Denmark e.i. Copenhagen, Aarhus, Odense and Aalborg has the highest consumption. These municipalities are where most Danes live and perhaps even more important in the sense of power consumption work. 

Furthermore, it is seen that agricultural areas and low population municipalities also have a lower power consumption. It is likewise interesting to see that Roskilde municipality has a relative low power consumption compared to the population size of the municipality. This might be explained by the municipality of Roskilde having a lower day population (workplace municipality) than night population (municipality of residence) while municipalities like Copenhagen is the opposite with a [large margin](https://www.statistikbanken.dk/PEND101). If one were to take a look at a [choropleth map showing the day population of the municipalities](https://www.statistikbanken.dk/statbank5a/Graphics/MapAnalyser.asp?maintable=PEND101&lang=0&dataclasses=linear(3230,60605)&BRANCHE07=TOT&PENDLING=DAG&K%C3%98N=M) on would see almost same patterns as the map above.

Finally, the size of a municipality e.i. Samsø or Læsø, as well as the strangely detached enclave Frederiksberg - which is relatively small while consisting mostly of housing, is also worth mentioning.

## Price

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

On the pricing visualizations, the price of consuming energy in the month, day, and hour is seen. It’s seen that September especially has a high price at 290,404 DKK. This could be connected with supply and demand. It was seen that there is a relatively low energy production in September at 3653,13 MW/h and compared to the other months, the difference between the energy production and consumption is very little, so this might have an effect on the overall price. 

For the days of the week, we see that there is a tendency in terms of pricing to be lower during the weekend and higher during the week. This is the same tendency seen in consumption and production, and as mentioned it might have something to do with people being at work in a company, and inevitably, companies consume more energy than a household. 

Talking about households, chores can be annoying during the day, so sometimes we do them while we sleep instead, and why not take advantage of the lower prices. During midnight and 5 in the morning, we see that the prices are between 120.933 DKK - 148.092 DKK. Another household chore is cooking dinner which apparently happens for many around 18 or 19 o'clock, so here the price is also higher. 
Furthermore, around 15 o'clock, we see that there’s a suspicious dip in pricing. When looking at the energy production and consumption from earlier, there’s a relatively high difference in energy production versus the amount of consumption, as there’s more than 1000MW produced than consumed. In order to balance things out, as the exporting of energy is expensive, one might think that the prices are lowered which encourages higher consumption.
This also shows that price might be more dependent on consumption rather than production.

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

We draw a scatter plot between production, consumption, and price. Calculate the Pearson correlation coefficient and corresponding P-value. A linear regression analysis was performed and the regression line was drawn on the graph.
Since energy production is demand-based, and energy imports and exports usually account for a small portion, The conclusion of the first graph can be easily understood: a very strong positive correlation between energy production and consumption, with a regression line slope almost equal to 1.
The relationship between price and production(consumption) is an interesting conclusion: the more energy is produced (or consumed), the higher the price tends to be. This conclusion is drawn because we found that the slopes of the two regression lines are positive, and the P-values obtained by calculating the Pearson correlation coefficients are 6.9E-284 and 5.9E-310, which are far less than 0.05, which means that the price and production (consumption) was significantly correlated.

We explore the relationship between energy production, consumption and price through scatter plots, regression lines and correlation coefficients: production and consumption are strongly correlated, and the slope of the regression line is close to 1. There is also a significant positive correlation between price and the first two: the more energy is produced and consumed, the higher the price of energy is.

## Prediction

Now comes the part of prediction. First, we divide all hours into two categories according to the price of energy and the proportion of green energy: the time that is suitable for purchasing energy, which is a “good” time, and the time that is not suitable for purchasing energy, which is a “bad” time. Here, we define an hour when the price is less than 300 DKK per MWh and the proportion of green energy is greater than 60% as “good”, and vice versa.
 
The data in 2020 is randomly divided into a training set and a testing set according to the ratio of 7:3. We hope to judge whether it is suitable to buy energy only using the information of time. According to the bar plots, we extract three characteristics from each specific time: month of the year, day of the week and hour of the day.
 
With these three features as independent variables and “good”/”bad” as dependent variables, the decision tree is constructed as follows.

<p align="center">
<iframe src="\socialdatawebsite\tree.html"
    sandbox="allow-same-origin allow-scripts"
    width="1400px"
    height="1440px"
    scrolling="yes"
    seamless="seamless"
    frameborder="0">
</iframe>
</p>

Following table compares the performance metrixs of the decision tree and that of the baseline. The decision tree presents a significant performance boost in accuracy, precision and recall.

|             | Baseline    | Decision Tree |
| ----------- | ----------- | ------------- |
| Accuracy    | 0.52        | 0.66          |
| Precision   | 0.59        | 0.67          |
| Recall      | 0.54        | 0.73          |

A confusion matrix can show the performance more intuitively. In the decision tree, “good” time is marked as positive and “bad” time are marked as negative. Compared with the false-positive rate and false-negative rate, the true-positive rate and true-negative rate have larger values, which means the decision tree has a better performance. In addition, the decision tree performed better on samples that are actually positive than on samples that are actually negative.

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

Plotting the feature importance, we can draw the conclusion that the month of the year is the most important factor affecting the suitability of purchasing energy, followed by the day of the week. This reminds us that it is important to plan energy purchases on an annual basis.

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

Plot the ROC curve as follows. The orange solid line is the ROC curve, and the blue dotted line is the baseline line for comparison, which is the curve in the case of completely random judgment (false-positive rate equals to true-positive rate). There is a significant gap between the two curves, indicating that the improvement brought by our decision tree is obvious.
In practical problems, true-positive rate and false-negative rate are of different importance. If we want to grab as many good times as possible to buy energy, we want the true-positive rate to be larger, i.e. more towards the upper-right corner of the image. If we care about not buying energy at bad times as much as possible, then we want the false-negative rate to be smaller, i.e. more towards the lower-left corner of the image.

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

Following is the Precision-Recall curve. In the decision tree, different thresholds can be selected, and each selection leads to different precision and recall.  The precision and recall corresponding to each specific threshold are marked as a point in the image, and the Precision-Recall curve connects these points together. The overall curve is down, but there are also partial upswings.
In practical, if we want to find a balance point, i.e. Precision = Recall, then precision and recall are both around 0.7, which is a relatively good performance in the general sense.

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

Three factors are extracted from the time data, and a decision tree is constructed to judge whether an hour is a good time to buy energy. Compared with the baseline, the improvement brought by our decision tree is obvious, and its performance on positive samples is better than that on negative samples. According to feature importance, planning energy purchase in the dimension of year is important. If it is clear what we care about in the actual problems, then the ROC curve and Precision-Recall curve can provide more reference for decision-making, especially the selection of thresholds.

## Conclusion
