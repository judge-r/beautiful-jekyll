---
type: posts
layout: post
title: GIS Pittsburgh
subtitle: My first independent GIS project (2014)
---
This is a project I completed in 2014 for my Geographic Information Systems (GIS) class at Northeastern using the ArcGIS 10.2 program. I apologize for the low quality graphics- some things may be difficult to read without zooming in. I am working on learning how to create better quality images. Enjoy!

In the increasingly unpredictable world we live in, GIS demonstrates its capacity to act as an important tool for emergency response planning in the event of catastrophe. Therefore, it is an important asset to map hazardous areas for environmental risks such as: flooding, landslides, groundwater pollution, hazardous waste facilities, nuclear facilities, chemical plants, landfills, air emission plants, and many others that pose either direct or indirect threats to public health. Once GIS identifies these areas, emergency response agencies such as Firefighting, EMS, FEMA, CDC, and Police can plan strategies to mitigate the risk to people who live in hazardous areas. For example, people who live close to an inactive landfill may be at risk of health problems from contaminated drinking water if the landfill is seeping waste into groundwater. GIS allows public/environmental health agencies to address these hazards more easily in cases of emergency by developing strong emergency response plans. This study identifies the health risks posed by multiple man-made hazards including: landfills, air emissions facilities, hazardous waste storage sites and other natural hazards such as: landslide-prone areas and flooding in the city of Pittsburgh, PA. Here, the 3 most hazardous neighborhoods are identified based on a sum of the hazardous features located within them. An additional neighborhood is also identified as hazardous for its high landslide potential. Finally, spatial data tools are used to illustrate the geographic location of all neighborhoods in relation to Level 1 Trauma centers and other area hospitals to simplify city emergency response plans. 

The Office of Emergency Management of New York City uses GIS capabilities extensively to prepare for natural disasters. For example, the office has mapped Hurricane evacuation zones for the entire city. In addition, they map areas of the city where languages other than English are spoken to plan for sending translators to those areas to help people find emergency resources in the event of a natural disaster or other emergency. After the 2010 earthquake in Haiti, a company called Geoeye used imagery satellite data to assist rescue crews in searching areas of Port-Au-Prince where people were most likely to be found among the wreckage. The applications of GIS are very comprehensive and can be useful in many different situations. 

All of the layers used in the development of GIS maps for this study utilize the State Plane projected coordinate system labeled as: NAD_1983_StatePlane_Pennsylvania_South_FIPS_3702_Feet. Some of the layers were sourced from the Pennsylvania Spatial Data Access and were thus either countywide or statewide data. The remaining layers were sourced from the Pittsburgh GIS website and just included data within Pittsburgh City limits. Therefore, many of the county and statewide layers were clipped to the Pittsburgh polygon layer (Neighborhoods). 

The first map illustrated in this paper highlights the environmental hazards around the city of Pittsburgh such as flood risk and landslide potential (Fig. 1). The landslide risk varies around the city on a scale of 1-37 as shown by a graduated color map. The Western part of the city to the West of the Allegheny River is very hilly and also has some undermined areas which both contribute to its high landslide potential. 

__Figure 1.__ Environmental Hazards
[![Figure 1. Environmental Hazards]({{ site.url }}/img/PIT_GIS_Fig_1.png)]({{ site.url }}/img/PIT_GIS_Fig_1.png)

The man-made hazards within Pittsburgh city limits include: captive hazardous waste, commercial hazardous waste facilities, air emission plants, and municipal waste facilities comprised mainly of landfills and dump sites (Fig. 2). This visual better illustrates the most hazardous areas of the city in terms of direct public health threats from air pollution and groundwater contamination.

__Figure 2.__ Man-made Hazards
[![Figure 2. Man-made Hazards]({{ site.url }}/img/PIT_GIS_Fig_2.png)]({{ site.url }}/img/PIT_GIS_Fig_2.png)

Figure 3 provides a more complete visual that shows all of the neighborhood boundaries with all the natural and man-made hazards explored in this study. To measure the extent of risk for man-made hazards for each neighborhood, several spatial joins were conducted to join the attribute tables of the man-made hazard features to uncover which neighborhoods contained the greatest number of hazards. The results showed that the 3 "high risk neighborhoods" were: Central Business District with 30 hazardous features, and the Bloomfield and South Side Flats neighborhoods each with 27 hazardous features. The South Side Flats neighborhood is at particular risk because it is completely within the 100-year flood zone, which is also mapped. The symbology of these neighborhoods was changed first by selecting them and then creating a new, separate layer. The other neighborhood highlighted in this map is the Fineview neighborhood in the Northwest part of the city. Although it is at low risk of man-made environmental hazards, nearly the entire land area of Fineview is at substantial risk for landslides (Fig. 3).

__Figure 3.__ Hazardous Neighborhoods
[![Figure 3. Hazardous Neighborhoods in Pittsburgh]({{ site.url }}/img/PIT_GIS_Fig_3.png)]({{ site.url }}/img/PIT_GIS_Fig_3.png)

Figure 4 shows the hospitals and Level 1 trauma centers in Pittsburgh labeled by blue and red crosses respectively. To show the neighborhoods closest to each of the 3 trauma centers, a simple join was conducted and each group of neighborhoods that corresponded to a certain trauma center were color-coded in green, red, and blue. The proximities were each measured as the distance from the center of each neighborhood, to the trauma centers. A map like this can help emergency services plan for emergency response to each hospital in the event of a medical emergency caused by one of the hazards.

__Figure 4.__ Hazard and Health Response Zones
[![Figure 4. Hazard and Health Response Zones]({{ site.url }}/img/PIT_GIS_Fig_4.png)]({{ site.url }}/img/PIT_GIS_Fig_4.png)

All of the data used for this project was acquired from the Pennsylvania Spatial Data Access (PASDA) or the City of Pittsburgh GIS website through the Division of City Planning. This data allowed me to conclude that the most at-risk neighborhoods in Pittsburgh are: Fineview, Central Business District, South Side Flats, and Bloomfield. The hazards in these neighborhoods vary by location. Potential catastrophes that could occur in these areas (while unlikely in most cases) would be: power plant explosions, hazardous waste leaks, landfill seepage and groundwater contamination, flooding, and landslides. The only less serious health hazard from this study would be air pollution from emissions. The Central Business district is the only neighborhood that is in close proximity with air emissions plants in this case making it most at risk of effects of air pollution or a potential gas leak or explosion anomaly. In terms of response strategy, the University of Pittsburgh Medical Center Mercy Hospital best serves the Central Business District and South Side Flats neighborhoods. The Bloomfield neighborhood is best served by the UPMC Presbyterian Hospital and the Fineview area is best served by Allegheny General Hospital. These new city divisions that correspond to access to medical care are vital to further planning of rescue and emergency services. This study serves to act as a simple basis for which more GIS strategies can be utilized to research natural and man-made human health hazards and response strategies in Pittsburgh.

Data References:
1.	Pennsylvania Spatial Data Access (PASDA)
(http://www.pasda.psu.edu/uci/SearchPage.aspx)

2.	City of Pittsburgh GIS Database:
(http://pittsburghpa.gov/dcp/gis/gis-data)
 
