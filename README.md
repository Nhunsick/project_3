## Repository Structure 
```
├── Notebooks 
│   └── EDA.ipynb 
│   └── Final_Notebook.ipynb (models)
├── data
├── images
├── .gitignore
└── README.md
```
# 2018 House of Representatives Election Forecasts 

## Business Proposition
How well can we predict the outcome of the 2018 House of Representatives election?

## Data Sources
- 2018 MIT Election Data and Science Lab
- Dave Leip's Atlas of U.S. Elections, specifically the 2018 House of Representatives election 

## Results
Created a Margin of Victory(MOV) scale to determine how likely each political party will win a county 

MOV = the difference of the votes between the two major political parties then divided by the total votes

<img src='images/mov_scale.png' width='800' height='200'>

As you can see the distributions of the MOV of previous elections are right-skewed. 
<img src='images/pres_mov.png' width='800' height='400'>
<img src='images/house_mov.png' width='500' height='300'>

It may seem the Republican party is performing well in these elections, however, we need to consider population density.

Here, you can see the population distribution by size of each county. 

<img src='images/pop.png' width='400' height='400'>
The sizes of counties are much larger for Democrats than Republicans. 
County votes do not determine the actual winner of a congressional election, the district-wide votes do, and many small counties may be outvoted by one large county.

&nbsp;
## Model
We performed multiple model types such as Logistic Regression, Decision Trees, and K-nearest neighbors(KNN) in our analysis. 

With KNN, having the highest accuracy score of ~80%.

Here is the KNN Confusion Matrix:

<img src='images/confusion_matrix.png' width='400' height='400'>


## For More Information
See the full analysis in the Jupyter Notebook or review this presentation. For additional info, contact Noah Hunsicker or Julie Leung.
