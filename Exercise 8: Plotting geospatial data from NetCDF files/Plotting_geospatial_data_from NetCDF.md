# Exercise 8: More on netCDF4 and plotting geospatial data with imshow()

In today's class we're going to learn more about the netCDF4 library and how to access information from netcdf files. We're also going to take a mini detour to learn about dictionaries. Finally, we'll learn how to make quick plots of geospatial data using the matplotlib function imshow(). First, we will go through the class notes together. You can find the powerpoint slides for the class in this "Exercise 8" folder.

## In-class exercise: Part A
In our in-class exercise today, our objective is to do a quick exploratory plotting data analysis to see how GPP changes over the year. *How might we do this?*

To complete the task, set out the steps below in a Jupyter Notebook (with comments for each task!):  
* Download data
* Import all relevant libraries, including matplotlib for plotting
* Open the netcdf file
* Read in the GPP data
* Close the netcdf file
* Create a loop over and plot each of the the first 12 months of the data and within that loop use imshow to plot each month.
* Answer the questions in the instructions on the Github page.

When you have completed the programming task, answer the following questions below:
1. How does the GPP of the tropical regions change over the course of the year?
2. How does the GPP in the northern hemisphere change over the course of the year?
3. Bonus question: why do you think there is a difference in how much change occurs in the tropics and in the northern hemisphere? [Hint: think what GPP is representing - the uptake of CO2 by plants]

**That's it for today. However, do not hand in this assignment. You will complete Part B of this in-class exercise on Wednesday before you hand it in.**

## In-class exercise: Part B
In the second part of the in-class exercise the task is to complete the following steps:
* Calculate the mean GPP over time
* Plot the mean temporal GPP and add a colorbar and a plot title.
* Then save the new mean GPP array to a netcdf file following the notes in class.

**Once you have completed this task, upload both Parts A and B to Canvas before the start of next class**
