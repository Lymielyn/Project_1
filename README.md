# Project 1 - King County Sales dataset


## Questions:

1) What are the factors affecting price?
2) Which is the most prominent factor?
3) How our recommendations might look like?

## Names, delegation:

Ly Nguyenova - cleaning data, visualisation, models 
Stuti Singh - cleaning data, visualisation, models

We did not specify the delegation of tasks as we both wanted to be familiar with the dataset so we both cleaned the data, plotted visualisation, build our own models and at the end, we compared and merged our findings together.

## Overview:

As a newcomer to the King County Housing Market, our client wanted to know more about housing price in this area. As we are two freelance data scientists hired by the agency, our task was to find out the factors affecting price the most and to come up with a model that would be able to predict the price for the future. The client has handed over a dataset of the current housing market in the County. Based on this dataset, we have examined the variables that might have impact on price and have figured out the most prominent ones which will be presented in our deliverables. 

The dataset is comprised of information about the current price offered on the market. Furthermore, it has data about the size, location, number of bedrooms and bathrooms of the houses in the County. There are more aggregate data created based on the density of population in the area. Those are also taken into consideration.

## Dataset

kc_house_dataset.csv - King County Sales dataset

## Deliverables

- jupyter notebook
- presentation pdf

## Libraries 

We have used these libraries including Python to examine the dataset:

- Pandas
- Numpy
- Matplotlib Pyplot
- Seaborn
- Statsmodel
- Scikit.learn
- Scipy
- Folium

## Methodology and findings

### Goal 
Goal of my project is to predict price of house by utilising other variables available in dataset and find out how many variable are strongly corelated with price. We were also analysing how strongly they correlate with each other and which variable is playing most important role in prediction of price.

Our first step was to clean the data:
            
            (a)Missing Values- if some of your data is missing, the data set can lose expressiveness, which can lead to weak or                biased analyses
            (b)Outliers - your data might also contain values that diverge heavily from the big majority of your other data
            (c)checking for extraneous values
            
            -->>EDA(generate hypotheses for further analysis)
            (a)added two new columns as yr_of_sale and age_of_house(for more understanding with data to check if age of house is                also affecting its price)
            (b)describing data
            (c) features selection(finding corelation and data visualization)
            
            --->>Modeling
            (a)simple linear regression
            (b)multiple linear regression, comparsion of diifferent models based on r2

This methodology has resulted in findings of living area square footage, living area square footage for 15 neighbors and grade are the most powerful factors. Even though they will not have a huge impact on price like grades, they belong to to most prominent factor of price. As living area square footage is bigger, the price of the houses will also be higher. 

Meanwhile, location also has a big impact on price as the closer to the center(Seattle) a house is located, the higher price should be offered. Houses with waterfront are generally more expensive, however, due to the fact that there are very few of them waterfront does not belong to the list of factors strongly affecting price in the County. However, houses located near the coast cost more than other houses around them.

While it sounds quite obvious, houses with higher grades tend to cost more. Houses with grades from 0 to 2 would not sell well on the market as these grades will just decrease the price of the houses. From grade 3 houses will sell much better.

Houses with waterfront must be offered with higher price.

Prices for three-bedrooms-houses must be higher as they are in demand.
