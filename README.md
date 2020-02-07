# Determining Severity of Vehicle Collisions in the U.S.

> by: [:globe_with_meridians: Mark Payumo](https://www.linkedin.com/in/markpayumo/)

Exploratory data analysis and machine learning model development of nationwide dataset on U.S. car accidents.

## Description

![Road accident in Florida](img/FHP_in_Traffic_Accident.jpg "Florida road accident: Daniel Oines via Wikimedia Commons")

The **goal of this project** is to investigate trends in U.S. car accidents and use it to develop a machine learning regression model that will predict the severity of collision if it were to occur in a particular city. Severity is defined within a range of integers, **1 to 4** and which represent the following:
<ul><li>1 - Short Delay</li>
    <li>2 - Manageable Delay</li>
    <li>3 - Extended Delay</li>
    <li>4 - Long Delay</li></ul>

## Data Source

The dataset is a nationwide traffic accident record of 49 U.S. states between Feb. 2016 to Dec. 2019. It was obtained from Sobhan Moosavi, Srinivasan Parthasarathy, Mohammad Hossein Samavatian, Rajiv Ramnath, researchers from Ohio State University who wrote a [paper](https://arxiv.org/pdf/1906.05409.pdf) describing vehicle accidents in the country under a grant from the Ohio Supercomputer Center. The researchers purposely released the dataset to the public in order to democratize its utility for machine learning model development by interested individuals. It contains 49 features and 2,974,335 data points. You can find it [here](https://smoosavi.org/datasets/us_accidents).

## Exploratory Data Analysis


### U.S. Vehicular Accidents by State

California stands out as having the most share of traffic accidents followed by Texas, Florida, South Carolina, North Carolina, and upstate New York. The heatmap and bar graph show the magnitude of the frequency distribution.

<p align="center"><img src="img/accidentsUS.jpg"></p

![Frequency distribution by state](img/Frequency_dist_by_state.jpg "Frequency Distribution of U.S. Accidents by State")

---

### Severity 

Vehicular accidents usually imposed "manageable" delay upon commuters during the specified time period with Class 2 Severity occuring the most nationwide.

![Severity frequency distribution](img/severity-dist.jpg "Frequency Distribution: Severity")

---

### Make Your Voice Visually Heard

If cities had a way to make their voices heard, the respective sizes of their names would represent their share of the distribution upon the reader. Out of **11,507** U.S. cities, one can deduce which ones are most likely in need of attention.

<p align="center"><img src="img/wordcloud.jpg"></p>


### Top 20 Cities with Most Vehicular Accidents

The frequency distribution below quantifies the word cloud above.

![Top 20 Cities](img/topbar.jpg "Top 20 Cities with Most Vehicular Accidents")

---

### Day of Week

More traffic accidents occur during the weekdays.

![Accidents of by day of week](img/dayofweek.jpg "U.S. Accidents by Day of Week")

---

### Weather Conditions

Contrary to what would otherwise be popular intuition, most accidents occur during "fair winds, clear skies, and following seas."

![Accidents in different weather conditions](img/weather.jpg "Accidents in Different Weather Conditions")

---
## Model Development

>### Narrowing down to California

### Time Series Analysis: Car Accidents in California

A spike in vehicular accidents impacted commuters in California towards the end of 2019.

<p align="center"><img src="img/timeseries.jpg"></p>

---

### Correlation Heatmap
>### Numerical features vis-á-vis Severity

Exploring how our features might satisfy the linearity assumption for linear regression, this heatmap shows five out of 96 features that have numerical values along with our target variable, "Severity." 

<p align="center"><img src="img/correlation.jpg"></p>

---

### Linear Regression
>### OLS (Ordinary Least Squares) Summary

The linear model performed poorly with an **adjusted R^2** of **0.085**. **Heteroscedascity** was also detected using the **Goldfeld-Quandt Test** with a **p-value** of <code>2.270459470776888e-10</code>.

<p align="center"><img src="img/linearsummary.jpg"></p>

### Random Forest Regression
>### Feature importances and an improved R^2

Random Forest Regression improved by twice the linear model with an **R^2 score** of <code>0.17945677024559692</code>. Feature importances are shown below that may provide for better modeling.

<p align="center"><img src="img/featureimp.jpg"></p>




## Future Direction




