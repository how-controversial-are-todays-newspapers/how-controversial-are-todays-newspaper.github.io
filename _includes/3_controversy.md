<br>

#### Controversy score with sentiment analysis

For each selected topic we want to calculate a sentiment score to assess how controversial it is. A sentiment analysis can be done on all quotes linked to the sub-topics defined in the previous step. <br>

The sentiment analysis allows us to define if a quote is addressed in a positive or negative manner. We ended up with a repartition of positive and negative sentiments for a given word.<br>

From this distribution, we defined a controversy score as follows: a subject with an equal repartition of positive/negative sentiment should be interpreted as strongly controversial.<br>

The following formula was implemented to define the score: $$ 2 \cdot \frac{min(\#pos, \#neg)}{\#pos + \#neg}  $$.

As we can see from the figure below the theme “Politic” is more controversial (controversy_score = 0.98) whereas “Team” does not reflect a strong controversy (controversy_score = 0.54).

{% include frame.html text= "assets/export/politic_pos_neg.html" content= "assets/export/teamwork_pos_neg.html" %}




<br>

{% include side.html text="assets/export/Controversy_Trump_over_time.html"  content = " <br>
We took some time to analyse the term **Trump**, which obviously represents the well known former President of the United States, Donald J. Trump. <br>

Regarding all the drama around the character, the word **Trump** had to be a controversial topic! So we looked at how its controversy score evolved over time. <br>

The score is at its peak in the year 2015, when he was running for President and had the reputation of being a successful businessman with the tendency to speak very frankly on Twitter. <br>

But, after his election his status changed radically since he became one of the most powerful people in the world.<br>

In some way, his communication might have become wiser. However, the number of articles citing him increased and the controversy score of his name stayed around 80%!"
 width = "120%" height = "600" %}

<br>
<br>

#### Signature score

To assess the correctness of our controversy score, we have compared it to methods available from literature. In particular we compared it to a method based on the variance of sentiments from the paper "[Quantifying controversy in social media](https://dl.acm.org/doi/10.1145/2835776.2835792)".<br>

We also considered a method that compares sentiment distributions within quotations. Additionally, this “sentiment signature” based method aims at providing a relative controversy score to attempt to validate our model.<br>


<iframe src="assets/export/heatmap.html" height="500" width="100%" scrolling = no></iframe>

To validate or discard our model, we applied a principle of majority vote. Our expectation was that the two methods that “agreed” the most often should be more accurate and closer to the ground truth. In the figure above, we have the similarity scores of the three different methods we considered. Essentially, it can be seen from the cells colors how similar one method is to another for a given topic. Doing this pairwise comparison, we got that the mean similarity score (across all topics) is highest (i.e. 0.52) between our method and the sentiment signature based one. One can remark that this analysis provides us with arguments against the variance-based method. <br>

As a conclusion, we will rely on our method for the aforementioned reasons and also for the fact that it is simpler and provides an absolute measure of controversy.



<br>

#### Controversy score for each topic

Finally, after checking our model, it was time to evaluate the controversy score of the selected topics. <br>

The controversy scores was calculated by summing all the positives and negatives sentiments over all sub-topics. Here, it was done over a 5-year period, from 2015 to 2020, see graphic below.

<iframe src="assets/export/Controversy_of_topic_over_time.html" height="600" width="1000"></iframe>

First, it can be observed that our scores are consistent over the years and specific to each topic (they are not all packed together).  In addition, some topics, such as “Politics”, “Investing” or even “Countries", seem strongly controversial as they are usually perceived within popular opinion. <br>

In opposition to the terms like “Sports”, “Datetime” and “Games” do not seem to represent controversial subjects, as sport journalists are supposed to stay neutral in their report.
