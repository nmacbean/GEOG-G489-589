# Exericse 14: Unsupervised hyperspectral image classification

This week we will be learning about unsupervised learning using the KMeans Clustering analysis from scikit-learn (https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html). We will be applying this to classify hyperspectral imagery to determine fraction of land cover types (shrub, grass, bare soil) at the semi-arid Santa Rita site in southern Arizona.

In today's class our guest lecturer Rubaya Pervin will be talking through the methods as well as the data cleaning and tidying process.

In Wednesday's class we'll be doing an in-class exercise to practice the image classification using KMeans clustering.

Today's (Monday's) homework is to complete the DataCamp tutorial on "lustering for Dataset Exploration: (Chapter 1) of the Unsupervised Learning Module: https://www.datacamp.com/courses/unsupervised-learning-in-python. This will help you to become more familiar with the KMeans method before Wednesday's in-class exercise.

## In-class exercise: KMeans Clustering for unsupervised classification at the Santa Rita site

In today's exercise you will follow the classification steps taught in the lecture on Monday to classifiy hyperspectral dataset from a different part of the Santa Rita Experimental site. These data were collected from the NEON airborne platform in August 2018. The photo below shows the camera image of area we'll be classifying.

![santa rita](2018_SRER_2_514000_3519000_image.png)
The camera image has a spatial resolution (spatial footprint) of 10cm, whereas the hyperspectral data have a spatial resolution of 1m.

The hyperspectral data have already been cleaned following the steps described on Monday (removing missing and negative numbers, cleaning the bad/noisy bands of information). The cleaned data are in a file called "2018_SRER_2_514000_3519000_hyperspectral_cleaned.tif". Due to the size of the file, it is provided in this folder on box: https://iu.box.com/s/6az0ez3s9u6jx6pimd3l7p1blc2sojli

As detailed in the lecture on Monday, there are three dimensions in the data corresponding to [nbands, nrows, ncols], where nbands is the number of (cleaned) hyperspectral bands. *Note, the order of the dimensions is different from the lecture slides.* There are 360 bands, 1000 rows and 1000 columns.

Follow the steps below to complete the exercise and then answer the following questions. Look through the lecture notes from Monday to help you with the code. You may also want to look back to Exercise 10 on GDAL to help you with how the GDAL commands are structured

**i.** Download the data from the box folder and open the file using the gdal open file command. (Don't forget to import all the libraries you will need first).

**ii.** Then read in the array to the variable data with the gdal command ReadAsArray. 

**iii.** Reshape your data so they correspond to the dimensions we need for the sklearn KMeans clustering algorithm (this is similar to slide 17 but because the dimensions are different we need to use:

**data = data.reshape((np.shape(data)[0], -1))**

NOTE: We then need to transpose the data so the dimension order matches the way sklearn wants us to input the data (with nsamples and nfeatures - see below. For this, we use the command:

**data = np.transpose(data)**

Print the shape of the data before and after each step so you can understand what is happening in each step. 

For this step, it would be useful to refer to the sklearn kmeans clustering method manual page (see above). If you scroll down to the methods "fit" and "fit_predict" you will see that the same of the array we give to the method (X on the manual page) needs to have the dimensions of "nsamples" and "nfeatures". 

Recall from what we have learned about Sklean so far that the nsamples is the number of observations we have of each "feature". The features are essentially the different types of information we will use to form the clusers.  

In this case, the features are the different hyperspectral bands containing reflectance information from different parts of the electromagnetic spectrum (read the links on hyperspectral data from the lecture if you would like to learn more).  

The nsamples are the information from both the rows and columns - therefore, we need to collapse the rows and columns from 2 dimensions into 1 dimension containing all the rows and columns (note we did something similar in the statistical analysis in Python).  

**iv.** Now you have reshaped your data, you will be able to perform the KMeans clustering algorithm following the steps shown in slide 16 (also 18 and 19). Repeat the classification for 2, 3 and 4 clusters.  

**v.** Now plot your result using plt.imshow (see slide 20 of the lecture) Note that you will have to reshape your data again to get the data into .  

**vi. Once you have completed the classification and plotted the results for 2, 3 and 4 clusters, answer the questions below.**. 



*Using the camera image provided above, answer these questions in your Jupyter Notebook:*

If you need to zoom in to compare the classification and the camera image - select a subset of your data with simple indexing BUT beware that because the resolution of your camera image is 10cm (0.1m) and the resolution of the hyperspectral classification is 1m, the extent of your subset will need to be 10x larger for the camera image. E.g.:  
**labels2_zoom = labels2[0:100,0:100]**
**camera_image = camera_image[0:1000,0:1000]**  
You can read in the camera image using plt.imread(camera_image_filename), which is "2018_SRER_2_514000_3519000_image.tif" and is in the box folder.

Questions:  
1. Which land cover/vegetation classes do you think each cluster corresponds to in your "2 cluster" classification?
2. Which land cover/vegetation classes do you think each cluster corresponds to in your "3 cluster" classification?
3. Which land cover/vegetation classes do you think each cluster corresponds to in your "4 cluster" classification?
4. Which number of clusters do you think is most appropriate for classifying the different cover types at this site?


That's it, you're done for this in-class exercise. Complete all your code in a Jupyter Notebook and upload it by the start of next class.

