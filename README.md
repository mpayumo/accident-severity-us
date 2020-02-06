# Determining Severity of Vehicle Collisions in the U.S.

> by: [:globe_with_meridians: Mark Payumo](https://www.linkedin.com/in/markpayumo/)

Exploratory data analysis and machine learning model development of nationwide dataset on U.S. car accidents.

## Description

![Road accident in Florida](img/FHP_in_Traffic_Accident.jpg "Florida road accident: Daniel Oines via Wikimedia Commons")

The **goal of this project** is to investigate trends in U.S. car accidents and use it to develop a machine learning regression model that will predict the likely severity of collision if it were to occur in a particular city. The severity is quantified within a range of **1 to 4** (1 being the least severe or least impact).

## Data Source

The dataset is a nationwide traffic accident record of 49 U.S. states between Feb. 2016 to Dec. 2019. It was obtained from Sobhan Moosavi, Srinivasan Parthasarathy, Mohammad Hossein Samavatian, Rajiv Ramnath, researchers from Ohio State University who wrote a [paper](https://arxiv.org/pdf/1906.05409.pdf) describing vehicle accidents in the country under a grant from the Ohio Supercomputer Center. The researchers purposely released the dataset to the public in order to democratize its utility for machine learning model development by interested individuals. It contains 49 features and 2,974,335 data points. You can find it [here](https://smoosavi.org/datasets/us_accidents).

## Exploratory Data Analysis


### U.S. Vehicular Accidents by State

<p align="center"><img src="img/accidentsUS.jpg"></p

![Frequency distribution by state](img/Frequency_dist_by_state.jpg "Frequency Distribution of U.S. Accidents by State")

---

### Severity 

Vehicular accidents usually imposed "manageable" delay upon commuters during the specified time period with Class 2 Severity occuring the most nationwide.

![Severity frequency distribution](img/severity-dist.jpg "Frequency Distribution: Severity")

---

### Word Cloud: Make Your Voice Visually Heard

If cities had a way to make their voices heard, the respective sizes of their names would represent their share of the distribution upon the reader. Out of **11,507** U.S. cities, one can deduce which ones are most likely in need of attention.

<p align="center"><img src="img/wordcloud.jpg"></p>


### Top 20 Cities with Most Vehicular Accidents

![Top 20 Cities](img/topbar.jpg "Top 20 Cities with Most Vehicular Accidents")

---

### Day of Week

![Accidents of by day of week](img/dayofweek.jpg "U.S. Accidents by Day of Week")

---

### Weather Conditions

Contrary to what would otherwise be popular intuition, most accidents occur during "fair winds, clear skies, and following seas."

![Accidents in different weather conditions](img/weather.jpg "Accidents in Different Weather Conditions")

---
## Model Development

>### Narrowing down to California

A spike in vehicular accidents impacted commuters in California towards the end of 2019.

<p align="center"><img src="img/timeseries.jpg"></p>

---

###




## Conclusion




