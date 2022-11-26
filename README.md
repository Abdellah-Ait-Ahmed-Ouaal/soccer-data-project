# Soccer Data Analysis
## by Abdellah Ait Ahmed Ouaal

## Dataset

The dataset we are going to use for analysis comes form four csv files attached with this project, Country ,Leagues ,Matchs and Teams all combined in one dataframe matches_df through many steps bellow, and in which we find :
11 european countries along with their 11 championship 
the names of all teams competitors for all 11 countries
the stage represents the order of the week (generally 34) in the year in which each team play one match
the date of each match of all seasons and the season (the year) from 2008 to 2016
the result of each match with the number of goals of both home and away team
All metionned datasets and more can be found in the original database [here](https://www.kaggle.com/datasets/hugomathien/soccer?resource=download)
## Summary of Findings and Insights

First we try to find the league/country that has the most goals in the first 3 stages of the season and for the first three season from 2008 to 2010, we used our cleaned dataframe matches_df after that we add a column containing the total number of goals, then we filter the dataframe using query method twice to get only desired stages and seasons, and as a final step we groupby league/country name and calculate the sum of total goals, just to find after checking that the England Premier League is the answer.

Second we want to know more about the evolution of the average goals scored in seasons : 2008/2009 , 2010/2011 and 2014/2015, so we take the first step which is groupby season and league name and calculating the mean for each season and each league, then we use the first function to plot horizontal bars with league names shown clearly for desired season, after we use a second function to plot line graphs to check more if the difference between leagues in term of average goals scored per season is becoming smaller, which means that the dispertion around the average of averages(for each league) is is decreasing ,and to verify that claim we calculate the standard deviation and we found that is true.