![DSL Logo][dsllogo]


# Identifying Food Desert Neighbourhoods in the Niagara Region

### Introduction
For this project, I will explore neighbourhood data using ArcGIS Insights to identify food desert neighbourhoods in Niagara Region. Data for the purpose of this project were gathered from Niagara Open Data and Niagara Poverty Initiative websites. Variables that will be examined to identify food deserts are distance to supermarkets and number of supermarkets. I will also analyze the data to detect spatial patterns. Finally, I will share my work on ArcGIS online and create new shapefiles from my results.

### Project Procedures

1 . Download the Niagara Food Deserts compressed folder from the GitHub link below:
https://github.com/pdwomoh/Philip-Dwomoh-DSL-Project

2 . Locate the downloaded file on your computer. Right-click the file and extract it to a location where you can easily find it, such as your Documents folder.

3 . Sign in to your Insights Online account:https://insights.arcgis.com/#/

>**Note**: If this is your first time using Insights, the **Welcome to Insights** window appears with a list of things you can do with Insights.


4 . If necessary, in the **Welcome to Insights** window, click **Skip**.

5 . Click the **Workbooks** tab.

6 . Click **New workbook**.

![ Picture of New Workbook][logo1]


 
>Note: The **Add To Page** window appears.
>In this window, you can choose a dataset to add to your new workbook. 
>You can choose data hosted in your ArcGIS organization, data in a file on your computer, or data from Living Atlas. 


7 . In the left pane, click **Files**.

![picture of File button][logo2]


8 . Click Browse my computer. Browse to the extracted **Niagara Food Deserts** folder and select **Book1.xlsx**. and **NhbBoundaries compressed zip** folder and click **Open**.

9 . In the **Selected Data** pane, click **Add**.

![picture of selected data][logo3]

 
>The datasets are added to a new card in your workbook. 
>You use cards and pages to organize information in a workbook.
>Each page can contain multiple cards, and each card can contain a map, chart, or table. 



10 . Click **Untitled Workbook**, type *Niagara's Food desert Neighbourhoods* and press **Enter**.

11 . Click **Page 1**, type *Data Exploration*, and press **Enter**.

12 . In the data pane, point to **Book1** and click **Rename dataset**.

![picture of rename dataset][logo4]

 
13 . Type *Food Desert Data* and press **Enter**.

14 . Repeat the above step and rename **NhbBoundaries to Niagara Neighbourhood Boundaries** and press **Enter**.

15 . Point to **Food Desert Data**, click **Dataset Options**, and choose **Enable Location**. 

![picture of enable location][logo5]

           
16 . In the **Enable Location** window, for **Location type**, choose *Geography*. For **Location Fields** choose *Multiple*, and for the **Multiple Fields** choose *NHB_NAME and MUN*. For **Matching Geography Level**, choose *Niagara Neighbourhood Boundaries*.

![picture of location type in enable location][logo6]

 
17 . Click **Run**.

18 . When the **Enable Location tool** finish loading, a new locations attribute named **Niagara Neighbourhood Boundaries** is added to **Food Deserts Data**.

![picture of new location in the data pane][logo7]

 
 
>Note: I chose geography as the location type because the food Deserts Data did not have any coordinate or address attribute.
>Hence making it possible to correspond the food deserts data’s locations to that of the zipped Niagara Neighbourhood boundaries  shapefile. 


19 . Rename the following fields in the food deserts data in the data pane:

From |	To 
--- | ---
NBH_NAME |	Niagara Neighbourhoods
MUN |	Municipality
No_sup |	Number of Supermarkets
No. supermarket within 5km |	Number of Supermarket within 5 km


After completing the renaming, click on the **Food Deserts Data** to close the drop-down attribute.


20 . In the data pane, Drag **Food Deserts Data** to your page and onto the **Chart** drop zone. And finally drag it to the **Bar Chart** zone.

 ![picture showing the movement of food deserts data to your page][logo8]


21 . Click on the **Visualization type** and select **Summary table**.

  ![picture of visualization type][logo9]


22 . Click on the **NBH_ID** drop down arrow and click on the field “**Municipality**”.

![picture of NBH_ID drop down arrow][logo10]

 
23 . Similarly click on the**Counts of Food Deserts Data** drop down arrow and click on “**Number of Supermarkets**”.

![picture of count of food deserts data drop down arrow][logo11]

 
The **Summary Table** now depicts Municipalities in Niagara and their corresponding supermarket accessibility.

![picture of summary table][logo12]

 
24 . Click **Visualization type** and select **Bar Chart**. Drag the center-right handle of the **Bar Chart Card** until the card is at a maximum length.

![picture showing the extension of the bar chart card][logo13]



**Changing the symbology of the bar chart card**.

25 . First click on the ‘**Legend**’. Click **Options** inside the Layer option box. Change the **Symbol type** from **Single symbol** to **Unique symbols** and click “**x**” to close the layer option box. Finally click anywhere outside the **Bar Chart Card**.

![picture showing how to change the symbology of a bar chart card][logo14]

 
 >**Note**: Click on the **bars** to identify the number of supermarkets available to each municipality.
 
26 . Click on **Card 1** and type “**Number of Supermarkets by Municipality**” as the title for the bar chart, and press **Enter**.

27 . Click **Save**.

![picture showing the save button][logo15]
 
 


