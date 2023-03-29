# Module 6 Challenge

In this challenge job is to use your data visualization skills, including aggregation, interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities.

# Imports
The Imports used are pandas and hvplot.


![alt text](https://github.com/reiccv/Module_6_Challenge/blob/main/Images/imports.PNG)

![alt text](https://github.com/reiccv/Module_6_Challenge/blob/main/Images/imports1.PNG)

# Calculate and Plot the Housing Units per Year

use numerical and visual aggregation to calculate the number of housing units per year, and then visualize the results as a bar chart.

Use the groupby function to group the data by year. Aggregate the results by the mean of the groups.
![alt text](https://github.com/reiccv/Module_6_Challenge/blob/main/Images/collect1.PNG)


# Calculate and Plot the Average Sale Prices per Square Foot

Use the hvplot function to plot the housing_units_by_year DataFrame as a bar chart. Make the x-axis represent the year and the y-axis represent the housing_units.

Style and format the line plot to ensure a professionally styled visualization.
![alt text](https://github.com/reiccv/Module_6_Challenge/blob/main/Images/collect2.PNG)

# Compare the Average Sale Prices by Neighborhood
Create a new DataFrame that groups the original DataFrame by year and neighborhood. Aggregate the results by the mean of the groups.

Filter out the “housing_units” column to create a DataFrame that includes only the sale_price_sqr_foot and gross_rent averages per year.

Create an interactive line plot with hvPlot that visualizes both sale_price_sqr_foot and gross_rent. Set the x-axis parameter to the year (x="year"). Use the groupby parameter to create an interactive widget for neighborhood.

Style and format the line plot to ensure a professionally styled visualization.

![alt text](https://github.com/reiccv/Module_6_Challenge/blob/main/Images/compare1.PNG)

![alt text](https://github.com/reiccv/Module_6_Challenge/blob/main/Images/compare2.PNG)

# Build an Interactive Neighborhood Map
Read the neighborhood_coordinates.csv file from the Resources folder into the notebook, and create a DataFrame named neighborhood_locations_df. Be sure to set the index_col of the DataFrame as “Neighborhood”.

Using the original sfo_data_df Dataframe, create a DataFrame named all_neighborhood_info_df that groups the data by neighborhood. Aggregate the results by the mean of the group.


![alt text](https://github.com/reiccv/Module_6_Challenge/blob/main/Images/visualize1.PNG)

![alt text](https://github.com/reiccv/Module_6_Challenge/blob/main/Images/visualize2.PNG)

Using hvPlot with GeoViews enabled, create a points plot for the all_neighborhoods_df DataFrame.

Set the geo parameter to True.
Set the size parameter to “sale_price_sqr_foot”.
Set the color parameter to “gross_rent”.
Set the frame_width parameter to 700.
Set the frame_height parameter to 500.
Include a descriptive title.
![alt text](https://github.com/reiccv/Module_6_Challenge/blob/main/Images/visualize3.PNG)



# Compose Your Data Story