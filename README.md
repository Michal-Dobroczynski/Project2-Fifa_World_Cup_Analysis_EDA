# Project2-Fifa_World_Cup_Analysis_EDA
Exploratory Data Analysis on 2 datasets of Fifa World Cup tournament. </br>

## Table of content:
- Introduction of Fifa World Cup
- Data Summary
- Exploratory Data analysis
- Dashboards

## Introduction of Fifa World Cup: 

The FIFA World Cup, often simply called the World Cup, is an international association football competition contested by the senior men's national teams of the members of the Fédération Internationale de Football Association (FIFA), the sport's global governing body. 

It is contested every four years and is the most prestigious and important trophy in the sport of football, as well as the most widely viewed and followed single sporting event in the world. 

As of the 2018 FIFA World Cup, 21 final tournaments have been held. The trophy has been won by eight national teams. Brazil, with five wins, are the only team to have played in every tournament. The other World Cup winners are Germany and Italy, with four titles each; Argentina, with two titles; France and inaugural winner Uruguay, each with two titles; and England and Spain, with one title each.

## Data Summary

Take a look at my dashboard for World Cup Statistics. 

Tools/programs used: 
- Excel + Power Query 
- Power BI

Date of project: 09.03.2023
Source: https://www.kaggle.com/datasets/evangower/fifa-world-cup

Datasets cover summary of each World Cup held and every single World Cup match played in its history from Uruguay in 1930 to Russia in 2018.

**Dataset wcmatches** </br>
This dataset has 900 observations in it, with 15 columns mixed between categorical and numerical values. 
Example of data: Columns inside the dataset include year, country, city for the match being played in, outcome which team claimed victory or did the match result in a draw, score of the match (home_team and away_team vs home_score vs away_score and many more interesting data.

**Dataset worldcups** </br>
This dataset includes 21 observations, with 10 columns mixed between categorical and numerical values.
Example of data: contains information about winners, second, third, fourth places, goals scored and attendance per tournament and many more.

**Wcmatches**

![wc_matches](https://user-images.githubusercontent.com/127090462/224045218-956f21ca-d3e6-46e5-82c4-8fed629aa718.JPG)


**World_cups**

![world_cups](https://user-images.githubusercontent.com/127090462/224045230-e65c1492-794c-49c9-b49a-6b4b2329c3f0.JPG)

## Exploratory Data Analysis (EDA)

Exploratory data analysis (EDA) is used by data scientists to analyze and investigate data sets and summarize their main characteristics, often employing data visualization methods. It helps determine how best to manipulate data sources to get the answers you need, making it easier for data scientists to discover patterns, spot anomalies, test a hypothesis, or check assumptions. </br>
Source: https://www.ibm.com/topics/exploratory-data-analysis


**Used steps in the process of EDA**

- Acquiring and loading data (.csv files)
- Understanding datasets and variables (categorical and numerical)
- Cleaning/Transforming dataset (Excel + Power Query)
- Data analytics and Visualizing Data (Power BI)

**Steps of data cleaning/transformation done** (Excel, Power Query)

1. **Data cleaning**

- **Duplicates** - no duplicates found in datasets
- **Missing data** - null values, the only column (win_conditions) which has null values is in dataset - wcmatches. Anyway we can ignore that fact as it won't be analyzed, it is only informative column. We have got filled in only these fields when match ended in draw and it wasn’t the group stage of the tournament. For example, win in extra time (AET - after extra time), by penalties. 

![null](https://user-images.githubusercontent.com/127090462/224044712-e144e67a-d4a3-48c4-85a0-6936bd59d711.JPG)

- **Added new columns for analysis** </br>
 a) Continent -> vlookup/xlookup from Country </br>
 b) Goals per game/Attendance per game - Excel Calculations </br>

## Dashboards

I divided my analysis into 3 main dashboard </br>
1. **Fifa World Cup All Tournament Statistics**

General information about all World Cup Tournaments:
- Sum of scored goals - 2548 (distribution is diversified as first tournaments started with 18 games, nowadays it's 64 games)
- Avg goals per game - 2,83 goals
- List of Winners - Brazil has most wins so far - 5, there are only 8 unique champions (West Germany and Germany we can treat as 1 country)
- Hosts of tournament by continent - out of 21 tournaments, 11 were organized in Europe 

2. **Top teams performance**

Analysis of top teams which reached top 3 places:
- List of all countries which reached top 3 places at least once
- Germany played 8 times in final and won 4 times (50%), Brazil won 5 times playing 7 times in final 71,4%
- Uruguay, England and Spain have 100% winning ratio of finals

3. **Goals/matches statistics**
Analysis of goals, matches statistics
- Brazil is the only team which played in all 21 tournaments so far. 
- The best ratio of goals per game have Hungary - 2,72
- Germany played the most games in all tournaments - 115

**Graph charts used in analysis:**
- Stacked column chart
- Card
- Table
- Donut chart
- Clustered column chart
- Funnel

1. **Fifa World Cup All Tournament Statistics**

![Fifa_World_Cup_Statistics](https://user-images.githubusercontent.com/127090462/224049869-47ce54bc-0bea-4e0a-ba75-ddc3f3de1c03.JPG)

2. **Top teams performance**

![Top_teams](https://user-images.githubusercontent.com/127090462/224067623-408c7f54-6392-4b44-bcb7-e8c668d517c2.JPG)

3. **Goals/matches statistics**

![Goals_matches statistics](https://user-images.githubusercontent.com/127090462/224028140-0d515739-4456-4a39-a15c-3832e92d1c98.JPG)

