# Exercise 13: Performing statistical analyses on global geospatial datasets.

In today's class we'll briefly go over for loops again and learn about if statements (see powerpoint slides). We will then carry out an in-class exericse to perform a linear regression to determine if there's a trend in the GPP monthly data over time. To achieve this, you will use any of the statistical analysis tools we learned the other day to determine the slope of the relationship between monthly GPP (y) and time (X) for every land surface grid cell using for loops to loop over each row and column. The GPP data are the same data you have used in previous exericses "orch_gpp_monthly_2007-2011.nc".

We will consider how to do this calculation in a more efficient way in a future class, but for now you're going to carry out this task for every land surface grid cell using for loops.

Think through the steps needed to carry out this task from the very first step of importing the libraries and write your algorithm step by step. Some tips:
* You will create nested for loops to loop over both the rows and columns of the data.
* You will need to create an array outside the loop in which you can save the slope information within the loop.
* You will need to consider the fact that the ocean grid cells are masked and ignore them (i.e. do not perform the statistical analysis for these pixels) [Hint: look up masked array functions for how you can check ***if*** a grid cell is masked].

Once you have written out the logic of your algorithm for this assignment, write the code in a jupyter notebook.

When you have finished performing the statistical analysis for every land grid cell, plot your results using imshow() (or using the geographic mapping functions in Cartopy if you wish) and add a colorbar and title. Remember to save your jupyter notebook with the figure before submitting to Canvas.

**The deadline for this in-class exericse in Sunday 27th October at 11:59pm.**

*If you are very familiar with Python and complete the task quickly, investigate/search for how you might perform this analysis without using for loops in this way. You may add anything you test to your Jupyter Notebook with your submission.*
