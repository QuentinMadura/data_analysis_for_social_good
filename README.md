# Data analysis methods 

Here we apply some standard data analysis methods to analyze and visualize the data for social good. 
The methods we are using are mostly based on:

1. network theory 
https://github.com/Liyubov/networks_beauty

2. stochastic processes 
https://github.com/Liyubov/networks_random_walking

Repository for analysis of mobility data and trajectories analysis https://github.com/Liyubov/mobility_analysis


### Motivation for this project

These are projects, which inspired creation of this repository:

1. Unicef school mapping project and Magicbox git repository
https://www.unicef.org/innovation/school-mapping

2. Lecturers without borders project, hosted at CRI 
www.scied.network 

3. Open global mobility data of airplane traffic 
from https://bluehub.jrc.ec.europa.eu/migration/app/index.html?state=5cc845a97758cd17cdecd1fb 

# Data description 

The open datasets for this project are taken from:
1. citizen science projects, such as https://scistarter.org/lecturers-without-borders-collecting-information-a
2. open database from mobility data 
https://bluehub.jrc.ec.europa.eu/migration/app/index.html?state=5cc845a97758cd17cdecd1fb 
and from Erasmus travel data



# Data visualisation 

First of all, we start with visualisation of the data. 
We are working with data from csv files structured as:
   |institution name | institution type| institution location| institution contact| institution properties|
The notebooks here are dedicated to data visualisation and data analysis
Example of open data files can be found here https://data.cityofnewyork.us/Education/School-Point-Locations/jfju-ynrr

### Data visualisation sources for interactive maps

Links from Hugo on blocks:
- bl.ocks.org : the main community platform for D3js devs and their nominative porfolio.
-- https://bl.ocks.org/mbostock - Mike Bostock is the creator of D3js
--- https://bost.ocks.org/mike/ - Mike Bostock  tutorials. More links there.
---- Command-Line Cartography
---- Towards Reusable Charts
---- Thinking with Joins
-- https://bl.ocks.org/jasondavies -- Best budy of mbostock for maps
-- https://bl.ocks.org/hugolpz/c89a76096c070a5a7d23 - Hugo Lopez, was a leading D3js cartographer back in 2014. Very rusty fingers now (2019). Globe tour
--- Stackoverflow answer for focus on something !

Codes browsers :
- Blocksplorer : http://bl.ocksplorer.org , tap in bl.ocks.org. Really 2014.
- Observable : https://observablehq.com/search?query=d3.geo -- by mbostock, more 2018

Toolkits:
- https://jsoneditoronline.org -- for topojson data

# Code

### data_on_map_visualisation.ipynb 

We visualise datafiles from two example files 
1. the csv file with data on randomized anonymized educational institutions data
2. the dbf with open data from https://toolbox.google.com/datasetsearch/search?query=schools%20around%20the%20globe&docid=2T2%2BDeqbWNzcqeorAAAAAA%3D%3D 
The example of data are randomized data from educational centres around the world. 
Due to the data privacy reasons we are visualising only in the average characteristics of the data, such as average number of data points and average parameters of datapoints (such as number of resources needed in datapoints etc.).

### mobilitydata analyzer.ipynb 

We analyze open GLOBAL mobility data from open flights where we get information about all cross-border flights. Our main goal is to understand trends in growth of mobility cross-borders vs. intercontinental flights.
More information on it is here https://github.com/Liyubov/mobility_analysis


### LeWiBo_on_map.ipynb 
It is file for the visualisation of activities of the project "Lectures without borders": lectures uploaded to the airtable visualised on a world map, 
preprocessing data from dataframe exported from csv file with all lectures made or planned. More details about project and activities (lectures, seminars of Lectures without borders) are on www.scied.network
We collect the information about schools around the globe on Open Street map file. Contact us if you would like to contribute. 
We also plan to extent mapping to general projects, such as Open Street map plus Humanitarian dataprojects https://data.humdata.org/dataset/hotosm_arm_roads 

###  	analysis_mobility_trajectories_oh_data.ipynb 
We analyze INDIVIDUAL mobility data from openhumans example of data in order to understand movements of individuals. 
(work in progress for analysis of individual trajectories)

### bikes_mobility_analysis.ipynb 
We start to analyze bike mobility data and other properies of bikes sharing systems in Berlin. The notebook is inspired by A.Kapp workshop at City lab Berlin https://github.com/technologiestiftung/bike-sharing . This notebook is in progress.
