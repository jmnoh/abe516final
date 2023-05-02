

ABE516 Final Project


## Research Backround

Tillage operation play a crucial role in **seedbed** preaparation and crop yield. It affects the many aspects in initial condition for crop growth such as enhancing soil aeration and allowing good seed-to-soil contact which facilitater tbe seed germination and emergence. This research is focused on the objective of measuring the seedbed profile with the Lidar sensor to validate it's performance on evaluating seedbed quality. It is more a concept of testing, validation and developing a method for seedbad management.

## Problem

Newer tillage technology and embedded softwarehave been developed to monitor and adjust a fieldcultivator sweep's vertical position in real-time, allowing farmers to optimize the agronomic seed-bed environment. The current tool position and control feedback architect lack sensing of the soil-tilth quality for creating an optimal seed-bedenvironment. Methods are needed to determine soil tilth quality in field conditions and the tool's existing lifecycle, which could then be integrated into the tool's control feedback(software).

## Interesting question

*  1. What is the effect of the two treatments (new coated sweep and worn sweep) on the soil profile (making seedbed), as measured by the lidar sensor? 
*  2. A simple observation if the plant heights are different from two tillage treatments.


## Data description
Lidar data excel file, First of all, was derived from the LiDAR software and then useful data was selected and calculated mean, min, max and roughness value from each observations by matlab. After that, plant heights and vegetative stage was added for the project.

## Methods
In this project, it is more focused on the LIDAR data not on the plant height or vegetative stage.
* 1. Load the data, checking Missing values, correlation, and mean differences for each treatment
* Using Bootstrap and permutation
  * Check distribution type
  *Bootstrap and permutation
  *P-value, to check significant differences
  *Repeat the method to see the different results
    *Average soil depth in all runs, New vs Worn
    *Average soil depth in adjacent rows as pair, New vs Worn
    *Average soil depth in adjacent rows at the same subplot, New vs Worn

## Results and future work
* Bootstrap and permutation method didn’t work on the combined mean differences in New and Worn treatment (accepting the null hypothesis), but it was more effective when the data was separated into the precise region of the field.
* It also allows me to see the confidence intervals easily which helps to understand the lidar data.
* 2 out of 3 pairs of adjacent rows testing showed significant differences between treatments.
* Applying the same method by separating them with adjacent rows and subplots can be done in further process in the future.
* Through this project, I learned a lot in coding and found out the coding methods and visuals help me a lot to understand the data and propose another idea how to analyze data. For the question that I had before the project was answered since it showed some proof that It can differentiate the two treatments.
 
Thank you.
