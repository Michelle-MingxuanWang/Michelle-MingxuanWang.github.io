Title: Assignment 3 Description
Slug: Assignment 3 Description
Date: 10/1/2021
Category: Assignment 3
Author: Mingxuan Wang
Summary: Description of Assignment 3


For plot 1, I draw a map plot for the deaths over the year in each entity
In this plot, I want to show the deaths of each country on a map to clearly visualize the deaths in each entity
Therefore, I use "choropleth" function in "plotly" package. 
Moreover, I figure an animation widget will be suitable here to present the change of deaths over the year, so I use "Play" and "IntSlider" function in "widgets" package to create an animation.

For plot 2, I create a line plot of deaths over the years for each entityin each age group.
I want to present the change of deaths over the year, and contrast the deaths of different age groups.
So I use "line" function in "plotly" package to create a line plot, as "year" on the x-axis, "deaths" on the y-axis, and "age_group" as the color.
Futhermore, I think specifying the entity will be helpful for the plot's interpretability, so I use "Dropdown" function in "widgets" package to make the plot interactive with choosing entities.

For plot 3, I make a pie chart of deaths for age groups of each country. 
I want to show the different proportion of deaths in each age group, so I use "pie" function in "plotly" package.
And I use "Dropdown" function in "widgets" package to make the chart interactive when choosing entities.