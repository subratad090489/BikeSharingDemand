# Project Name
> This is a assignment where we built a multiple linear regression model for the prediction of demand for shared bikes.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)
* [Contributors](#contributors)


## General Information
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.


A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 


In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 



## Conclusions
- 
R- Sqaured train:  0.8   Adj. R-Squared train: 0.792
R- Sqaured test :  0.79   Adj. R-Squared test : 0.778

Coefficent for the variables are:
const                                                                                           0.051
yr                                                                                              0.256
holiday                                                                                        -0.088
temp                                                                                            0.581
windspeed                                                                                      -0.139
season_winter                                                                                   0.142
mnth_mar                                                                                        0.070
mnth_apr                                                                                        0.106
mnth_may                                                                                        0.086
mnth_jun                                                                                        0.056
mnth_sep                                                                                        0.080
weathersit_Light_Snow, Light_Rain_Thunderstorm_Scattered clouds, Light_Rain_Scattered_clouds   -0.226
dtype: float64


- From R-Sqaured and adj R-Sqaured value of both train and test dataset we could conclude that the above variables can well explain more than 80% of bike demand. Coeffiencients of the variables explains the factors effecting the bike demand

Based on final model top three features contributing significantly towards explaining the demand are:

Temperature (0.581) weathersit_Light_Snow, Light_Rain_Thunderstorm_Scattered clouds, Light_Rain_Scattered_clouds (-0.226) year (0.256) So it recomended to give these variables utmost importance while planning to achieve maximum demand.

- The equation of our best fitted line is:

𝑐𝑛𝑡=0.051+(0.256×𝑦𝑟)-(0.088×ℎ𝑜𝑙𝑖𝑑𝑎𝑦)+(0.581×𝑡𝑒𝑚𝑝)−(0.139×𝑤𝑖𝑛𝑑𝑠𝑝𝑒𝑒𝑑)+(0.142×season_winter)+(0.070×mnth_mar)+(0.106* mnth_mar)+ (0.086xmnth_may)+(0.056*mnth_jun)+(0.080xmnth_sep)−(0.226xweathersit_Light_Snow, Light_Rain_Thunderstorm_Scattered clouds, Light_Rain_Scattered_clouds)




## Technologies Used
- library - Python 3.0
- library - numpy 1.24.3, pandas 1.5.3 
- library - statsmodels 0.14.0, seaborn 0.12.2



## Acknowledgements
Give credit here.
- This project was inspired by... US bike-sharing provider BoomBikes
- References if any... https://ml-course2-upgrad.s3.amazonaws.com/Linear+Regression+Assignment/Bike+Sharing+Assignment/day.csv
- This project was based on [this tutorial]().


## Contact
Created by [@githubusername] - feel free to contact me!

## Contributors
Subrata Das
Developed as part of the Multiple Linear regression assignment required for Post Graduate Diploma in Machine Learning and AI - IIIT,Bangalore.

