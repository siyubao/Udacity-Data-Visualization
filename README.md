# Visualizing Education Inequality

## Summary 
This visualization shows the inequality in Math performance between male and female students in various countries.
- Male students perform better than female students in most countries.
- Asia has the most countries in which girls perform better
- The more developed a country is, the higher the students' math levels are, especially among European countries.
- Economic development does not improve math performance after a certain point.

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

#### Feedback 4
- Currently your visualisation is more on the exploratory side - presenting the reader with the data and allowing them to interpret for themselves. To make your visualisation more explanatory you need to make sure this message is in your graphic as well. Changing the wording of your title and introductory paragraph is the easiest way to do this. Often a newspaper headline style title is a good start.
- I think you've got one key problem - you are trying to tell too many stories on one chart and in doing so you are not getting a clear message across. So you are looking at Gender Inequality AND Financial Inequality. Looking at these issues one at a time:
Gender Inequality - your colour scales are fantastic. They really highlight how pronounced the male dominance is across the board. However, the overlapping of the bubbles makes it very difficult to see what's going on, particularly from $0-$60,000. And, the bubble size is also confusing both with overlapping and having a legend which refers to colour but not size.
Financial Inequality - as referenced in the feedback the correlation between low performance and low GDP is really interesting but you just can't see what's going on with all the overlapping.
- I have various suggestion, all or a combination of which might solve the problem above. It is a matter of testing them out and seeing which you prefer.
1. restricting the GDP scale - i.e. 0, 20,000, 40,000, 60,000, over 80,000
2. keeping the chart type, colour coding and X-axis (GDP) but losing the radius scale and having two charts alongside each other - one with Maths score on the Y-axis, the other with Gender Difference on the Y-axis.
3. making your chart bigger or responsive to the size of the webpage - see link here under cross browser solution.

#### Version 4
<a href=http://bl.ocks.org/siyubao/b74542d1aba425380812b0894a1a3657>- Gender and Economic Inequalities Remain Critical to High School Math Education Levels</a><br><br>
In this version, I changed the title into a self-explanatory one and added some key findings right below the graphics. 
I've also created buttons to filter the countries, making it a lot easier to see each point. I've also deleted the feature of 'scaling circle by size' because it distract readers from the main points I'm making. 
Also, I've changed the styling to make the graph look better.

## Resources
<a href=http://arnicas.github.io/interactive-vis-course/Week7/lines_transition.html>Interactive Data Vis</a><br>
<a href=http://www.oecd.org/pisa/data/pisa2012database-downloadabledata.htm>PISA 2012</a><br>
<a href=http://data.worldbank.org/indicator/NY.GDP.PCAP.CD>GDP Per Capita</a>
