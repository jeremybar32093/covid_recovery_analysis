# philadelphia_housing_analysis

This repository contains jupyter notebooks and relevant source data to perform a high level analysis and exploration of the Philadelphia housing market over the past 5 years (2016-2020). The 2 main jupyter notebooks are as follows:

**1.) 1_housing_etl**

This notebook reads in a dataset obtained from the [Philadelphia Office of Property Assessment](https://www.opendataphilly.org/dataset/opa-property-assessments). The dataset from this link obtained is the *Properties (CSV)* dataset.
* The scope of analysis was limited to primarily finished residential properties. As such, the following filtering conditions were applied:
  * Filter only on residential zoning codes
  * Filter on only categories of single family, multi-family, mixed use
  * Filter out properties marked as 'unfinished'
  * Filter on records with sale prices >= 1000
  * Filter on number of rooms > 0
* In addition to row filtering, some columns were determined as out of scope and thus excluded from analysis
* Lastly, some column reformatting was necessary to reformat Excel formatted dates and remove extraneous decimals from zip code field  

**2.) 2_housing_visualizations**

After cleaning up the dataset in our **1_housing_etl** notebook, relevant analysis and visualizations are created in the **2_housing_visualizations** notebook. Some visualizations created/analyzed are as follows:

* Summary statistics table
* Boxplot/outlier analysis
* 5 year trend of prices/interest rates
* Choropleth maps analyzing total number of sales/average sales by zip code
* Scatter plots analyzing size of home versus sale prices
* Pie charts comparing prices based on age of home

All visualizations created within the notebook were stored in the *output* folder.


