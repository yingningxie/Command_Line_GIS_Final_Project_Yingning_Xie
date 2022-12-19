# Philadelphia Bike Network Converage for Urban Agriculture and Community Gardens

## Description of Datasets
I used the datasets from "OpenDataPhilly", for Urban Agricutlure Programs (2021), Community Gardens (2021), and Bike Network (2014). I also used US Census Data (2019) for population and household Income, and the calculation of population density, as well as the bike network density. 

Urban Agricutlure Programs, Community Gardens, and Bike Network were downloaded as GeoJSON, and read into Google Colab. I joined the two datasets "Urban Agricutlure Programs" and "Community Gardens", and created a column "type".

I also joined "Bike Network" with census data, which I cut to Philadelphia level, and grouped and sumed Bike Network shape_length by census tract, and calculated the density by area.

### Figure 1: Population Density
![Figure 1](https://user-images.githubusercontent.com/118480366/208327547-e3b249ed-3b55-4839-8ef8-e2b20a1e4666.png)

### Figure 2: Median Household Income
![Figure 2](https://user-images.githubusercontent.com/118480366/208328030-9f4561d2-be75-4980-8d3a-fb7a35248687.png)

### Figure 3: Bike Network Density
![Figure 3](https://user-images.githubusercontent.com/118480366/208328097-a3cd31b0-231c-4328-94f6-7616a6b12e0a.png)

### Interactive Map: Urban Agriculture Programs and Community Gardens
<iframe src="final.html" height="1200" width="105%"></iframe>
