<img src="https://studenthub.atu.ie/assets/ATU_Logo.fa93bf0a.svg" alt="ATU Logo" width="300" height="100">

This is the project for the 2024 Programming for Data Analytics (PFDA) module. A description of the project can be found [here](https://github.com/andrewbeattycourseware/PFDA-courseware/blob/main/labs/Project%20Description.pdf). 

Initially, I was going to do a project on aviation but struggled to find usable datasets that were free of charge. [Cirium.com](www.cirium.com), the world's most trusted source of aviation analytics for example provides top notch datasets, unfortunately none of them available for simple download. Same goes for [Iata](www.iata.org), International Air Transport Association or [CH-Aviation](https://www.ch-aviation.com), a subscription-based platform that provides accurate and reliable data and news on operators, aircraft, airports, and more. 

There are some aviation datasets available on [Kaggle](https://www.kaggle.com/) a brilliant platform for incipient data analysts but after all I decided to do the project on Irish weather data since we so often talk about the weather here in Ireland due to its erratic nature. As the saying goes: “If in the sky you see cliffs and towers, it won’t be long before there is a shower.” 

As of January 5, 2025, data for December 2024 was still unavailable. Consequently, I chose to exclude the entire year 2024 from the analysis to ensure the most accurate results by focusing exclusively on complete years.


Major key takeaways:

Windspeed vs. Rainfall:

The correlation coefficient of 0.47 indicates a moderate positive correlation windspeed and rainfall. This means as windspeed increases, rainfall also tends to increase but while while there is some degree of association between windspeed and rainfall, other factors likely influence the relationship as well. In this case a correlation of 0.47 suggests that higher windspeed tend to be somewhat associated with increased precipitation, but this is not a strong or definitive relationship.

Windspeed vs. Mean Temperature:

The correlation coefficient of -0.43 indicates a moderate negative correlation between windspeed and mean temperature. A negative correlation means that as one variable increases, the other tends to decrease or in other words, there’s an inverse relationship between the two variables. This value suggests that while there is a noticeable relationship, it is not particularly strong or perfectly linear. A correlation of -0.43 might imply that higher temperatures are generally associated with lower windspeed, but with some variability.

Rainfall vs. Mean Temperature:

The correlation coefficient of -0.13 indicates a very weak negative correlation between windspeed and mean temperature. Since the value of -0.13 is close to zero, it suggests that the relationship between the two variables is minimal or negligible what means that changes in one variable are not strongly associated with changes in the other. In this case it might imply a very slight tendency for higher rainfall to be associated with lower temperatures, but the effect is so weak that it may not be practically meaningful.




Regarding the code I have mostly refered to the documentation of the libraries used in the project as well as code we covered in this module's as well as previous module's lecture: 

https://github.com/andrewbeattycourseware/pands-course-material
https://github.com/andrewbeattycourseware/PFDA-courseware/tree/main

6.1: Combining PolynomialFeatures and LinearRegression into a single model:

https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.PolynomialFeatures.html
https://stackoverflow.com/questions/69443936/sklearn-pipeline-with-standardscaler-polynomialfeatures-and-regression



Additional sources I have used to complete the project and to back up my analysis:




https://www.twinkl.ie/blog/10-common-irish-weather-phrases

Met Éireann:

Annual Climate Statement 2018: https://cli.fusio.net/cli/bulletin/data/2018/17/sum_172018.pdf

Annual Climate Statement 2020: https://cli.fusio.net/cli/bulletin/data/2020/17/sum_172020.pdf


Annual weather summary 2015:

https://edepositireland.ie/bitstream/handle/2262/77499/clim-2015-ann.pdf?sequence=1&isAllowed=y


State of Climate 2019

https://www.met.ie/state-of-the-climate-2019
https://www.galway.pl/wp-content/uploads/2020/01/Met_Eireann_Weather_Summary__2019.pdf

Ireland’s future weather will be even warmer and wetter than predicted, scientists warn:

https://www.irishtimes.com/environment/climate-crisis/2025/01/03/ireland-will-be-warmer-and-wetter-than-predicted-due-to-climate-disruption-scientists-warn/

Predictions of Future Global Climate:

https://scied.ucar.edu/learning-zone/climate-change-impacts/predictions-future-global-climate

Earth shattered heat records in 2023 and 2024: is global warming speeding up?:

https://www.nature.com/articles/d41586-024-04242-z

The Beast from the East:

This day last year it was 18 degrees colder as Beast from the East struck

https://www.irishtimes.com/news/ireland/irish-news/this-day-last-year-it-was-18-degrees-colder-as-beast-from-the-east-struck-1.3809900

Storm Ellen:

https://www.met.ie/cms/assets/uploads/2020/08/StormEllen-003.pdf


The 'Beast from the East': Everything you need to know as Ireland prepares for Siberian freeze:

https://www.independent.ie/irish-news/the-beast-from-the-east-everything-you-need-to-know-as-ireland-prepares-for-siberian-freeze/36641136.html


Further readings on London climate:

Climate driven trends in London's urban heat island intensity reconstructed over 70 years using a generalized additive model

https://www.sciencedirect.com/science/article/pii/S2212095521002200

On the correlation coefficient:

https://statisticsbyjim.com/basics/correlations/

Regarding the code I have mostly refered to the documentation of the libraries used in the project as well as code we covered in this module's as well as previous module's lecture: 

https://github.com/andrewbeattycourseware/pands-course-material
https://github.com/andrewbeattycourseware/PFDA-courseware/tree/main



Additional sources:

https://www.geeksforgeeks.org/rainfall-prediction-using-machine-learning-python/




Athenry dataset: 

https://www.met.ie/climate/available-data/historical-data


London dataset: 

https://github.com/pc1991/London-Weather-Data-From-1979-To-2023/tree/main?tab=readme-ov-file:

Courtesy: Klein Tank, A.M.G. and Coauthors, 2002.

Daily dataset of 20th-century surface air temperature and precipitation series for the European Climate Assessment. International Journal of Climatology, 22, 1441-1453.

Data and metadata are available at http://www.ecad.eu.

London Weather Data From 1979 To 2023

Dataset Overview This dataset provides daily weather observations from Heathrow, United Kingdom (STAID: 1860), spanning the period from 1979 to 2023. The data is sourced from the European Climate Assessment & Dataset (ECA&D) and includes multiple weather parameters such as temperature, precipitation, sunshine, and more.



Pandas Cookbook: Recipes for Scientific Computing, Time Series Analysis and Data Visualization using Python Paperback – 24 Oct. 2017
by Theodore Petrou



