# Visualizing Education Inequality

## Summary 
This visualization shows the inequality in Math performance between male and female students in various countries.
- In most countries, male students perform better than female students in math.
- The more developed a country is, the better the students' math performance is.
- The level of development of a country does not reduce gender gap in math performance.

## Design 

#### Dataset information
The dataset taken from a survey designed by <a href=http://www.oecd.org/pisa/data/pisa2012database-downloadabledata.htm>Programme for International Student Assessment (PISA)</a>. Around 510,000 students in 65 economies took part in the PISA 2012 assessment of reading, mathematics and science, representing about 28 million 15-year-olds globally. Rather than examing how well students have learnt the school curriculum, this assessment evaluates how well prepared the students are for life beyond school.<br><br>
I cleaned up the dataset by taking the weighted average score of each country as well as the average score for both genders. I have also incorporated <a href=http://data.worldbank.org/indicator/NY.GDP.PCAP.CD>The World Bank's data</a> on countries' GDP per capita to compare the assessment results based on the level of development of each country.

#### Version 1
<a href=https://bl.ocks.org/siyubao/51ecf537beac3e588b76254079207a36>- Math Performance by GDP Per Capita</a><br><br>
My initial idea is to show two kinds of inquality: 1) the level of development of countries; 2) in each country, the gap between male and female students. <br><br>
In this visualization, I used GDP per capita on the x-axis to represent the level of development of countries, and students' test scores on the y-axis to indicate the performance of each country in relation to other countries globally. Size of the circles reflects how big the gap between male and female students' performance is, and colors of the circles represent which gender perform better (red for female and blue for male). I also added tooltips explaining which country is represented by each of the circles, values for both x and y axes, and the size of the gender gap of math performance. <br>

#### Feedback 1
- Wording in the legend is a bit confusing: What does 'advantage' mean?
- Explanation needed: It's hard to interpret what the bubbles and their varying sizes mean. There are too many things going on at once. May consider adding some explanation, or segment the chart to make it clearer for readers.
- Vagueness in circle sizes: It's unclear whether the diameter or the size of the circles is representing the sizes of gender gap.
- Extent of the y-axis: It may be necessary to tell the audience a little more about the test and the range of the test score, such as "Test Scores, Max 650, based on X exam".
- Sizes of the bubbles: It's hard to hover over the bubbles on the left as it's so crowded over there. May consider reducing the bubble size.

#### Feedback 2
- The data points are a little cramped on the left side of the graph. It seems that the correlation between GDP and math performance is extremely high for low-income countries. It's rather interesting that if the country is poor, GDP per capita explains almost all of the test performance, but as the country gets richer, the correlation goes closer to zero. The left side contains a lot of interesting information, but because it's so crowded, the audience cannot actually see anything. It would be great if you could zoom in on the left side to really go into the details.
- It’s also pretty cool to see the gender gap in math performance. However, I don't see why you would want to associate it with the level of development of the countries. It would make a lot of sense if more red bubbles appear as the countries get richer, or the blue ones gets smaller towards the right, but currently there seems to be no correlations between the gender gap and the country's level of development. I would consider making two charts, one with and one without gender, to display the sizes of the gap and see what to do from there.

#### Version 2
<a href=https://bl.ocks.org/siyubao/6b29e4a5d50ad0e171ce97911a98bbcd>- Visualizing Inequality in Math Performance</a><br><br>
In this version, I clarified the meaning of "advantage" in the legend and changed the title and subtitle to directly address the two types of education inequality. I also decreased the size of the circles so that the graph looks neater and clearer. Also, more information is now shown on legend. 
However, I didn’t split the graph as is suggested. The clarity of the graph improved a great deal simply by reducing the bubble size. My initial goal of creating this visualization was to fit in as much information as possible. The current version looks pretty good to me and I would love to ask more people if they could understand what I'm tring to say in the visualization.

#### Feedback 3
- In this visualization, I see a moderate correlation between a country’s economic development and its students’ math performance. Gender inequality seems to be a problem in most of the participating countries.
- I like this visualization because it contains many layers of information – the use of color and orientation of the elements makes the communication pretty efficient. However, I also noticed in your code that the bubble size is scaled from 5-15. Since our eyes are not so sensitive with changes in area, we may perceive a larger blue coverage than there really is. I would suggest scaling the bubbles from 1-15.
- As a reader who has absolutely no prior knowledge, it would be great if the visualization contains more information to guide us through understanding the graph.

#### Version 3
<a href=http://bl.ocks.org/siyubao/3190dda26c5d6af283d930020feede2f>- Visualizing Inequality in Math Performance</a><br><br>
In this updated version, I added some more information about the two datasets and replaced the subtitle with a clearer step-by-step explanation of the elements in the graph. I’ve also rescaled the circle size so that it reflects the range truthfully. 

## Resources
<a href=http://www.oecd.org/pisa/data/pisa2012database-downloadabledata.htm>PISA 2012</a>
<a href=http://data.worldbank.org/indicator/NY.GDP.PCAP.CD>GDP Per Capita</a>
