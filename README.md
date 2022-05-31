# NBA-Players-Seasons-2021-22
An analysis of NBA players in the 2021/2022 season

This project will rely heavily in the use of API as data sources. Contrary to most machine learning challenges and competitions, working in the industry usually requires the ML Developer to work with multiple teams and use heterogeneous sources of information to get the necessary data to solve a particular problem. Access to data is often provided through application programming interfaces (APIs), whether internal or external to the organization. It is very important to understand how to interact with APIs to collect data in our day to day work.

You might be wondering: why basketball? The main reason is availability of data.

The sport is played at a fast pace, with hundreds of plays in each single game, thousands of games in a season, and with a relatively small amount of on-court players, which gives them a lot of interactions with the ball, which in turn provides an oportunity to collect a great amount of data about each player performance.

These are the objectives of the project:

Understanding how to query an API to create a dataset with Python and Pandas
Learning how to cleanup a dataset and generate new fields from calculated data
Storing the created dataset in a serialized manner
Generating statistics about the data
Visualizing data
Introduction
A brief description of basketball and the NBA
The National Basketball Association is the main basketball league in the United States of America. It currently features 30 teams from different cities, divided in 2 conferences (East and West) of 15 teams. Each team plays a total of 82 games during the regular season. After that, the 8 teams with better records from each conference are seeded in a playoff format, with the winner of each conference playing the finals to determine the eventual champion. NBA seasons usually play out between october of one year, to june of the next year, so for example the current season being played is called the 2021/2022 season.

As in most leagues in the world, the game is played 5 vs 5 players, with as many as 9 reserve players that can rotate with the starters as many times as the team wants. Games are played to 48 minutes, so the total amount of minutes of combined play time for any team in a single game with no added time is 240 minutes. If the score is tied at the end of the 48 minutes, 5 minutes of extra time are played, this continues until a winner is decided.

Even though they can play multiple positions, players are usually classified according to the following positions:

Guards
Point Guards
Shooting Guards
Forwards
Small Forwards
Power Forwards
Centers
We will mainly focus on the three main positions: Guards/Forwards/Centers

The dataset
You'll be in charge of creating our dataset. We want to create a single pandas dataframe with information about all active players in the current NBA season. The dataset needs to have the following structure:

Personal Information
player_id (int) (INDEX)
player_name (str)
team_name (str)
position (str)
height (int) (in centimeters)
weight (float) (in kilograms)
country of origin (str)
date_of_birth (datetime)
age (str) (years and months)
years_of_experience (int) (years since entering the league)
Draft position (int)
Player career statistics
games played (int)
minutes per game (float)
points per game (float)
rebounds per game (float)
assists per game (float)
steals per game (float)
blocks per game (float)
Misc
salary in dollars (int) (contract value for this season only)
next_game_date (datetime)
