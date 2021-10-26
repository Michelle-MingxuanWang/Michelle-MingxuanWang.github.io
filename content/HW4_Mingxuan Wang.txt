Title: Assignment 4 Description
Slug: Assignment 4 Description
Date: 10/25/2021
Category: Assignment 4
Author: Mingxuan Wang
Summary: Description of Assignment 4

I chose the dataset 6, "Doctorates awarded, by state or location, broad field of study, and sex of doctorate recipients: 2017".  

Firstly, I read the dataset while assigning both the first row and the second row as a multi-index and reform the dataset so it can be used to create a dashboard.  
I Insert a column contains the correspond state code of the states in order to draw the choropleth map.  Moreover, I stacke the dataframe and transformed the formation of the dataframe, then replace the "D" value in the dataset as NaN.  

Then, I do some analysis in Pandas. I calculate the total num of doctorates awarded in different states, field, and print the top 5 states and the top 5 fields with the highest doctorates awarded.   
Moreover, I calculate the proportion of doctorates awarded of male and female.   
What's more, I calculate the ratio of female doctorates awarded and male doctorates awarded among all the field, and find that Education has the highest female to male ratio, Engineering has the lowest female to male ratio.  

Then, I create a dashboard in Dash in plotly.   
By using "px.choropleth" in "dcc.Graph", I draw the choropleth map of the total doctorates awarded in all the 51 states on the map of United States.  
By using "dcc.Dropdown", and "px.bar" and "px.pie" in "dcc.Graph", I create two plots with dropdowns.  The dropdown is useful because it enables the users to choose the feature that they are interested in and add interaction to the dashboard.
The dropdown is linked to the bar plot and the pie plot by using "callback".
Moreover, I add a "hoverData" function to the dashboard. This means that when the user hovers their mouse on the a certain state in the choropleth map,  the corrspond par plot and pie plot of that certain state will be drawn.   
This is another way to add interaction to the dashboard.




