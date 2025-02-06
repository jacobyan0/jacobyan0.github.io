---
title:  "A Novel Method for Locating Mobility Hubs"
mathjax: true
layout: post
---

  
Mobility hubs are physical locations that allow travelers to seamlessly switch between various modes of transportation such as public transit, ridehailing, and micromobility. These hubs, by enhancing connectivity and accessibility, contribute to an improved quality of travel and offer various socioeconomic benefits. Also, as integral components of transport networks, mobility hubs play a crucial role in integrating new mobility technologies.

  <img align="center" width="350" height="250" src="https://github.com/jacobyan0/jacobyan0.github.io/raw/master/images/Mobilityhub_fig1_intro.png" style="vertical-align:middle;margin:15px 15px"/> 

  <br/>
  
- ### Research Objectives

   We have developed a methodology to assess the suitability of an area for establishing mobility hubs and identify potential locations. This involves considering five major factors, including
  - Accommodating multimodal travel needs and streamlining transfer processes,
  - Integrating with existing bikeped infrastructure,
  - Enhancing first-/last-mile connectivity,
  - Promoting access to destinations,
  - Promoting socioeconomic equity.

<br/>

- ### Analytical Framework

  We have developed a multi-criteria approach for identifying multi-level mobility hubs. The approach considers bus stop clusters as the spatial units for potential hub locations (as it is widely recognized that mobility hubs are most effective when located at or near transit stops with high ridership activity). We calculate scores, assign weights, and calculate mobility indexes based on different scenarios. We then carry out the evaluation procedure at various scales, including neighborhood, district, or regional levels. 

  <img align="center" width="700" height="250" src="https://github.com/jacobyan0/jacobyan0.github.io/raw/master/images/Mobilityhub_fig2_flow.png" style="vertical-align:middle;margin:15px 15px"/> 

  The framework comprises several key steps:

  1. <u>Cluster Transit Stops</u>: Mobility hubs should be anchored by high-frequency transit. We use the DBSCAN algorithm to cluster stops and generate 1-mile buffer zones, and consider the buffer areas to be the spatial unit for siting mobility hubs. The below calcualtions are processed and scaled to these spatial units.
  
  2. <u>Determine Criteria and Weights</u>: The framework allows planners to adjust weights for different considerations (criteria) and construct the final mobility hub index. It can generate different results for different scenarios. Based on literature reviews and stakeholder discussions, five criteria for siting mobility hubs are identified: transit ridership and supply, first-/last-mile connectivity, accessibility, infrastructure, and social equity. Each criterion includes several indicators and sub-indicators. The final mobility hub index is constructed by summing the weighted scores of the five criteria, with varying weights based on scenarios or planning priorities.
  
  3. <u>Compute Neighborhood-Level Hub Index</u>: Using the results from Steps 1 and 2, we calculate the index value for the neighborhood-level hubs. We then identify the neighborhood-level hubs based on the index. Steps include selecting the site with the highest index value as the first hub, excluding potential hubs within 1.5 miles of selected hubs, and repeating these steps until the service area of the mobility hubs covers 75% of transit coverage areas or the total number of hubs reaches a specified limit (N). 
  
  4. <u>Identify a Network of Mobility Hubs</u>: District- and regional-level hub indexes are then computed for the selected neighborhood hubs. In this step, we enlarge the catchment area of the spatial unit and assume catchment areas of 3 and 5 miles, respectively.

<br/>

- ### Data sources
    1. Transit Data: Gainesville Regional Transit System (RTS) provides information on bus routes and stops through the General Transit Feed Specification (GTFS) dataset. RTS also provides bus ridership data, including passenger counts and on-board wheelchair and bicycle amounts.
    2. FM/LM Connectivity Data: Micromobility trip data, covering e-scooter and micro-transit trips, is collected from the City of Gainesville. Census block-level FM/LM gap scores are derived from the American Community Survey (ACS) and LEHD Origin-Destination Employment Statistics (LODES).
    3. Infrastructure Data: Intersection density data, indicating multi-modal and pedestrian-oriented facilities, is sourced from the Smart Location Database. Road infrastructure data is collected from OpenStreetMap (OSM), offering detailed information about road networks.
    4. Socioeconomic Data: Demographic variables related to population, race, age, income, and vehicle ownership are considered for socioeconomic analysis and are sourced from ACS.
    5. Accessibility Data: Smart Location Database provides data on destination accessibility via auto or transit. Walkability around bus stops is evaluated using walk scores obtained from the Walkscore API.

