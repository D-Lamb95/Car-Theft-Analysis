🚗 Car Theft Analysis

Exploring theft patterns for Kia/Hyundai vehicles using Python visualizations

Overview

This project analyzes vehicle theft data with a focus on Kia and Hyundai models, which experienced a nationwide spike in thefts due to a well‐publicized security vulnerability. The analysis explores how frequently these vehicles were stolen compared to other brands, how thefts vary by city, and how counts differ across years. The project uses Python to create multiple visualizations, including pie charts, stacked bar charts, and treemaps, to help highlight patterns within the data.
The visualizations and calculations used to support this analysis are found in the notebook export:

Data Description

The dataset includes records of stolen vehicles with fields such as:

  -  Vehicle make (Kia, Hyundai, or Other)

  -  Theft type

  -  Year

  -  City or location

  -  Theft counts (e.g., total thefts per location in 2022)

The notebook processes these fields to generate aggregated tables (e.g., thefts by location for 2022) and visualizations like pie charts and stacked bar charts that highlight how strongly Kia/Hyundai models appear in the theft totals.
For example, the code grouping theft data by location and summing theft counts for 2022 appears here:

Methods
1. Data Cleaning

Numeric fields such as annual theft counts were cleaned and coerced into numeric values (pd.to_numeric(..., errors='coerce')).
Rows with missing or invalid counts were removed.

2. Theft Distribution Visualization

A pie chart was created to compare the share of thefts between:

Kia/Hyundai

All other makes

This visualization highlights the disproportionate impact on Kia and Hyundai vehicles.
The plotting code can be seen here:

3. Theft Counts by Year and City

A stacked bar chart shows the number of thefts across different cities and years.
Labels, legends, and rotation settings were applied to ensure readability.

4. Treemap Visualization

A treemap aggregates theft counts by location to show the highest‐impact areas.
Data was grouped by location and summed to create proportional block sizes.

Key Findings

  -  Kia and Hyundai thefts represent a large share of total thefts in the dataset, as shown in the distribution pie chart.

  -  Theft counts are clustered in specific cities, which appear clearly in the stacked bar visualization.

  -  The treemap highlights several “hotspot” locations with much higher theft counts.

  -  Year‐over‐year trends show that the spike aligns with the years when security vulnerabilities became widely known.

Requirements

  -  To run the notebook, you need:

  -  Python 3.x

  -  pandas

  -  matplotlib

  -  seaborn (optional depending on plotting)

  -  numpy

Install dependencies:
pip install pandas matplotlib seaborn numpy

How to Use

  -  Open the notebook or exported HTML file.

  -  Load the theft dataset into a pandas DataFrame.

  -  Run each cell to clean the data, generate summary tables, and view visualizations.

  -  Inspect charts (pie, stacked bar, treemap) to compare Kia/Hyundai theft patterns vs. all other vehicles.

Future Improvements

  -  Add geospatial mapping using GeoPandas or Folium

  -  Incorporate temporal animations to show theft trends over time

  -  Compare theft patterns to population density or income by area

  -  Extend analysis to model‐level details (e.g., specific Kia/Hyundai models)

Files Included

  -  Car_Theft_Analysis.ipynb or HTML export (your uploaded file)

  -  Dataset of reported vehicle thefts

  -  README summarizing analysis and results
