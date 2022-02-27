# Project 1 By Jonas Smith 
Design Documentation for Project 1 in INFO H517 Data Visualization. <br />

You can see the YouTube video showcasing how to use this visualization here: <br />
[John Snow 1854 Cholera Map in D3 YouTube Video by Jonas Smith](https://youtu.be/zA9nTEFmsqs)

I began my design planning by reviewing the various data files we had been provided and decided how best to make use of the data contained within each. I knew from the beginning that I wanted to end up with 4 graphs. I wanted a graph of the map of London to the left of the screen and a bar chart timeline graph in the upper right hand corner of the screen with two pie charts for age and gender breakdowns underneath the bar chart but still next to the map. Ideally, I wanted to have the bottom of the pie charts match up to the bottom of the map. I have provided a sketch of the desired layout below <br />

![IMG_2883](https://user-images.githubusercontent.com/54475489/155890763-854c2070-8feb-4aa5-b10c-4453f172d86b.jpeg)

Ultimately, I could not get the positioning how I wanted it initially. I also made the decision to change the pie charts to bar charts, as it was difficult to see just how close the gender divide was on a pie chart compared to a bar chart. <br />

Looking specifically at the street map, I began with drawing the points connected using polyline. I decided to use the channel of color to designate the different types of individuals graphed on the map. I used the [IBM color blind color palette](https://davidmathlogic.com/colorblind/#%23648FFF-%23785EF0-%23DC267F-%23FE6100-%23FFB000) so that individuals with color blindness could still differentiate between the different circle on the map. The burnt orange circles are female deceased individuals and the blue colored circles are male deceased individuals. The channel of size and color were used to indicate pumps which are marked by yellow hued dots on the map. I did not add shape differences based on age groupings to the map as I felt it would diminish the map's interpretability with so many overlapping points. You can see where the major streets Regent Street and Oxford Street are located as well as the Workhouse and Brewery locations. 

