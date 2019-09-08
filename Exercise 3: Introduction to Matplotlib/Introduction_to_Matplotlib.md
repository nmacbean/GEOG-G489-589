# Exercise 3: Introduction to Matplotlib and more in-depth NumPy

In today's class we're first going to go into a bit more depth on the NumPy package. Then we'll learn some of the basic plotting commands for data visualization in Python's Matplotlib plotting library

You can find out more about Matplotlib here: https://matplotlib.org

First, we will go through the class notes together. You can find the powerpoint slides for the class in this "Exercise 3" folder.

## In-class exercise
Our in-class exercise today is to complete the following in a Jupyter Notebook (with comments for each task!):  
* Load a file called “CO2_emissions_Americas_1960-2017_nopound.txt”. 
* Use slicing and indexing to separate out the country names (headers) from the 1st row. 
* Use slicing and indexing to separate out the years. 
* Use slicing and indexing to separate out the CO2 data for all countries across the Americas.  
* Explore your data! E.g:  
  * Print out the array that contains your country names to see which countries are there and how they are spelt etc.  
  * Print the first 10-20 rows of the CO2 data for your chosen countries to see if there are any missing data – if so, set them to np.nan.  
* Plot the 1960 – 2017 time series of CO2 emissions for 1 North American country, 1 Central American country and one South American country on the same plot with a legend! Change colors if you would like.  
* **--> How will you find the column index for each country?**. 
* Give the plot axis labels and a title.  
* *Don’t forget to use comments for each separate bit of code!*

&nbsp;
&nbsp;

### EXTRA if you’re familiar with python or if you’re finding this too easy!
* Google pyplot.bar() to see how to plot a bar plot in Matplotlib
* Plot a bar plot for the 2017 (last year in the file) CO2 emissions of the first 10 countries in the file.
* Change the xtick labels to the 10 country names.
* Give the plot axis labels and a title.

* *Question: which country from the list of the 1st 10 countries had the highest CO2 emissions in 2017?*


&nbsp;
&nbsp;

**As you did for Exercise 2, complete this exercise in a Jupyter Notebook with the title "*Your_Name* Exercise 3". Upload the jupyter notebook to Canvas by the beginning of next class - Wednesday 11th September at 1pm.** 

**Good luck and feel free to ask me any questions or to work with others!**

