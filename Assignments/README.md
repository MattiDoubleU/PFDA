# This is the repository for the weekly assignments for the Programming for Data Analytics module.
Assignment descriptions copied from the course page: https://vlegalwaymayo.atu.ie/course/view.php?id=10462#section-2.
Please note that the numbering differs from the course page.

## Assignment 1:

Create a repository for this module, and upload a link to where you will put your handups.

You have a Choice of the format of your repositories, Either:

- One repository with three folders (assignments, mywork, project). Make sure you submit a link to the appropriate folder.
- Three separate repositories (PFDA-assignments, PFDA-mywork, PFDA-project). Make sure you submit a link to the appropriate repository

Summary: I have opted for the first choice. Initially I was struggling with the creation of subfolders inside a Github repository since it isn't possible to commit an empty directory to git. The workaround was to create an empty .gitkeep file inside each of the three folders. Later during the semester I learned that the easiest way to create directories or subfolders inside Github repositories is via command line interface (bash terminal) in Linux VM in Github codespaces.

### References:

https://stackoverflow.com/questions/29249134/how-to-create-new-subfolder-in-git-repository
	
## Assignment 2 Weather:

- Task 1: Commit something to your assignment repository this week (anything).

- Task 2: I have put a CSV file in a assignment folder in the PFDA-courseware repository.

Create a jupyter notebook called assignment2-weather.ipynb that has a nice plot of the temperature over time.

( "dryBulbTemperature_Celsius" ). 

Marks will be give for:

- Completing the assignment
- How nice the plot looks

You may use PANDAS if you wish to read in the data.

Summary: I will skip Task 1 for obvious reasons and briefly summarize Task 2: I have indeed used PANDAS for this exercise; the function ```pd.read_csv()``` reads in a CSV file and load its contents into a two-dimensional, tabular data structure or DataFrame. PANDAS are a fantastic tool to combine with Matplotlib a library for plotting. I availed of two Matplotlib submodules, ```matplotlib.pyplot``` and ```matplotlib.dates``` to complete the task. The first used for creating visualizations such as plots or graphs whereas the former one is designed to handle date and time data in plots. If it wasn't for the date/time bit I had issues with at the beginning this exercise would have been fairly easy.  

### References:

https://stackoverflow.com/questions/36692861/avoiding-error-from-pd-to-datetime-in-pandas
https://matplotlib.org/stable/api/_as_gen/matplotlib.figure.Figure.autofmt_xdate.html
https://matplotlib.org/stable/api/_as_gen/matplotlib.axis.Axis.set_major_formatter.html

## Assignment 3 Domains:

Create a notebook called assignment03-pie.ipynb.

The note book should have a nice pie chart of peoples email domains in the csv file at the url

https://drive.google.com/uc?id=1AWPf-pJodJKeHsARQK_RHiNsE8fjPCVK&export=download.

This csv file has 1000 people. You may download the data or link to it.

Marks will be given for:

- Just creating the pie chart
- Making it look nice
- and as always a very small amount of marks will be given for just pushing something to your repository this week

As always your code should be well laid out.

Summary: Again PANDAS and Matplotlib were my go-to libraries for this assignment. It took me a bit of research to figure out how to extract and split the email addresses. A combination of the lambda function ```lambda x``` and split ```.split()``` was the solution: ```lambda x: x.split('@')[-1]``` splits the string x, the email address into a list of two parts using @ as the separator. [-1] Since there is only one element in the list following @.

### References:

https://www.geeksforgeeks.org/applying-lambda-functions-to-pandas-dataframe/
https://oregoom.com/en/python/lambda/
https://www.freecodecamp.org/news/how-to-split-a-string-in-python/
https://docs.python.org/3/tutorial/datastructures.html#more-on-lists
https://matplotlib.org/stable/gallery/pie_and_polar_charts/pie_features.html

## Assignment 5 Risk:

Write a program (or notebook) called assignment_5_risk (.py or .ipynb)

The program should simulates 1000 individual battle rounds in Risk (3 attacker vs 2 defender) and plots the result.