**Identifying Food Deserts Neighbourhoods in the Niagara Region**

28 . In the data pane, Drag **Food Deserts Data** to your page below the **Bar Chart Card** and onto the **Map** drop zone.  

29 . Click **Legend**, click the **arrow** to the right of the food deserts data as shown on the map.

![picture that can show the legend options][logo16]

 
30 . The **Layer options** box pops up. Click **Options**. For **Style by**, choose *Niagara Neighbourhoods* and for the **Symbol style** confirm that it is *Unique symbols*. When finished close the Layer options box.

![picture of the layer options procedure][logo17]

 
**We now want to identify neighbourhoods with no access to supermarkets**.
31 . Click on **Card Filter**.

![picture of the filter button][logo18]

 
32 . A new filter box pops-up. Below **Filter By** click on the **Choose a field** drop down arrow and select **Number of supermarkets**.
 
![picture of the filter by procedure][logo19]
 
 
33 . Drag to you left from **7** until you reach **0**. Click **Apply** and close **Filter**.

**Below is the map of Niagara’s neighbourhoods without supermarkets**.

![picture of neighbourhoods without supermarkets][logo31]


>**Note**: Click on each **area on the map** to identify neighbourhoods without supermarkets.

34 . Finally click anywhere outside the Map Card.

35 . Click on **Card 1** and type “*Niagara Neighbourhoods without Supermarkets*” as the title for the Map, and press **Enter**.

36 . Click **Save**.

37 . Go to the **Data pane**, click **Dataset** at the right side of **Food Deserts Data Map Result**. Click **Share Data**. 

![picture of the share data procedure][logo20]

 
38 . Follow the steps in the Share data box below and click Share.
 
![picture of the share data box][logo21]
 

Once the data is shared, ‘Shared.Open Item’ appears below the Food Deserts Data as seen below.

![picture of the shared.Open item in the data pane][logo22]

  
39 . Repeat the same process for **Bar Chart 1** in the Data pane and follow the procedure in the shared data below. Click **Share**.

![picture of the share data procedure][logo23]

 
Once the data is shared, ‘Shared.Open Item’ appears below the Bar Chart 1 as seen below.

![picture of the shared.Open item in the data pane][logo24]


 
**Identifying food deserts in Niagara neighbourhoods using distance parameters**.

40 . Go back to the map. Click **Card filter** to add new filter. Click **New Filter**. For **Filter by** choose the field ‘**Number of supermarkets within 5km**’. Drag from **25** to **0** and click **Apply**.

![picture of the filter by number of supermarket procedure][logo25]


**Below is the map of Niagara’s food desert neighbourhoods without access to supermarkets within 5 km**.
 
 ![Map of Niagara's food desert neighbourhoods without access to supermarkets within 15 km][logo26]
 
 
 >**Note**: Click on each **area on the map** to identify neighbourhoods considered as food deserts within 5 km.
 
41 . Click anywhere outside the Map card.

42 . Click on “**Niagara Neighbourhoods without Supermarkets**” and rename it as **Niagara’s Food Desert Neighbourhoods by Distance**, and press **Enter**.

![picture of the new map name][logo27]

 
43 . Share the map using the same steps used for the first map result. 
 
![picture of the share data procedure][logo28]
 
 
44 . Click **Share**.

45 . Finally Click **Save**.

**Creating new shapefiles from my results**.

46 . Go to the **Food Desert Data** map output dataset in the **Data pane**, click **Dataset** and click **Export**, and finally select **Shapefiles**.

![picture showing the procedure for creating  shapefiles][logo29]

 
47 . Save the new shapefile to your desired location on your computer.

![picture showing the procedure for saving  shapefiles][logo29]


48 . You can also repeat this above process to also create a shapefile for the **Bar Chart** as well. 
                                             
                                             
                                                                                    

### Conclusion

This project explored the potential of ArcGIS Insight in identifying Niagara's food desert Neighbourhoods.The findings revealed that neighbourhoods deemed as food deserts within 5 km were Caistor, Wainfleet, Gainsborough, Bethel/Gasline/Sherkston and Stevensville. Results from the project were also shared on ArcGIS online. Finally, new shapefiles were created from the project results.


 
                          **Thank you and have a prosperous New Year**.
 









<!--- Please use reference style images so that it is easier to update pictures later --->

[dsllogo]: dsl_logo.png
[logo1]: logo1.png
[logo2]: logo2.png
[logo3]: logo3.png
[logo4]: logo4.png
[logo5]: logo5.png
[logo6]: logo6.png
[logo7]: logo7.png
[logo8]: logo8.png
[logo9]: logo9.png
[logo10]: logo10.png
[logo11]: logo11.png
[logo12]: logo12.png
[logo13]: logo13.png
[logo14]: logo14.png
[logo15]: logo15.png
[logo16]: logo16.png
[logo17]: logo17.png
[logo18]: logo18.png
[logo19]: logo19.png
[logo20]: logo20.png
[logo21]: logo21.png
[logo22]: logo22.png
[logo23]: logo23.png
[logo24]: logo24.png
[logo25]: logo25.png
[logo26]: logo26.png
[logo27]: logo27.png
[logo28]: logo28.png
[logo29]: logo29.png
[logo30]: logo30.png
[logo31]: logo31.PNG

