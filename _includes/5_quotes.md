<br>

#### Finding the quotes within selected newspapers


Subsequently, we extracted all quotes cited in those newspapers from the subset of 100’000 quotations for each year. <br>

Secondly, to link a topic to a quote we looked if the quote contained one of the sub-topics. This resulted in a matrix where we could find the number of occurrence of each topic for the different newspapers. <br>

The distributions of the quotes over the topics were normalized by the total number of quotes by newspaper. From the heatmap below, one can observe that all newspapers are focused on mainstream topics such as "Sports" or "Teamwork". It can also be noted that the topic "Investing" has a higher chance to appear in one article of the newspaper **Financial Times** than in another one, this makes sense as the newspaper is specialized in this field.

<iframe src="assets/export/Distribution_topic_newspaper.html" height="600" width="100%" scrolling = no></iframe>
<br>
<br>
#### Measuring newspapers controversy

{% include im_side.html text= "assets/export/newpapers_multiplication.PNG"

content= " <br>
Finally, by multiplying the topic-newspapers matrix with the controversy score vector for each topic, we got the controversy score of each journal.

The process was applied for each year of the period individually, this resulted in the controversy score evolution of each newspaper over time. The resulting graphic is presented below." height="200" width="500" %}


<iframe src="assets/export/contro_news_year.html" height="550" width="1000" scrolling = no></iframe>


Looking at the sales table one can observe that they are decreasing over the years, however the controversy score seems to react in an opposite manner. Is it a reaction of the newspaper companies, which are willing to keep their numbers as high as possible and are willing to modify their usual topics to do so?  In 2020, all newspapers seem to have talked less on controversial subjects, one can explain this behaviour by the pandemic which was taking all the spotlight.

One newspaper clearly stands out from the others, FT which stands for **Financial Times**.  It is the most controversial newspaper and its controversy score is continuously increasing until it suddenly dropped in 2020. We, first, tried to explain this behaviour with the fact that the pandemic completely stopped the global economy in 2020. It generated a consensus regarding the financial market. However, as good ADAventurers that we are, we took a closer look at the data and quickly realized that for this year an abnormally small amount of quotations were selected in the dataset. This value was neglected for subsequent calculations.

<br>

On the graphics below you can see how newspapers sellings are related to their controversy score. On the left the results for all newspapers and on the right you can scroll through the graphics to have a better view of each newspaper separately.
