# Oil Field Development Project

## Project Description

You work for OilyGiant, an oil extraction company. Your task is to find the best locations to open 200 new oil wells.

To complete this task, you will need to perform the following steps:

1.  Read the files with parameters collected from oil wells in the selected region: crude oil quality and reserve volume.
2.  Create a model to predict the reserve volume in new wells.
3.  Choose the oil wells that have the highest estimated values.
4.  Choose the region with the highest total profit for the selected oil wells.

You have data on crude oil samples from three regions. The parameters of each oil well in the region are already known. Create a model that helps choose the region with the highest profit margin. Analyze potential profits and risks using the bootstrapping technique.

### Conditions:

* Only linear regression should be used for model training.
* When exploring the region, a study of 500 points is carried out with the selection of the best 200 points for profit calculation.
* The budget for the development of 200 oil wells is $100 million.
* A barrel of raw material generates $4.5 in revenue. The income from a unit of product is $4500 (the reserve volume is expressed in thousands of barrels).
* After risk assessment, keep only the regions with a loss risk of less than 2.5%. Of those that meet the criteria, the region with the highest average profit should be selected.
* The data is synthetic: contract details and well characteristics are not disclosed.

### Data Description

Geological exploration data from the three regions are stored in files:

* `geo_data_0.csv`
* `geo_data_1.csv`
* `geo_data_2.csv`

Data columns:

* `id` — unique oil well identifier
* `f0`, `f1`, `f2` — three point characteristics (their specific meaning is not important, but the characteristics themselves are significant)
* `product` — reserve volume in the oil well (thousands of barrels).
