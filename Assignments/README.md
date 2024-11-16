# This is the repository for the weekly assignments for the Programming for Data Analytics module.
Assignment description copied from the course page: https://vlegalwaymayo.atu.ie/course/view.php?id=10462#section-2

## Assignment 1:

Create a repository for this module, and upload a link to where you will put your handups.

You have a Choice of the format of your repositories, Either:

- One repository with three folders (assignments, mywork, project). Make sure you submit a link to the appropriate folder.
- Three separate repositories (PFDA-assignments, PFDA-mywork, PFDA-project). Make sure you submit a link to the appropriate repository

Summary: tba
	
## Assignment 2 Weather:

- Task 1: Commit something to your assignment repository this week (anything)

- Task 2: I have put a CSV file in a assignment folder in the PFDA-courseware repository

Create a jupyter notebook called assignment2-weather.ipynb that has a nice plot of the temperature over time 

( "dryBulbTemperature_Celsius" ). 

Marks will be give for:

- Completing the assignment
- How nice the plot looks

You may use PANDAS if you wish to read in the data

Summary: tba

## Assignment 3 Domains:

Create a notebook called assignment03-pie.ipynb

The note book should have a nice pie chart of peoples email domains in the csv file at the url

https://drive.google.com/uc?id=1AWPf-pJodJKeHsARQK_RHiNsE8fjPCVK&export=download

This csv file has 1000 people. You may download the data or link to it.

Marks will be given for:

- Just creating the pie chart
- Making it look nice
- and as always a very small amount of marks will be given for just pushing something to your repository this week

As always your code should be well laid out.

Summary: tba

## Assignment 5 Risk:

Write a program (or notebook) called assignment_5_risk (.py or .ipynb)

The program should simulates 1000 individual battle rounds in Risk (3 attacker vs 2 defender) and plots the result.

One battle round is one shake of the attacker and defender dice.

I am being vague about what it plot, I will leave that to you.

For the last few marks.

A more complicated version simulates a full series of rounds for armies of arbitrary sizes, until one side is wiped out,

and plots the results.

(This is open ended, so it is only for the last few marks)

Rules of Risk

In Risk one army fights another. (using 6 sided dice)

In each battle round, the attacker can put forward up to three of their troops (3 dice).

The defender can use up to two of their defending troops (2 dice).

Each side looses troops depending on the following rules:

1. The two top dice dice are compared (ie the attackers top dice roll with the defenders top dice   roll) 
    - If the attackers dice is the same or lower they loose one troop otherwise the defender looses a troop (ie if the attackers dice is higher)
2. The next two highest dice from each side are then compared (ie the attackers second highest to the defenders second highest)
    - If the attackers dice is the same or lower they loose one troop otherwise the defender looses a troop (ie if the attackers dice is higher)

Summary: tba

https://matplotlib.org/stable/users/explain/animations/animations.html
https://stackoverflow.com/questions/72654607/userwarning-animation-was-deleted-without-rendering-anything

## Assignment 6 Knock airport Weather:

Create a python file or notebook called assignment_6_Weather (.py or .ipynb)

Get the data from this link.

https://cli.fusio.net/cli/climate_data/webdata/hly4935.csv

(This is different that the data I used in the lecture)

Plot:

- The temperature
- The mean temperature each day
- The mean temperature for each month

60% of the marks will be given for the above

For the last 40%

Plot:

- The Windspeed (there is data missing from this column)
- The rolling windspeed (say over 24 hours)
- The max windspeed for each day
- The monthly mean of the daily max windspeeds (yer I am being nasty here)

You do not need to over comment your code. Marks will be given for how nice the plots are.

Summary: tba

https://www.statology.org/seaborn-plot-multiple-lines/
https://www.dataquest.io/blog/tutorial-time-series-analysis-with-pandas/
https://stackoverflow.com/questions/21030171/how-get-monthly-mean-in-pandas-using-groupby
https://www.slingacademy.com/article/pandas-mastering-dataframe-groupby-method-8-examples/
https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.set_index.html
https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.T.html#pandas.DataFrame.T
https://stackoverflow.com/questions/20625582/how-to-deal-with-settingwithcopywarning-in-pandas
https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.gca.html

