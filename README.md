# Assignment #6

### Due Date: Friday 4/26 by 5pm

## Repository Setup

The link to create your own cloned version of this week's repository is:

https://classroom.github.com/a/rBuR0r-s

## Assignment

This week's assignment will be broken into two parts:

### Part 1: Proposal for the final project

You should submit a short (1/2 to 1 page) proposal that outlines and describe your plan for the final project. 

The description of the final project can be found [here](https://github.com/MUSA-620-Spring-2019/final-project).

The focus of the proposal should be on:

- the data set(s) you wish to use in the project,
- the questions that you want to explore
- the analysis methods and techniques that you will use 
- how the above items satisfy the requirements outlined in the [final project description](https://github.com/MUSA-620-Spring-2019/final-project)

#### Note
For the moment, do not worry too much about how the visualizations/interactive maps will be hosted on the web. We will cover several methods for embedding your visualizations on the web in the coming weeks. These methods fall generally into three categories:

- embedding interactive altair/holoviews plots produced in Python
- embedding visualizations produced in a Observable notebook
- creating an interactive dashboard of plots using a free-tier server to host your code

Much more on these methods in the coming weeks!


### Part 2: Interactive web maps with Folium and Leaflet

In this part, you'll visualize a geospatial data set, queried using an API, using both Folium in Python and Leaflet in Observable. The choice of data set is up to you, but must satisfy a few requirements:

- The data must be pulled using an API
- The data should be in GeoJSON format and be Point features (latitude, longitude)
- In Python, use Folium to create two maps:
  - A map showing the Point features as a GeoJSON layer, with the points styled by a property of the feature data, e.g., red for fatal shootings and blue for non-fatal shootings
  - A map showing a heat map of the data, using the Leaflet.heat plugin
- In Observable, create one map:
  - There must be a slider that controls the data being shown on the map. This could be done by changing the SQL query for the API based on the slider input (as in class), or by filtering the full data set returned by the API based on the user's input. 
  - You can choose to reproduce either of your Foliumn maps as described above. So, the map should show either the Point features as a GeoJSON layer, or use the leaflet heat map plugin to show a heatmap of the data.

**Be sure to make your Observable notebook public by hitting the "publish" button.**

#### Notes

- See the [week 10 lecture](https://github.com/MUSA-620-Spring-2019/week-10/blob/master/lecture-10.ipynb) and [this Observable notebook](https://observablehq.com/@nickhand/shootings-in-philadelphia) for example maps using the Philadelphia shootings data set. **Note: you must choose a data set other than the shootings data set**.
- There are several options for data on OpenDataPhilly — any data set hosted on the CARTO SQL database with associated API documentation will work, similar to the shootings data set. 
- You can also choose a different API to use, as long as it satisfies the above requirements. For example:
  - the [Philadelphia bike share Indego](https://www.rideindego.com/about/data/) has an API of live station data in GeoJSON format: https://www.rideindego.com/stations/json/
  - Data.gov maintains a list of APIs in GeoJSON format: https://catalog.data.gov/dataset?res_format=GeoJSON. Note that not all of these are Point features

## Deliverable and Submission

- Upload a Jupyter notebook with your two Folium plots to your private repository (using the link given above)
- Email to nicholas.adam.hand@gmail.com: 
  - your final project proposal
  - the link to your public Observable notebook that contains your single Leaflet.js map
