# Exercise 4: Introduction to Pandas

In today's class we're first going to go have a first look at the Pandas Python Data Analysis package: https://pandas.pydata.org

Pandas has its own data structures called data frames, which we will look at today. It is built on the NumPy package, but is higher level data manipulation. In particular, it is useful for dealing with tabular data - especially datasets that contain a mix of datasets - e.g. numerical, categorical and string data. 

First, we will go through the class notes together. You can find the powerpoint slides for the class in this "Exercise 4" folder.

## In-class exercise
Our in-class exercise today is to complete the following in a Jupyter Notebook (with comments for each task!):  
* First, download data.zip and unzip it in your downloads folder. Inside you will find the file: FLUXNET_US-Srm_Daily_1989-2014.csv file that we have been looking at in class.  
* Load pandas. 
* Open the US-Srm .csv file and save to a variable (e.g. data_df, but it can be called anything). 
* Query what’s in the file and answer these questions in a markdown box in your Jupyter Notebook:
  * What are the column headings?
  * How many data points are there in each column?
  * What is the data type and is it the same in all columns?
* Print out the 1st 5 lines of the “TA” (daily air temp) column using both methods we have learned
* We have TA_DAY and TA_NIGHT as two columns representing day and nighttime temperature. **What plot would we use if we wanted to plot both curves on the same plot for the 1st year of data (hint: from the filename we know this is daily data)?** 
* Plot this plot, with a legend, labels and a title
* **What type of plot would we need if we wanted to see the relationship between “TA” (daily air temp.) and “VPD” (vapor pressure deficit)?**
* Plot this plot with labels and a title


### EXTRA if you’re familiar with python or if you’re finding this too easy!
* Replot the plot you have just created, but change the size of the markers to be smaller and add a fine lined marker edge with a black edgecolor.
* *What do you notice about the patterns in the data when you make the marker size smaller?*


**That's it, you're finished! Remember to upload your .ipynb jupyter notebook to Canvas by the start of next class.**