One battle round is one shake of the attacker and defender dice.

I am being vague about what it plot, I will leave that to you.

For the last few marks.

A more complicated version simulates a full series of rounds for armies of arbitrary sizes, until one side is wiped out,

and plots the results.

(This is open ended, so it is only for the last few marks).

Rules of Risk

In Risk one army fights another. (using 6 sided dice)

In each battle round, the attacker can put forward up to three of their troops (3 dice).

The defender can use up to two of their defending troops (2 dice).

Each side looses troops depending on the following rules:

1. The two top dice dice are compared (ie the attackers top dice roll with the defenders top dice roll) 
    - If the attackers dice is the same or lower they loose one troop otherwise the defender looses a troop (ie if the attackers dice is higher)
2. The next two highest dice from each side are then compared (ie the attackers second highest to the defenders second highest)
    - If the attackers dice is the same or lower they loose one troop otherwise the defender looses a troop (ie if the attackers dice is higher)

Summary: It was clear that I needed to use **functions**, **control flow**, **lists** and **for loops** for this task, yet it was challenging to make the program work. The Numpy library has proven to be the most useful for this assignment (addtionally to Matplotlib.Pyplot). ```np.random.randint()``` was first used to generate random numbers between 1 and 6 for the rolls of the attacker and the defender and second to stimulate a total of 1000 battle rounds that is to generate random numbers between 0 and 2 until a total of 1000 had been reached: ```np.random.randint(0, 3, 1000)```. Furthermore ```np.bincount(array, minlength=N)``` and ```numpy.arange()``` were indispensable to make the code work. The first function counts the occurrences of each integer in a 1D array and returns an array where the index corresponds to the value being counted, and the value at that index is the count, whereas the second one generates an array of evenly spaced values within a specified range (['0 losses', '1 loss', '2 losses']). As with the previous tasks, I had to tweak the outputs a bit to make the plots 'look nice.' However, for this one, I decided to animate the plot so that, as the battle rounds progress, the bars grow accordingly. I imported the FuncAnimation submodule from matplotlib.animation to achieve this, but unfortunately, I wasn't able to get it to work. It kept throwing an error no matter what troubleshooting steps I applied.

### References:

https://docs.python.org/3/tutorial/controlflow.html
https://matplotlib.org/stable/users/explain/animations/animations.html
https://stackoverflow.com/questions/72654607/userwarning-animation-was-deleted-without-rendering-anything
https://numpy.org/doc/stable/reference/generated/numpy.bincount.html
https://numpy.org/doc/stable/reference/generated/numpy.arange.html

## Assignment 6 Knock airport Weather:

Create a python file or notebook called assignment_6_Weather (.py or .ipynb).

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

Summary: For this assignment I used the Seaborn library which I haven't used for any of the previous assignments alongside PANDAS and Matplotlib. I have probably over complicated some of the code as I was trying to finish the task well ahead of time and before the lectures of that particular week. For this reason there are two type of plots, the ones that display each of the years in an individual color coded line and the ones with a single line and the dots or scatter plots with a linear regression line. I simply adapted the lecturer's code from the lab in week 7 for those. The key take away for this assignment was to learn about and correctly use ```df.groupby()``` a tool to calculate summary statistics like mean, sum, min, max, etc. ```df.dropna()``` was brought to use in the second part to rid the data set of any non numeric values and therefore allows for a clean data frame to work of. It is in my opinion one of the most useful and easy to use tools for data cleansing. Last but not least I was trying out different values and parameters to see what the plots would look like.

### References:

https://www.statology.org/seaborn-plot-multiple-lines/
https://www.dataquest.io/blog/tutorial-time-series-analysis-with-pandas/
https://stackoverflow.com/questions/21030171/how-get-monthly-mean-in-pandas-using-groupby
https://www.slingacademy.com/article/pandas-mastering-dataframe-groupby-method-8-examples/
https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.set_index.html
https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.T.html#pandas.DataFrame.T
https://stackoverflow.com/questions/20625582/how-to-deal-with-settingwithcopywarning-in-pandas
https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.gca.html

