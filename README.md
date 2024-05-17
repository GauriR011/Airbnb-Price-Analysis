# F20DV Group 5 - Data Visualization Project

## GitLab Project URL
This project has been taken from GitLab where it was originally uploaded. Below is the link to the GitLab page:
[https://gitlab-student.macs.hw.ac.uk/dr2007/f20dv-group-project](url)

## **Team Members:**
- Arshati Ajay (H00382093)
- Farheen Anwari Badubhai (H00379639)
- Gauri Revankar (H00373987)
- Prasitha Prasanna Naidu (H00379641)

## **Contributions:**
- Arshati - Density Plot visualization
- Farheen - Scatter Plot Map visualization
- Gauri - LM Plot visualization and Dashboard
- Prasitha - Grouped Bar Chart visualization and Dashboard

## **Overall Project Concept**

This project explores the factors affecting the Air Bnb prices in European cities - Berlin, Rome, Paris, London, and Amsterdam.

Each listing is evaluated on various attributes such as 
- [ ] Room types
- [ ] Latitude and Longitude
- [ ] Distance from the city center
- [ ] Distance of the metro from the housing
- [ ] Tourist Attraction index and restaurant index

#### The dashboard displays 4 visualization charts:

**1) Scatter Plot Map -**
The interactive map visualization dynamically illustrates the geographical spread of Airbnb listings across five key European cities: London, Paris, Amsterdam, Berlin, and Rome. 

It is designed for an intuitive user experience:
- By selecting a city, the viewer is taken to a detailed map of that location.
- The map displays the listings as colored dots to indicate pricing tiers: green for low-priced, yellow for middle-range, and red for high-priced properties, with specific price ranges established for each category.
- Hovering over any dot on the map reveals additional information, such as the listing's weekday and weekend prices, providing an immediate, detailed understanding of pricing variations.

_Attributes Covered:_
- [ ] Latitude
- [ ] Longitude
- [ ] realSum (Total Price of the listing)
- [ ] Cities
- [ ] day_type (Weekday/Weekend)


**2) Density Plot -**
We're using the density plot to visually explore the distribution of Airbnb prices with respect to distances from the city center and metro distance from the listing, across different cities.

_Attributes covered:_
- [ ] realSum (Total Price of the listing)
- [ ] City
- [ ] Distance
- [ ] Metro distance


**3) Linear Model Plot (LM Plot) -**
We're using the LM Plot to find how the proximity of restaurants and attractions affects the housing prices in different cities. 

_Attributes covered:_
- [ ] realSum (Total Price of the listing)
- [ ] City
- [ ] Restaurant Index
- [ ] Attraction Index


**4) Grouped Bar Chart -**
The grouped bar chart on the Airbnb dataset displays the relationship between the price (on the y-axis) and the city name (on the x-axis) for different room types (represented by bars). 

Each bar represents a different room type, and the height of the bar indicates the average price for that room type in the respective city.

_Attributes covered:_
- [ ] realSum (Total Price of the listing)
- [ ] Room type
- [ ] City name
- [ ] Number of Airbnbs of each room type in the city (hover)

## _**Project File Stucture**_

The main branch contains the final code of the project. Project is executed through the home.html file of id branch.

#### The main branch contains the following files and folders:
- The **data folder** contains the csv file that contains the data to be visualized on the dashboard.
- The **lib/d3 folder** contains the Javascript file to execute d3 version 7 commands. 
- The **scripts folder** contains the Javascript files of each visualization.
- The **styles folder** contains the CSS stylesheets of each visualization as well as the dashboard. 
- The **home.html** file contains the code for the dashboard where all the visualizations are linked throught their corresponding Javascript files. This file needs to be executed to view the dashboard.
- The **images folder** contains image.png and up_arrow.png icons that are included in the layout of the dashboard.

#### The scripts folder contains the following files:
- **BarChart.js** contains the Javascript code for the Grouped BarChart visualization.  
- **LM_Plot.js** contains the Javascript code for the LM plot visualization. It defined a class named LM_Plot which is imported in **LM_Plot_main.js** file.
- **density.js** contains the Javascript code for the Density plot visualization.
- **map.js** contains the Javascript code for Scatter Plot map visualization.
- **LM_Plot_main.js** imports the LM_Plot class and passes the dataset to the class and renders the graphs. It also defines the buttons to help users switch between the 2 LM plots (Restaurant Index and Attraction Index graphs).

#### The styles folder contains the following files:
- **barchart.css** contains the CSS  properties that apply to the Grouped BarChart visualization.
- **density.css** contains the CSS  properties that apply to the Density plot visualization.
- **lmPlot.css** contains the CSS  properties that apply to the LM Plot visualization.
- **map.css** contains the CSS  properties that apply to the Scatter Plot Map visualization.
- **home.css** contains the CSS  properties that apply to the dashboard screen (home.html file).
- **main.css** imports all the other CSS  files mentioned above.

### Interactions
The Density plot and Grouped Bar chart visualizations are inter related. As in, results of selections made in one of the graphs are applied to the other. For instance, if London was selected to be explored in the Density plot visualization, then the Grouped Bar chart will show the bars of the corresponding city. 

All the 4 graphs can be interacted from the dashboard. By selecting the options given in the sidebar, the user can immediately jump to where the graph is located (instead of having to scroll down to the graph). The user can always go back to the top of the dashboard view by clicking the up arrow icon on the top right corner of the dashboard screen.

### Additional information
- Each member has created their own branch to work on their own visualizations.
- The combining branch was used to combine the visualizations into the dashboard.
- The final design was pushed to the main branch.
