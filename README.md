# BDAI-capstone_project-3

<img src="https://drive.google.com/uc?export=view&id=1Sv-Hu59Gngw4ai6ald6JiU5GYm0G-dye"/>

## :round_pushpin: Table of contents
> * [Table of contents](#)
> * [Vision 2030](#)
> * [About Dataset ](#)
> * [Business problem](#)
> * [EDA](#)
> * [Dashboard](#)
> * [Pig Latin](#)
> * [PySpark-MLClassification](#)
> * [Apache Kafka](#)
> * [Web blog](#black_small_squarereal-Web_blog)
> * [Team Memebers](#octocatteam-memebers)

## :green_circle:	 Vision 2030
Vision 2030 set ambitious goals for Saudi Arabia to achieve a qualitative leap in several areas and programmes, including:

The Quality of Life Programme, which is concerned with improving the quality of life of citizens, residents and visitors by supporting and developing new options, including the construction, development and maintenance of roads, and by supporting traffic systems and automated monitoring of violations.

## About Dataset
NYC Parking Tickets
It consists of 51 columns and 42.3M Rows 
from Aug 2013-June 2017   

### Columns:
> * Summons Number
> * Plate ID
> * Registration State
> * Plate Type
> * Issue Date
> * Violation Code
> * Vehicle Body Type
> * Vehicle Make
> * Issuing Agency
> * Street Code1
> * Street Code2
> * Street Code3
> * Vehicle Expiration Date
> * Violation Location
> * Violation Precinct
> * Issuer Precinct
> * Issuer Code
> * Issuer Command
> * Issuer Squad
> * Violation Time
> * Time First Observed
> * Violation County
> * Violation In Front Of Or Opposite
> * House Number
> * Street Name
> * Intersecting Street
> * Date First Observed
> * Law Section
> * Sub Division
> * Violation Legal Code
> * Days Parking In Effect
> * From Hours In Effect
> * To Hours In Effect
> * Vehicle Color
> * Unregistered Vehicle
> * Vehicle Year
> * Meter Number
> * Feet From Curb
> * Violation Post Code
> * Violation Description
> * No Standing or Stopping Violation
> * Hydrant Violation
> * Double Parking Violation
> * Latitude
> * Longitude
> * Community Board
> * Community Council
> * Census Tract
> * BIN
> * BBL
> * NTA

## Business problem

Therefore, we strive to achieve the objectives of the vision by addressing data from the automated monitoring of irregularities and developing new and intelligent solutions in line with the Kingdom's vision of digital transformation and achieving excellence.

##  :bar_chart:	EDA
> *  This plot shows the violation County with the number of tickets and the place where the ticket was issued (front, opposite). the higest County in Violation is NY and the Violation in all County is in front.
<img src="https://drive.google.com/uc?export=view&id=1DOltiwC5xQkwsEP07keTHE0gTW4Nmu7p"/>

> * This plot shows the 10 highest vehicle Make in the parking. As can be seen, Ford ranks first, followed by Toyota and Honda. 
<img src="https://drive.google.com/uc?export=view&id=1y13dsGnYWgHI_yJNq0EY46C9GfAYoEW9"/>


> * This plot shows the top 10 years by the percentage of tickets as you can see 2015 is the highest year then 2016.
<img src="https://drive.google.com/uc?export=view&id=1pwtH3GYQb31jMUQlyuyBt0fvbxDFz9SH"/>


> * This plot shows the 20 highest Violation times.  As you can see, all the times are in the morning. the highest one at 8:36 AM and the lowest at 8:42 AM, probably because it's work time for most people. As a plan of action, we can set up a system for people who want to book ahead of time and pay a higher price.
<img src="https://drive.google.com/uc?export=view&id=1xk6Oj1ruIx_u2brAcPRR1fsg_nncPV5o"/>


> * This plot shows the top 4 Plate Type and number of tickets. PAS is the highest then COM, OMT, OMS.
<img src="https://drive.google.com/uc?export=view&id=1gxcSHcfIxlZ0q4K4UoDrwvAbjVYQOGAR"/>


> * This plot shows the number of Violation Precinct, most Violation are between 20 to 90.
<img src="https://drive.google.com/uc?export=view&id=1D8V3gu12BJcGpwCKPobmCxk3JqBkIXnT"/>



> * This plot shows the top 10 violations by description and summons number. the highest Violation is 21 (No Parking). This might be due to the low cost of this violation, and to solve this problem, we recommend increasing the cost.
<img src="https://drive.google.com/uc?export=view&id=1g69_I_q-V-NE-KyyN9cg0AL8V1toJQQL"/>


> * This plot shows the violation of the place where the ticket was issued (front, opposite). front is the highest with 62.9%
Also, this is going to be our target column for the classification problem, and it has a skew class distribution, so we will deal with that with some techniques.
<img src="https://drive.google.com/uc?export=view&id=1mZiVa6rpL-ZaHYVbE9_PkoWgY2ly3myA"/>


> * This plot shows the issue date and number of tickets. In general, 2017 and 2016 are the highest years to issue tickets. In 2016, the 25th of November was the highest day for ticket sales, with over 7,500 issued.

<img src="https://drive.google.com/uc?export=view&id=1bd7m6M1tPsfGGDSxEyVDHeWN6CtrHiwD"/>


> * This plot shows the top 10 vehicle models in 2015. We chose 2015 because it was the most successful year in terms of ticket sales. the highest Make was Toyot with more than 16,000 Tickets.
<img src="https://drive.google.com/uc?export=view&id=1FI7J-JS-UZLfa3tDRG7aEE1jZf21IfbF"/>

## Dashboard

<img src="https://drive.google.com/uc?export=view&id=1MUVellpzfRlPDMY9E6qvgOpBWIOiWp6D"/>

<img src="https://drive.google.com/uc?export=view&id=1mjmGKwge_sXDvskskAUUpC1j0L1syVw1"/>

## :black_small_square:	Web blog

## Pig Latin
>  we use Pig Latin to answer 20 interesting questions about our dataset 
> * Q1: What is the total number of violation tickets per year?
> * Q2: How much does a vehicle make have a number of parking violation tickets from highest to lowest?
> * Q3: Count of parking violation tickets per registration state?
> * Q4:  What is the total number of parking violation tickets for every vehicle description from lowest to highest.
> * Q5: What is the total number of parking violation tickets for Ford and Toyota?
> * Q6: What is the total number of parking violation tickets for every street name along with the violation code from highest to lowest?
> * Q7: What is the total number of parking violation tickets for NY and NJ Registration State?
> * Q8: What is the total number of violation tickets for every violation time along with whether the violation is in front or opposite from highest to lowest?
> * Q9: What is the total number of violation tickets for every violation time along with the violation description from highest to lowest?
> * Q10: Find the total number of parking violation tickets from    2013 to 2017.
> * Q11:  What is the top 20 of the total number of violation tickets for every plate type along with the violation description?
> * Q12:  What is the 5 highest total number of parking violation tickets for every vehicle make along with the violation precinct from highest to lowest? 
> * Q13:  What is the total number of parking violation tickets for vehicles ending up with expiration before 2018?
> * Q14: What is the total number of parking violation tickets for each vehicle make from highest to lowest.
> * Q15: What is the total number of parking violation tickets for every registration state along with the sub-division from highest to lowest?
> * Q16: What is the total number of parking violation tickets for the Registration States TX and OH?
> * Q17: What are the minimum and the maximum vehicle year that get a parking violation ticket in the BX violation county?
> * Q18: What is the top 10  total number of parking violation tickets for every issuer squad from highest to lowest?
> * Q19: What is the top 5 total number of parking violation tickets per vehicle color from highest to lowest?
> * Q20: What are the top 10 highest total number of parking violation tickets for every vehicle make along with the violation description?


## PySpark-MLClassification



## Apache Kafka


## :octocat:	Team Memebers

- [Abdullah Huwaishel](https://github.com/hush966)
- [Afnan Alzahrani](https://github.com/AfnanAlzahrani)
- [Jumana Almussa](https://github.com/jumana0)
- [Mahmuod Alhassan](https://github.com/alhassanm)
- [Amjad Almusallam](https://github.com/ASM650)



# SDA - CodingDojo - Vision 2030 - 

