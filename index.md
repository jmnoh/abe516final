

### ABE516 Final Project


## Research Backround

Tillage operation play a crucial role in **seedbed** preaparation and crop yield. It affects the many aspects in initial condition for crop growth such as enhancing soil aeration and allowing good seed-to-soil contact which facilitater the seed germination and emergence. This research is focused on the objective of measuring the seedbed profile with the Lidar sensor to validate it's performance on evaluating seedbed quality. It is more a concept of testing, validation and developing a method for seedbad management.

## Problem

Newer tillage technology and embedded software have been developed to monitor and adjust a field cultivator sweep's vertical position in real-time, allowing farmers to optimize the agronomic seed-bed environment. The current tool position and control feedback architect lack sensing of the soil-tilth quality for creating an optimal seed-bed environment. Methods are needed to determine soil tilth-quality in field conditions and the tool's existing lifecycle, which could then be integrated into the tool's control feedback(software).

## Interesting question

* 1. What is the effect of the two treatments on the soil profile (making seedbed), as measured by the lidar sensor? 
* 2. A simple observation if the plant heights are different from two tillage treatments.


## Data description
Lidar data excel file, First of all, was derived from the LiDAR software and then useful data was selected and calculated mean, min, max and roughness value from each observations by matlab. After that, plant heights and vegetative stage was added for the project. Data structure : 108 rows and 12 columns.

## Methods
In this project, it is more focused on the LIDAR data not on the plant height or vegetative stage.
* Simple analysis : Load the data, checking Missing values, correlation, and mean differences for each treatment
* Principal component analysis
* Linear regression
  * mean soil depth vs plant height(measured after planting)
* Using Bootstrap and permutation
  * Check distribution type
  * Bootstrap and permutation
  * Comparing P-value, to check significant differences
  * Repeat the method to see the different results
    * Average soil depth in all runs, comparing Two treatments
    * Average soil depth in adjacent rows as pair, comparing Two treatments
    * Average soil depth in adjacent rows at the same subplot, comparing Two treatments (just a one experimental trial)

## Results & Discussion and future work
* For this Project, Data wrangling, PCA, Linear regression, bootstrap and permutation method was used for the analaysis.
* There were no missing values in the data and location information columns(trt-treatment, trtwrun-treatment with run and subplot) wer added for the analysis.
* Principal component analysis was not effective to identify cluster of two treatments by mean soil depth.
* Linear regression between mean soil depth and plant height deosn't show the linear relationship with the R-square value: 0.022 and p-value: 0.12.
* Bootstrap and permutation method didn’t work on the combined mean differences in treatments (accepting the null hypothesis), but it was more effective when the data was separated into the precise region (adjacent rows) of the field.
* It also allows me to see the confidence intervals easily which helps to understand the lidar data.
* 2 out of 3 pairs of **adjacent rows** testing showed significant differences( p-value < 0.05) between treatments.
* Applying the same method by separating them with **adjacent rows and subplots** can be done in further process in the future.
* Through this project, I learned a lot in coding and found out the coding methods and visuals help me a lot to understand the data and propose another idea how to analyze data. For the question that I had before the project was answered since it showed some result that It can differentiate the two treatments in p-value. However, this research is still in progress so further studies should be needed to develop the method how to analyze the lidar data and the crop plant data such as plant height, spacing, vegetative stage and yield .
 
Thank you.
