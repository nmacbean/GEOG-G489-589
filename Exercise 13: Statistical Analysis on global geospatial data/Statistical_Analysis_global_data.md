# Exercise 13: Performing statistical analyses on global geospatial datasets.

In today's class we'll briefly go over for loops again and learn about if statements (see powerpoint slides). We will then carry out an in-class exericse to perform a linear regression to determine if there's a trend in the GPP monthly data over time. To achieve this, you will use any of the statistical analysis tools we learned the other day to determine the slope of the relationship between monthly GPP (y) and time (X) for every land surface grid cell using for loops to loop over each row and column.

We will consider how to do this calculation in a more efficient way in a future class, but for now you're going to carry out this task for every land surface grid cell using for loops.

Your first task is to think through the steps needed to carry out this task from the very first step of importing the libraries. Some tips:
* You will create nested for loops to loop over both the rows and columns of the data.
* You will need to create an array outside the loop in which you can save the slope information within the loop.
* You will need to consider the fact that the ocean grid cells are masked and ignore them (i.e. do not perform the statistical analysis for these pixels) [Hint: look up masked array functions for how you can check **if** a grid cell is masked].



