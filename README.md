# About
This is really rough-and-ready, as they say on GBBO, but for me and for where I started, I'm quite proud of the result. This Bar Chart project uses and SVG object to make the bar chart, taking the user's information and using it to create a rect element and adding it into the SVG in the HTML. 

# Context
This is the final stretch project for the prep modules for the Full-Time Web Development Bootcamp that begins July 25th! 

# Example Screenshots
![Screenshot of a graph made using the HTML page](https://github.com/danispinxo/Bar-Chart-Stretch/blob/master/images/SS-graph.png)

![Screenshot of the input section of the HTML page](https://github.com/danispinxo/Bar-Chart-Stretch/blob/master/images/SS-input.png) 

# API Functions
This bar chart maker engages with users through the webpage. They input data on the page and the JavaScript uses SVG to make a bar graph from the data, including title customization. 

# Functions and Parameters
This project relies on three primary functions: two anonymous functions added to button-click event listeners, and one function called drawBarChart. 

The first anonymous function on the title customizing button retrieves the user input for the title customization and applies it to a title placeholder div. 

The second anonymous function on the add-bar button collects the user input for each new bar, assembles it as an object, and pushes it to an array.

The drawBarChart function takes the array and uses the information for each object in that array to draw SVG rect elements. These elements are labeled and color-coded according to user input. Their size is determined by each bar's percentage of the overall data input, which is then applied as a percentage of the overall SVG object in the HTML file. The labels for each bar currently show at the end of each bar, which is not ideal. But, they are still functional as labels. 

# Feature list of your library
In this project I use some minor CSS (would love to use more), some jQuery for the event listeners, and, of course, SVG for the graph/rectangle creation.

# A list of known issues / bugs

## Bar Number
The primary issue here is that this graph can currently only hold a limited number of bars. More work would have to be done to adjust the SVG object and the bar creation functions to expand/contract depending on the number of items in the array. Should not be too hard, but wanted to submit something fully-functional before the prep module deadline. 

## Negative Numbers
Currently, this project does not support any negative values that may be input by a user. I am not sure how this would work using the SVG except to shift everything over to the right if a negative integer is input as a value. This would require a lot of work and I'm not anywhere close to there yet. 

## Arguments
I don't actually use any functions that take arguments here, even though I know that was a part of the assignment. I just found it easier to create the function without arguments. 

# List of features to add

## Design and More CSS
I would love to add more design and more extensive CSS to this project. Visually, it looks very rudimentary and I would like to keep the pink/purple color scheme and more cutomization on the buttons especially throughout. This is something I will continue to work on as we learn more CSS. 

## X/Y Customization
This project does not currently support customizing the bar graph to be from the x or the y axis, as recommended in the instructions. I suspect that this would be easy--just have two different bar creation functions, one that has static width and shifting height, and one with static height and shifting width (current)--but, again, this is a considerable amount of work and the time is limited.

## Bar Label Placement
I would prefer if the bar labels were on the bars themselves. This would require two levels of customization: 1. that would adjust the placement of the text depending on the size of the bar, and 2. that would make the text either black for a light-coloured bar or white for a dark-colored bar. Again, not too difficult. Plans for that in the future. 

# List of external resources used

- [w3 jQuery Tutorial](https://www.w3schools.com/jquERy/default.asp)
- [w3 SVG Tutorial](https://www.w3schools.com/graphics/svg_intro.asp)
- [Maximilian Schwarzmuller's Udemy Javascript Course](https://www.udemy.com/course/javascript-the-complete-guide-2020-beginner-advanced/)
- [MDN on Web APIs](https://developer.mozilla.org/en-US/docs/Web/API)
