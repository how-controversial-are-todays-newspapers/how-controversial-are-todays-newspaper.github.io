

The first step of our analysis is to extract relevant topics from the corpus. In fact, since we have to deal with Natural Language Processing (NLP), it is necessary to first preprocess the dataset. Therefore, the quotations need to be cleaned in order to get only their essence, i.e. words that represent the theme addressed by the speaker. <br>

{% include im_side.html text= "assets/export/coherence_score.jpeg"

content= "To carry this out, a Latent Dirichlet Allocation (LDA) model can be used either on the most frequent words through bag-of-words (BoW) model or on the most relevant words using the term frequency–inverse document frequency (TF-IDF) method. <br>

A coherence score can be computed for each list of words in order to quantify how good the two methods are compared to each other.
The LDA model then allows to separate the corpus into $$n$$ different topics. By running it with different values of $$n$$, as it is shown in the figure, we can see that there is an optimal number of topics.

This number can then be kept for further computations." height="300" width="500" %}



{% include im_side.html text= "assets/export/Chosen_topics_2.jpg"

content= "By fixing the number of topics, the LDA model can then be used to extract the most relevant terms for each topic. <br>

Next, a word which represents best each topic was chosen by using the list of most relevant terms in each topic. This resulted in the right-hand side graphic, with visual representation of the cluster (i.e. topic) formed by those words. <br>

It can be noted that by mapping the intertopic distance we can visually see how close two topics are to each other. <br>


You can play  with an interactive version of the figure below, which shows the top 10 most relevant words for each topic. By selecting a topic number, the probability to encounter its top 10 associated words in the corpus is given along with an estimate of the number of times they are linked to the topic. <br>

For the rest of our analysis we can choose those words to form a set of sub-topics that allows to have more meaningful representation of each topic. <br>

 " height="85%" width="120%" %}



 <br>
 <br>
 The following table summarizes the chosen topics and their associated number:

<table border="0" class="table table-striped text-center" font-size = 9px>
  <thead>
    <tr style="text-align: center;">
      <th></th>
      <th> 1 </th>
      <th> 2 </th>
      <th> 3 </th>
      <th> 4 </th>
      <th> 5 </th>
      <th> 6 </th>
      <th> 7 </th>
      <th> 8 </th>
      <th> 9 </th>
      <th> 10 </th>
      <th> 11 </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th> Topic </th>
      <td> Sports </td>
      <td> Teamwork </td>
      <td> Companies </td>
      <td> Politics </td>
      <td> Games </td>
      <td> Elections </td>
      <td> Datetime </td>
      <td> Family </td>
      <td> Changemakers </td>
      <td> Countries </td>
      <td> Investing </td>
    </tr>
  </tbody>
 </table>
