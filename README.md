# Project 1 By Jonas Smith 
Design Documentation for Project 1 in INFO H517 Data Visualization. <br />

You can see the YouTube video showcasing how to use this visualization here: <br />
[John Snow 1854 Cholera Map in D3 YouTube Video by Jonas Smith](https://youtu.be/zA9nTEFmsqs)

I began my design planning by reviewing the various data files we had been provided and decided how best to make use of the data contained within each. I knew from the beginning that I wanted to end up with 4 graphs. I wanted a graph of the map of London to the left of the screen and a bar chart timeline graph in the upper right hand corner of the screen with two pie charts for age and gender breakdowns underneath the bar chart but still next to the map. Ideally, I wanted to have the bottom of the pie charts match up to the bottom of the map. I have provided a sketch of the desired layout below <br />

![IMG_2883](https://user-images.githubusercontent.com/54475489/155890763-854c2070-8feb-4aa5-b10c-4453f172d86b.jpeg)

Ultimately, I could not get the positioning how I wanted it initially. I also made the decision to change the pie charts to bar charts, as it was difficult to see just how close the gender divide was on a pie chart compared to a bar chart. <br />

Looking specifically at the street map, I began with drawing the points connected using polyline. I decided to use the channel of color to designate the different types of individuals graphed on the map. I used the [IBM color blind color palette](https://davidmathlogic.com/colorblind/#%23648FFF-%23785EF0-%23DC267F-%23FE6100-%23FFB000) so that individuals with color blindness could still differentiate between the different circles on the map. The burnt orange circles are female deceased individuals and the blue colored circles are male deceased individuals. The channel of size and color were used to indicate pumps which are marked by yellow hued dots on the map. I did not add shape differences based on age groupings to the map as I felt it would diminish the map's interpretability with so many overlapping points. I struggled at first with getting the lines drawn properly as I forgot to adjust for the mirror effect caused by D3's y-axis inversion, but eventually corrected this issue. You can see where the major streets Regent Street and Oxford Street are located as well as the Workhouse and Brewery locations. <br />

Next, I moved on to the timeline graph where I placed a scaled y-axis and chose not to add an x-axis as I felt it made the visualization feel less interactive and over cluttered. I also made this graph using colors in IBM's color blind color palette linked above. When you hover over a single bar in the graph, it will change color and a title card will appear next to the cursor contain the count and day that the individual bar represents. I was unable to tie deaths on the map of London to deaths by day in the timeline graph as the two data files were not linked in any way. 

I chose to make the age and gender breakdown graphs all IBM color blind color palette compliant and each categorical grouping has a different color. First I felt like this added more color to the screen and made it easier at first glance to tell these were categorical groupings. Similar to the timeline graph I chose to use a hover title card feature that displays information about the individual bars. 

Overall, the two biggest questions that can be answered from these visualizations are "Did more men or women die from the 1854 Cholera outbreak in London?" and "What segment of the population is most likely to die?" From the image below, we can see that while women account for slightly more Cholera deaths than men, it is not at a rate that we could deduce women have a higher risk of death. We can see, however, that individuals aged 0-10 and individuals aged greater than 80 years old have the highest chance of death from Cholera infection.

![Screen Shot 2022-02-27 at 12 11 52 PM](https://user-images.githubusercontent.com/54475489/155892444-76e68a50-5124-4144-9f7b-390fde73c8b1.jpg)

I have definitely learned a lot about D3 throughout this process and look forward to developing my skills further as the semester continues! The github repository containing my code as index.html is located [here](https://github.com/jsmith873/Project1-Data-Visualization.git). While various examples were examined to understand logic, I only used coding example files from the *Interactive Data Visualization for the Web* textbook and our in course examples in writing the actual script itself. 
