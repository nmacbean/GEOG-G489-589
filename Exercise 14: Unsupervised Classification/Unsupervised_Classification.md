# Exericse 14: Unsupervised hyperspectral image classification

This week we will be learning about unsupervised learning using the KMeans Clustering analysis from scikit-learn (https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html). We will be applying this to classify hyperspectral imagery to determine fraction of land cover types (shrub, grass, bare soil) at the semi-arid Santa Rita site in southern Arizona.

In today's class our guest lecturer Rubaya Pervin will be talking through the methods as well as the data cleaning and tidying process.

In Wednesday's class we'll be doing an in-class exercise to practice the image classification using KMeans clustering.

Today's (Monday's) homework is to complete the DataCamp tutorial on "lustering for Dataset Exploration: (Chapter 1) of the Unsupervised Learning Module: https://www.datacamp.com/courses/unsupervised-learning-in-python. This will help you to become more familiar with the KMeans method before Wednesday's in-class exercise.

## In-class exercise: KMeans Clustering for unsupervised classification at the Santa Rita site

In today's exercise you will follow the classification steps taught in the lecture on Monday to classifiy hyperspectral dataset from a different part of the Santa Rita Experimental site. The photo below shows the camera image of area we'll be classifying.

![santa rita](2018_SRER_2_514000_3519000_image.png)

The data have already been cleaned following the steps described on Monday (removing missing and negative numbers, cleaning the bad/noisy bands of information). The cleaned data are in a file called "2018_SRER_2_514000_3519000_hyperspectral_cleaned.tif". Due to the size of the file, it is provided in this folder on box: 

As detailed in the lecture on Monday, there are three dimensions in the data corresponding to [nrows, ncols, nbands], where nbands is the number of (cleaned) hyperspectral bands.

Follow the steps below to complete the exercise and then answer the following questions. Look through the lecture notes from Monday to help you with the code. You may also want to look back to Exercise 10 on GDAL to help you with how the GDAL commands are structured

i. Open the file using the gdal open file command.  

ii. Then read in the array to the variable data with the gdal command ReadAsArray. 

iii. Reshape your data so they correspond to the dimensions we need for the sklearn KMeans clustering algorithm (slide 17 of the powerpoint).    

For this step, it would be useful to refer to the sklearn kmeans clustering method manual page (see above). If you scroll down to the methods "fit" and "fit_predict" you will see that the same of the array we give to the method (X on the manual page) needs to have the dimensions of "nsamples" and "nfeatures".  
Recall from what we have learned about Sklean so far that the nsamples is the number of observations we have of each "feature". The features are essentially the different types of information we will use to form the clusers.  
In this case, the features are the different hyperspectral bands containing reflectance information from different parts of the electromagnetic spectrum (read the links on hyperspectral data from the lecture if you would like to learn more).  
The nsamples are the information from both the rows and columns - therefore, we need to collapse the rows and columns from 2 dimensions into 1 dimension containing all the rows and columns (again, see slide 17 and the class on statistical analysis in Python for how to do this).  

iv. Now you have reshaped your data, you will be able to perform the KMeans clustering algorithm following the steps shown in slide 16 (also 18 and 19). Repeat the classification for 2, 3 and 4 clusters.  

v. Now plot your result using plt.imshow (see slide 20 of the lecture).  

vi. **Once you have completed the classification and plotted the results for 2, 3 and 4 clusters, answer the questions below.**. 


*Using the camera image provided above, answer these questions in your Jupyter Notebook:*
1. Which land cover/vegetation classes do you think each cluster corresponds to in your "2 cluster" classification?
2. Which land cover/vegetation classes do you think each cluster corresponds to in your "3 cluster" classification?
3. Which land cover/vegetation classes do you think each cluster corresponds to in your "4 cluster" classification?
4. Which number of clusters do you think is most appropriate for classifying the different cover types at this site?


That's it, you're done for this in-class exercise. Complete all your code in a Jupyter Notebook and upload it by the start of next class.

