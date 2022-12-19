# Philadelphia Bike Network Converage for Urban Agriculture and Community Gardens

## 1. Introduction
Urban Agriculture has been advertised as a nature-based solution to climate change. Many urban agriculture programs are also used to promote citizen participation and community cohesion. Meanwhile, as e-bikes get trendy recently, its benefits have attracted great attention. For instance, compared with conventional bikes, e-bikes travel faster, and longer distance. It has also been found that e-bikes could help to promote social equity, as it might be a mobility resource that could be more practical than convential bikes, but still affordable for low-income communities.

This project aims to look at the interaction between the Urban Agriculture Programs and bike network coverage in the city of Philadelphia. Combined with census data, such as population density, median household income, and percent of non-white population by census tract, the project will showcase the distribution of urban agricutlure and community gardens in Philadelphia, and how easily they could be accessed by bikes and ebikes, to provide potential equity implications.

## 2. Description of Datasets
I used the datasets from "OpenDataPhilly", for Planning Districts, Urban Agricutlure Programs (2021), Community Gardens (2021), and Bike Network (2014). I also used US Census Data (2019) for population and household Income, and the calculation of population density, as well as the bike network density. Urban Agricutlure Programs, Community Gardens, and Bike Network were downloaded as GeoJSON, and read into Google Colab. I joined the two datasets "Urban Agricutlure Programs" and "Community Gardens", and created a column "type". I also joined "Bike Network" with census data, which I selected to Philadelphia county, and grouped and sumed Bike Network shape_length by census tract, and calculated the density by area.

## 3. Static Maps
Three maps are presented: Population Density, Median Household Income, and Bike Network Density.

### Figure 1: Population Density
We could see from the map that high population density areas are in central Philadelphia and its surrounding areas. Some tracts do not have population data, such as airports.

![Figure 1](https://user-images.githubusercontent.com/118480366/208327547-e3b249ed-3b55-4839-8ef8-e2b20a1e4666.png)

### Figure 2: Median Household Income
Higher income households seem to be located in central Philadelphia, northwest and northeast Philadelphia. North, lower north, upper north, west, university southwest seem to have higher concentration of relatively low-income households.

![Figure 2](https://user-images.githubusercontent.com/118480366/208328030-9f4561d2-be75-4980-8d3a-fb7a35248687.png)

### Figure 3: Bike Network Density
Central Philadelphia, west, university southwest have the overall highest bike network density. 

![Figure 3](https://user-images.githubusercontent.com/118480366/208328097-a3cd31b0-231c-4328-94f6-7616a6b12e0a.png)

## 4. Interactive Map: Urban Agriculture Programs and Community Gardens
Most urban agriculture and community gardens in Philadelphia are located in central or south of the city. If we turn off other layers and turn on the layer "percent of non-white population", we could see a pattern of distribution of urban agriculture programs and community gardens in comparison with non-white population distribution. Meanwhile, we could combine the census information from tooltips to get an idea of how the distribution could be related to household income or population density.

From the initial map we could see the distribution of the coverage of bikes and e-bikes within 10 minutes of travel from the urban agriculture or community gardens. It is clear that e-bikes could better facilitate the connectivity of many more urban agriculture and community gardens. Also, if we just compare the census layer and the bike/e-bike buffer, we could explore the coverage of bike network for census tracts that have high share of non-white population.
<iframe src="final.html" height="1200" width="105%"></iframe>

## 5. Conclusion
Overall, from the maps we could get an overall idea of the interaction between bike network and urban agriculture/community gardens in Philadelphia. We could also see the differences in coverage between conventional bikes and e-bikes. However, since the bike/e-bike buffers are not built based on protected bike lanes, it could have limitation because unprotected bike lanes could be a barrier for bicycle use. 
