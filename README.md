# Project-6--Covid-test

In this exercise, we will focus on visualizing covid-19 tests statistics in Switzerland. The goal of this exercise
is to display and link daily total tests numbers together with positive cases numbers in two plots, so that
when we dragging the shaded overlay in the second plot, the range of the first plot will be automatically
updated. You will get access to the online dataset from this link, (optionally, you can also use the provided
same data named “covid19_tests_switzerland_bag.csv") and the complete tasks are described below:

Task1: Data Preprocessing.
T1.1: Read the online data into a DataFrame using pandas.
T1.2: Construct a ColumnDataSource for plotting according to the task descriptions in the code
skeleton. (Be attention that the original data from the link has an error, the last column should be
frac_positive rather than frac_negative, the provided data has already correct it.)
T1.3: Define a colormap and map the range of positive rate to a colormap linearly.

Task2: Data Visualization.
T2.1: Covid-19 Total Tests Scatter Plot. In this first plot, you need to display the daily tests numbers
in a scatter plot, and add a hover tool to display the date and the corresponding total test number. In
the scatter plot, point size is fixed, point color is mapped to the positive rate from the data.
T2.2: Create a ColorBar using the colormap in T1.3 and attach this bar to the first plot.
T2.3: Covid-19 Positive Number Plot. The second plot consists of a basic line glyph that displays the
general trend of positive cases, and add a RangeTool, with which we can observe detailed scatter
points distribution in the first plot. Add a hover tool to display the date and the corresponding
positive number.
T2.4: Arrange two plots in one layout appropriately
