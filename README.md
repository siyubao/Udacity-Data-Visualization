# Visualizing Education Inequality

## Summary 
This visualization shows the inequality in Math performance between male and female students in various countries.
- In most countries, male students perform better than female students in math.
- The more developed a country is, the better the students' math performance will be.

## Design 

#### Dataset information
The dataset taken from a survey designed by <a href=http://www.oecd.org/pisa/data/pisa2012database-downloadabledata.htm>Programme for International Student Assessment (PISA)</a>. Around 510,000 students in 65 economies took part in the PISA 2012 assessment of reading, mathematics and science, representing about 28 million 15-year-olds globally. Rather than examing how well students have learnt the school curriculum, this assessment evaluates how well prepared the students are for life beyond school.<br><br>
I cleaned up the dataset by taking the weighted average score of each country as well as the average score for both genders. I have also incorporated <a href=http://data.worldbank.org/indicator/NY.GDP.PCAP.CD>The World Bank's data</a> on countries' GDP per capita to compare the assessment results based on the level of development of each country.

#### Version 1
<a href=https://bl.ocks.org/siyubao/51ecf537beac3e588b76254079207a36>- Math Performance by GDP Per Capita</a><br><br>
My initial idea is to show two kinds of inquality: 1) the level of development of countries; 2) in each country, the gap between male and female students. <br><br>
In this visualization, I used GDP per capita on the x-axis to represent the level of development of countries, and students' test scores on the y-axis to indicate the performance of each country in relation to other countries globally. Size of the circles reflects how big the gap between male and female students' performance is, and colors of the circles represent which gender perform better (red for female and blue for male). I also added tooltips explaining which country is represented by each of the circles, values for both x and y axes, and the size of the gender gap of math performance. <br>

#### Feedback 1
- Wording in the legend is confusing: What does 'advantage' mean?
- Explanation needed: It's hard to interpret what the bubbles and their varing sizes mean. There are too many things going on at once. May consider adding some explanation, or segment the chart to make it clearer for the readers.
- Vagueness in circle sizes: It's unclear whether the diameter or the size of the circles is representing the sizes of gender gap.
- Extent of the y-axis: It may be necessary to tell the audience a little more about the test and the range of the test score, such as "Test Scores, Max 650, based on X exam".
- Sizes of the bubbles: It's hard to hover over the bubbles on the left as it's so crowded over there. May consider reducing the bubble size.

#### Feedback 2
- The data points are a little cramped on the left side of the graph. It seems that the correlation between GDP and math performance is extremely high for low income countries. It's rather interesting that if the country is poor, GDP per capita explains almost all of the test performance, but as the country gets richer, the correlation goes closer to zero. The left side contains a lot of interesting information, but because it's so crowded, the audience cannot actually see anything. It would be great if you could zoom in on the left side to really go into the details.
- The gender gap is also cool, but I don't see why you would want to associate it with the level of development of the countries. It would make a lot of sense if more red bubbles appear as the countries get richer, or the blue ones gets smaller towards the right, but currently there seems to be no correlations between the gender gap and the country's level of development. I would consider making two charts, one with and one without gender, to display the sizes of the gap and see what to do from there. 


#### Version 2
<a href=https://bl.ocks.org/siyubao/6b29e4a5d50ad0e171ce97911a98bbcd>- Visualizing Inequality in Math Performance</a><br><br>
I clarified the meaning of "advantage" in the legend and changed the title and subtitle to directly address the issue. I also made the circles smaller so that the graph looks neater and clearer. 


#### Version 3

## Resources

