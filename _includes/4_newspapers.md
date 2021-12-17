<br>


#### Newspapers in the dataset
{% include side.html text= "assets/export/nb_occurence_news.html"
content = "As the title of this story implies, one of our purposes was to see how controversial newspapers are. As such, it was necessary to select some newspapers to see if their performances were related to the usage of controversial topics.<br>

An initial idea was to select the 10 newspapers with the most appearances in the dataset, however as you will see, it quickly showed unreasonable. <br>

Assuming that a sample of 100’000 quotes might be representative of the dataset. We could extract the distribution of the newspapers over this subset, the results being presented on the histogram. Note that the first journal “news” is actually a newspaper called “news” in Australia.<br>

Those results were not as predicted, we expected to mainly find big names of the industry but it seemed that smaller newspapers were publishing more. They might have tried to overcome the lack of qualitative publications by their number of articles. <br>

It was necessary to check if we were able to access a performance indicator, for example the sales over the last decade, otherwise the selection of the newspapers had to be done using the later criterion.

"  width = "100%"  height = "600px" %}



<br>
#### Newspapers' sales data

The sales data for the aforementioned newspapers were not available. So instead, we checked for which newspapers the sales data could be obtained and then investigated those newspapers presence in our dataset. <br>

Several English newspapers, present in our dataset, had accessible sales data. Therefore, we focused our analysis on those journals. You can see below the evolution of their sales data over the years.

<iframe src="assets/export/sellings.html" height="600" width="1000"></iframe>


<table border="0" class="table table-striped text-center" font-size = 9px>
<thead>
    <tr style="text-align: center;">
    <th>ID</th>
    <th>Newspaper</th>
    <th>Nationality</th>
    <th>Foundation year</th>
    <th>Domain of expertise</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>metro</td>
    <td> <a href="https://metro.co.uk/tag/metro-newspaper/">Metro</a></td>
    <td>UK</td>
    <td>1999</td>
    <td>news, sport, entertainment</td>
  </tr>
  <tr>
    <td>thesun</td>
    <td><a href="https://www.thesun.co.uk/   "> The Sun    </a></td>
    <td>UK</td>
    <td>1964</td>
    <td>news, sport, celebrity, showbiz, politics, business</td>
  </tr>
  <tr>
    <td>dailymail</td>
    <td><a href="https://www.dailymail.co.uk/home/index.html   ">  Daily Mail   </a></td>
    <td>UK</td>
    <td>1896</td>
    <td> breaking news, showbiz, celebrity, sport news, rumours, viral</td>
  </tr>
  <tr>
    <td>standard</td>
    <td><a href=" https://www.standard.co.uk/ ">  Evening Standard   </a></td>
    <td>UK</td>
    <td>1827</td>
    <td>London news, business, sport, celebrity, entertainment</td>
  </tr>
  <tr>
    <td>mirror</td>
    <td><a href=" https://www.mirror.co.uk/  ">  The Daily Mirror   </a></td>
    <td>UK</td>
    <td>1903</td>
    <td>news, sport, celebrity gossip, TV, politics, lifestyle</td>
  </tr>
  <tr>
    <td>thetimes</td>
    <td><a href=" https://www.thetimes.co.uk/  "> The Times    </a></td>
    <td>UK</td>
    <td>1785</td>
    <td>sport, celebrity</td>
  </tr>
  <tr>
    <td>telegraph</td>
    <td><a href="https://www.telegraph.co.uk/   "> The Daily Telegraph    </a></td>
    <td>UK</td>
    <td>1855</td>
    <td>news, business, sport, lifestyle, culture</td>
  </tr>
  <tr>
    <td>dailystar</td>
    <td><a href=" https://www.dailystar.co.uk/  ">  The Daily star   </a></td>
    <td>UK</td>
    <td>1978</td>
    <td>breaking news, celebrity</td>
  </tr>
  <tr>
    <td>express</td>
    <td><a href=" https://www.express.co.uk/  "> Daily Express    </a></td>
    <td>UK</td>
    <td>1900</td>
    <td>news, showbiz, sport, lifestyle</td>
  </tr>
  <tr>
    <td>inews</td>
    <td><a href="  https://inews.co.uk/ ">  i   </a></td>
    <td>UK</td>
    <td>2010</td>
    <td>news analysis and breaking news, business, politics</td>
  </tr>
  <tr>
    <td>ft</td>
    <td><a href=" https://www.ft.com/  ">  Financial Times   </a></td>
    <td>UK</td>
    <td>1888</td>
    <td>world news, economy, finance,</td>
  </tr>
  <tr>
    <td>theguardian</td>
    <td><a href="  https://www.theguardian.com/ "> The Guardian<    </a></td>
    <td>UK</td>
    <td>1821</td>
    <td>world news, sports, business, opinion, analysis, reviews</td>
  </tr>
  <tr>
    <td>dailyrecord</td>
    <td><a href=" https://www.dailyrecord.co.uk/  ">  Daily Record   </a></td>
    <td>UK</td>
    <td>1895</td>
    <td>news, sport, politics, celebrity, gossip<br> </td>
  </tr>
  <tr>
    <td>cityam</td>
    <td><a href=" A.M.  "> City A.M.    </a></td>
    <td>UK</td>
    <td>2005</td>
    <td>business, finance, economy, politics</td>
  </tr>
</tbody>
</table>