<br/>

- ### Results 

  We have generated results for six planning scenarios:
    - Enhancing transit
    - Enhancing first-/last-mile connectivity
    - Leveraging existing infrastructure
    - Promoting equity
    - Enhancing accessibility
    - Equal weights

  For each scenario, we identified a network of neighborhood-level, district-level, and regional-level mobility hubs in the City of Gainesville.

  <img align="center" width="700" height="400" src="https://github.com/jacobyan0/jacobyan0.github.io/raw/master/images/Mobilityhub_fig3_case.png" style="vertical-align:middle;margin:15px 15px"/> 

  Most neighborhood-level hubs are located in southwest and east Gainesville. District-level hubs should be built at Oak Mall, north Gainesville, and GNV airport, which has the highest FM/LM gap. Butler Plaza and downtown Gainesville are also potential sites for district-level hubs, which have higher transportation equity scores and transit supply. Shands Hospital is most suitable for siting the regional-level mobility hub, where ridership and accessibility were the highest. 

  <br/>

- ### Validation and Refinement

We believe that mobility hub planning cannot be done through a pure data-driven process. Hence, we have aimed to validate and refine the results by engaging stakeholders and residents through an interactive-mapping-enabled crowdsourcing approach. Click on the image below to watch a YouTube video that describe our crowdsourcing approach:

[![Crowdsourcing community input for mobility hub planning](https://github.com/jacobyan0/jacobyan0.github.io/raw/master/images/MobilityHubCrowdsourcing.png)](https://www.youtube.com/watch?v=KqSUk5cCEII&ab_channel=Xiang%27Jacob%27Yan)

  <br/>
  <br/>

- ### Conclusion
  
    In this project, we present a GIS-based analytical framework for identifying the most suitable locations for mobility hubs within the context of Gainesville, Florida. The proposed methodology is designed to evaluate and prioritize potential hub locations at different scales by assigning scores and weights to a variety of criteria. These criteria encompass essential factors such as transit supply availability, first-/last-mile connectivity, accessibility, road infrastructure, and socioeconomic equity. By integrating these criteria into a comprehensive evaluation process, this research aims to provide valuable insights and data-driven recommendations that will guide the strategic placement of mobility hubs in Gainesville, ultimately fostering a more efficient, equitable, and accessible urban transportation system.

<br/>
<br/>


- ### Other Resources
The mobility hub identification tool (including a set of ArcGIS toolbox and Python script) developed from the project can be downloaded by [clicking here](https://github.com/jacobyan0/Just-and-Green-Transportatiion-Lab/tree/main/Florida%20Mobility%20Hubs). Read more about the project: 
- [ArcGIS Storymap](https://storymaps.arcgis.com/stories/9c56b17d9587428b8b4e323979576c67)
- Webinar: https://www.youtube.com/watch?v=d0FJiCnMOS8&ab_channel=Xiang%27Jacob%27Yan
- Final Report (coming soon)

<br/>
<br/>

- ### Acknowledgement
  
  The research team would like to thank the funding support from the Florida Department of Transportation (FDOT) for funding this project. Project managers Chris Wiglesworth, Gabe Matthews, David Sherman, and Kristin Gladwin provided valuable comments and guidance for this project. We would also like to thank the following stakeholders for participating in this project: the City of Gainesville (Jesus Gomez & Debbie Leistner), FDOT District Two (Janell Damato & Derek Dixon), and FDOT District Four (Lisa Maack & Wibet Hay). 
  
