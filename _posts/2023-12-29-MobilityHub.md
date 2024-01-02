---
title:  "Florida Mobility Hubs"
mathjax: true
layout: post
categories: transitnewmobility
---




- Mobility Hubs

  Mobility hubs are physical locations that allow travelers to seamlessly switch between various modes of transportation such as public transit, ridehailing, and micromobility. These hubs, by enhancing connectivity and accessibility, contribute to an improved quality of life and offer various socioeconomic benefits. Also, as integral components of transport networks, mobility hubs play a crucial role in integrating new mobility technologies.

  Cities and transit agencies are showing growing interest in integrating mobility hubs into their transportation improvement initiatives. However, there lacks a standardized method for identifying potential locations for mobility hub development.

  <img align="center" width="350" height="250" src="https://github.com/jacobyan0/jacobyan0.github.io/raw/master/images/Mobilityhub_fig1_intro.png" style="vertical-align:middle;margin:15px 15px"/> 

  
- Research Objectives

   The purpose of the research is to develop a methodology framework to assess the suitability of an area for establishing a mobility hub and identify the potential locations. This involves considering various factors, including
  - Accommodating multimodal travel needs and streamlining transfer processes, 
  - Enhancing first-/last-mile connectivity,
  - Promoting socioeconomic equity.

- Analytical Framework

  We have developed a multi-level and multi-criteria approach. The approach consider bus stop clusters as the spatial units for potential hub locations. (It is widely recognized that mobility hubs are most effective when located at or near transit stops with high ridership activity.) We then assign weights and calculate mobility scores based on different scenarios or objectives. We then carry out the evaluation procedure at various scales, including neighborhood, district, or regional levels. 

  <img align="center" width="700" height="250" src="https://github.com/jacobyan0/jacobyan0.github.io/raw/master/images/Mobilityhub_fig2_flow.png" style="vertical-align:middle;margin:15px 15px"/> 

  The framework comprises several key steps:

  1. <u>Cluster Transit Stops</u>: Mobility hubs should be anchored by high-frequency transit. We consider transit stops to be the spatial unit for siting mobility hubs. We use DBSCAN to cluster stops and generate the 1-mile buffer zones from the groups of adjacent transit stops. The below calcualtions are processed and scaled to the spatial units.
  
  2. <u>Determine Criteria and Weights</u>: Recognizing the need for prioritization in infrastructure investments based on various priorities, the tool allows users to adjust weights for constructing the mobility hub index, thereby generating different results for each scenario. Based on literature reviews and stakeholder discussions, five criteria for siting mobility hubs are identified: transit supply, first-/last-mile connectivity, accessibility, infrastructure, and social equity. Each criterion includes several indicators and sub-indicators, and their weighted sum results in a composite score. The final mobility hub index is constructed by summing the weighted scores of the five criteria, with varying weights based on scenarios or planning priorities.
  
  3. <u>Compute Neighborhood-Level Hub Index</u>: Using the results from Steps 1 and 2, the index value for the neighborhood-level hub is calculated, assuming a potential catchment area of one mile.
  
  4. <u>Identify a Network of Mobility Hubs</u>: Steps include selecting the site with the highest index value as the first hub, excluding potential hubs within 2 miles of selected hubs, and repeating these steps until the service area of the mobility hubs covers 75% of transit coverage areas or the total number of hubs reaches a specified limit (N). District- and regional-level hub indexes are then computed for the selected neighborhood hubs, assuming catchment areas of 3 and 5 miles, respectively.

  We develope the analytical procedure with ArcGIS Pro and Python.

- Project Data Collection
    1. Transit Data: Gainesville Regional Transit System (RTS) provides information on bus routes and stops, obtained from the General Transit Feed Specification (GTFS) dataset. Bus ridership data, including passenger counts and on-board wheelchair and bicycle amounts, are collected from the city of Gainesville.
    2. FM/LM Connectivity Data: Micromobility trip data, covering e-scooter and micro-transit trips, is collected from the city of Gainesville. Census block-level FMLM gap scores are derived from the American Community Survey (ACS) and LEHD Origin-Destination Employment Statistics (LODES).
    3. Infrastructure Data: Intersection density data, indicating multi-modal and pedestrian-oriented facilities, is sourced from the Smart Location Database. Road infrastructure data is collected from OpenStreetMap (OSM), offering detailed information about road networks.
    4. Socioeconomic Data: Demographic variables related to population, race, age, income, and vehicle ownership are considered for socioeconomic analysis. This data is sourced from ACS.
    5. Accessibility Data: Smart Location Database provides data on destination accessibility via auto or transit. Walkability around bus stops is evaluated using walk scores obtained from the Walkscore API.

- Results and Findings

  For each of the six different scenarios, we identified neighborhood-level, district-level and regional-level mobility hubs.

  <img align="center" width="700" height="400" src="https://github.com/jacobyan0/jacobyan0.github.io/raw/master/images/Mobilityhub_fig3_case.png" style="vertical-align:middle;margin:15px 15px"/> 

  In general, this outcome seems fairly plausible. Most of neighborhood-level hubs locate at southwest and east Gainesville. District-level hubs should be built at Oak Mall, north Gainesville and GNV airport, which has the highest FMLM gap. Butler Plaza and downtown Gainesville are also potential sites for district-level hubs, which has higher transportation equity score and transit supply. Shands Hospital is most suitable for siting the regional-level mobility hub, where ridership and accessibility were the highest. 
  
  

- Acknowledgement
  
  The research team would like to thank the Florida Department of Transportation (FDOT) Transit Office for the assistance in understanding the scope of the project and for providing feedback on this project.
  We would also like to thank the following stakeholders for participating in this project: the City of Gainesville, FDOT District Two, and FDOT District Four.
  And we would also like to thank Gainesville Regional Transit System (RTS) for providing the route and stop information, transit schedule, and ridership data.
  
  


For the full report and the developed tools: Report for the Gainesville Study; [ArcGIS toolbox and code](https://github.com/jacobyan0/Just-and-Green-Transportatiion-Lab).

  
*Key words: mobility hub, multimodal travel, public transit*
