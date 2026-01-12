# 3D mapping (Draft) 
**[LIVE DEMO ](https://map-issues.ditip.vn/3d)

![image](https://github.com/alicepham01/HCR-3D-Visualization/blob/fa56cfc988187958c559ec81212ac9115a68997f/overall%20interface.png)
| Layer Info |  |
|------------|---------------|
| **Walkability & Safety Layers**<br>• `walkability_point` layer — 🟢 Green, Map pointer icon<br>• `safety_point` layer — 🔴 Red, Map pointer icon<br>• `walkability_polygon` layer — 🟢 Green shaded areas<br>• `safety_polygon` layer — 🔴 Red shaded areas | ![image](https://github.com/user-attachments/assets/71fdf0de-9daf-4d31-a824-093e792a8d76) |
| **Building Block Layers**<br>• `1st_2nd_blocks`: First and second blocks with building height and function<br>• `3rd_4th_blocks`: Third and fourth blocks with similar attributes.<br> **Only land use affects children's walking, as shown by the colors in the legend of the left picture.** | ![Picture1](https://github.com/user-attachments/assets/13e91a51-8fb2-4afc-b715-76ff810bea5d) |

## Methodological Workflow
![image](https://github.com/alicepham01/HCR-3D-Visualization/blob/28a38c72cb83d8a29d723f3bf1e7f33a1b3d200c/Diagram.png)
## Data  
| Layer               | Description                                                                                 | Type     | Source                                                                                                                                                                                                                                                                       | Attributes                                 |
|---------------------|---------------------------------------------------------------------------------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------|
| walkability_point   | Points indicating walkability-related features                                              | point    | Field survey / Interview data                                                                                                                                                                                                                                                | [Category2Id](Import_template.csv)            |
| safety_point        | Points showing safety issues                                                                | point    | Field survey / Interview data                                                                                                                                                                                                                                                | [Category1Id](Import_template.csv)      |
| safety_polygon      | Areas classified under the safety category (e.g. High vehicle density area)                 | polygon  | Field survey / Interview data                                                                                                                                                                                                                                                | [Category1Id](Import_template.csv)    |
| walkability_polygon | Areas classified under the walkability category (e.g. Inadequate pedestrian amenities area) | polygon  | Field survey / Interview data                                                                                                                                                                                                                                                | [Category2Id](Import_template.csv)           |
| 1st_2nd_blocks      | First and second building blocks in study area                                              | polygon  | Field survey and OpenStreetMap                                                                                                                                                                                                                                               | building_height, building_function         |
| 3rd_4th_blocks      | Third and fourth building blocks in study area                                              | polygon  | Field survey and OpenStreetMap                                                                                                                                                                                                                                               | building_height, building_function         |
| Building_plain      | Building footprints around study area                                                       | polygon  | OpenStreetMap                                                                                                                                                                                                                                                                | Basic geometry only                        |
| Ho_Con_Rua          | 3D model of the Hồ Con Rùa area                                                             | 3D OBJ   | [model link](https://embed-3dwarehouse-classic.sketchup.com/model/240d196d-e025-4c86-bd1f-dbd7f9c46f73/Turtle-Lake-Ho-Chi-Minh-city-H%E1%BB%93-Con-R%C3%B9a) | Mesh geometry, texture, landmark elements  |

## Methodology (from investigating to mapping)

### Step 1 - Test walks and Photographing
We studied the literature and made a list of all the factors that are most commonly found to impact walking experience. A systematic walking audit was conducted across the study path to observe and document physical conditions affecting pedestrian experience. The team recorded field notes and photographs using GPS-enabled mobile devices to take coordination of objects, focusing on predefined indicators such as dangerous intersections, sidewalk encroachments, among others.

![image](https://github.com/user-attachments/assets/42fee24e-2e03-498e-890b-bfa5080fed5d)

### Step 2 - we clustered factors/issues into 3 categories: safety, convenience adn conviviality
![image](https://github.com/user-attachments/assets/b54e6822-b9fa-45fe-86d6-c749feca4e79)
![image](https://github.com/user-attachments/assets/19752d4b-659f-4e40-8966-be3ec4878c77)
![image](https://github.com/user-attachments/assets/cbeb6e5a-38bf-4bb2-9925-7bc42d65b15c)

### Visualizing issues and solution images
Each problem location was documented with textual descriptions, spatial information, field photographs, and visualised design solutions to facilitate intuitive understanding and informed voting.

<img width="564" height="463" alt="image" src="https://github.com/user-attachments/assets/bbfd8798-eff3-496b-981f-34d798997168" />
<img width="561" height="468" alt="image" src="https://github.com/user-attachments/assets/d306d72f-3e3d-464b-92bf-8009dca03542" />


### Step 4 - Mapping 
Drawing from both field survey observations and georeferenced data obtained through interviews, the 22 issues were digitized as point features and categorized into thematic groups within a structured GIS database. (Using QGIS)

![image](https://github.com/user-attachments/assets/9763f4c7-dd41-459c-ab97-dba9c08d4311)
### Step 5 - 	Visualize all layers in 3D using QGIS2ThreeJS, Export to HTML.
Follow this [instruction](https://opengislab.com/blog/2023/3/11/how-to-incorporate-3d-models-into-qgis-to-create-a-3d-scene) to visualize and export folder
### Step 6 - 
## Tool
QGIS 
@Manual{QGIS_software,
  title        = {QGIS Geographic Information System},
  author       = {{QGIS Development Team}},
  organization = {Open Source Geospatial Foundation},
  year         = {2024},
  url          = {http://qgis.org},
}
## References 
https://miliasv.github.io/CTstreets/?city=amsterdam#11.42/52.3451/4.915]

https://senseable.mit.edu/desirable-streets/

https://sidewalk-sea.cs.washington.edu/explore

https://media.voog.com/0000/0036/2451/files/BeirutCommunityStreets_catalog_Venice2023.pdf

https://cityform.mit.edu/projects/beirut-community-streets

