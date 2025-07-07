# 3D mapping (Draft) 
**[DEMO LIVE](https://alicepham01.github.io/HCR-3D-Visualization/) - This is just 3D model not the map to show images and voting hover,thus you can not click on the map pointer(issue markers)**
![image](https://github.com/user-attachments/assets/2a15519a-1b7f-44e6-9455-230a8ad8feba)
## Data  
| Layer               | Description                                                                                 | Type     | Source                                                                                                                                                                                                                                                                       | Attributes                                 |
|---------------------|---------------------------------------------------------------------------------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------|
| walkability_point   | Points indicating walkability-related features                                              | point    | Field survey / Interview data                                                                                                                                                                                                                                                | Import_template.csv             |
| safety_point        | Points showing safety issues                                                                | point    | Field survey / Interview data                                                                                                                                                                                                                                                | Type of issue, category, photo, notes      |
| safety_polygon      | Areas classified under the safety category (e.g. High vehicle density area)                 | polygon  | Field survey / Interview data                                                                                                                                                                                                                                                | Safety level, issue type, dominant feature |
| walkability_polygon | Areas classified under the walkability category (e.g. Inadequate pedestrian amenities area) | polygon  | Field survey / Interview data                                                                                                                                                                                                                                                | Walkability score, obstruction type        |
| 1st_2nd_blocks      | First and second building blocks in study area                                              | polygon  | Field survey and OpenStreetMap                                                                                                                                                                                                                                               | building_height, building_function         |
| 3rd_4th_blocks      | Third and fourth building blocks in study area                                              | polygon  | Field survey and OpenStreetMap                                                                                                                                                                                                                                               | building_height, building_function         |
| Building_plain      | Building footprints around study area                                                       | polygon  | OpenStreetMap                                                                                                                                                                                                                                                                | Basic geometry only                        |
| Ho_Con_Rua          | 3D model of the Hồ Con Rùa area                                                             | 3D OBJ   | [model link](https://embed-3dwarehouse-classic.sketchup.com/model/240d196d-e025-4c86-bd1f-dbd7f9c46f73/Turtle-Lake-Ho-Chi-Minh-city-H%E1%BB%93-Con-R%C3%B9a) | Mesh geometry, texture, landmark elements  |


## Methodology (from investigating to mapping)
### Step 1
![image](https://github.com/user-attachments/assets/1ba665f7-e843-46d6-a79d-15f7dd70a19d)
![image](https://github.com/user-attachments/assets/58c07462-897e-418d-8f1a-f952a2dd660f)
![image](https://github.com/user-attachments/assets/f30dc1b9-0374-4465-81b2-366c36cb81e1)
![image](https://github.com/user-attachments/assets/9c5183e2-5689-4d1e-ab73-322f71a54e8c)
![image](https://github.com/user-attachments/assets/f9b0203d-827e-4517-86f9-0b23551464af)
![image](https://github.com/user-attachments/assets/ba4eea18-f186-4308-827f-6d57fcff1fc8)

## Tool
## References 
https://miliasv.github.io/CTstreets/?city=amsterdam#11.42/52.3451/4.915
