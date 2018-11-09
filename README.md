# Data-Science-Proj-Forest-Cover-Type

Motivation :
The data is cartographic variables (as opposed to remotely sensed data). The actual forest cover type for a given 30 x 30 meter cell was determined from US Forest Service (USFS) Region 2 Resource Information System data. Independent variables were then derived from data obtained from the US Geological Survey and USFS. The data is in raw form (not scaled) and contains binary columns of data for qualitative independent variables such as wilderness areas and soil type. The areas of forest under study represent forests with minimal human-caused disturbances, so that existing forest cover types are more a result of ecological processes rather than forest management practices.

Data Overview :
The study area includes four wilderness areas located in the Roosevelt National Forest of northern Colorado which are as follows:
1 - Rawah Wilderness Area
2 - Neota Wilderness Area
3 - Comanche Peak Wilderness Area
4 - Cache la Poudre Wilderness Area

Our goal is to predict the forest cover type. The seven types of forest cover are :
1 - Spruce/Fir
2 - Lodgepole Pine
3 - Ponderosa Pine
4 - Cottonwood/Willow
5 - Aspen
6 - Douglas-fir
7 - Krummholz

This is a classification problem where the target could belong to any of the seven classes.

Data Fields:
Elevation - Elevation in meters
Aspect - Aspect in degrees azimuth
Slope - Slope in degrees
Horizontal_Distance_To_Hydrology - Horz Dist to nearest surface water features
Vertical_Distance_To_Hydrology - Vert Dist to nearest surface water features
Horizontal_Distance_To_Roadways - Horz Dist to nearest roadway
Hillshade_9am (0 to 255 index) - Hillshade index at 9am, summer solstice
Hillshade_Noon (0 to 255 index) - Hillshade index at noon, summer solstice
Hillshade_3pm (0 to 255 index) - Hillshade index at 3pm, summer solstice
Horizontal_Distance_To_Fire_Points - Horz Dist to nearest wildfire ignition points
Wilderness_Area (4 binary columns, 0 = absence or 1 = presence) - Wilderness area designation
Soil_Type (40 binary columns, 0 = absence or 1 = presence) - Soil Type designation
Cover_Type (7 types, integers 1 to 7) - Forest Cover Type designation

Question: Given the other attributes, what will be the 'Cover_Type'?
The training set (15120 observations) contains both features and the Cover_Type. The test set (565892 observations) contains only the features.

Assumptions:
Ecology of the areas across which the data is collected is similar.
Seasonal changes are constant across all the observations.
The dataset is recently collected.

Limitations:
Environmental factors affecting the growth of any cover type is not taken into consideration.
Human error while collecting data is not accounted for.
Management practices that might have affected the growth is not accounted for.
