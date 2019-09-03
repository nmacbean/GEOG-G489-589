# Welcome to GEOG-G489/589: Advanced Geospatial Data Analysis in Python

These course notes are for the in-class exercises and assessments in the GEOG-G489/589.
Department of Geography Indiana University
Fall 2019 Syllabus
Lecture: Monday & Wednesday 1:00 PM to 2:15 PM Lecture Location: Student Building 221
Instructor: Dr. Natasha MacBean
Office: Student Building 204
Email: nmacbean@indiana.edu
Office hours: Monday 12:00 PM to 1:00 PM and Wednesday 3:15 PM to 4:15 PM.
Course description
This course introduces students to the Python programming language and the Python skills needed to perform complex data analysis and data visualization with large spatiotemporal datasets (for example model simulations and remote sensing data).
In the course we will learn how to install python and how to download the various packages we will use, as well as how to download the remote sensing, climate, and modeling datasets we may analyze. In the first part of the course we will review fundamental concepts in Python (e.g. data types, data structures, indexing, subsetting, looping over data) that will be useful for handling large volumes of data. Following that, we will cover the following data handling topics: reading and manipulating large, multi-layer spatio-temporal datasets, vector and raster data manipulation, map reprojection, area selection based on geographic coordinates, masking data, data visualization (including plotting maps). Finally, throughout the course we will cover the following data analyses on large geospatial datasets, including: applying basic statistics to large datasets (sub, mean, max, min), interpolation and smoothing, regression, function fitting for extracting information from time series data, change detection, image classification and spatial clustering, dimensionality reduction.
Throughout, we will focus on developing the most fundamental and useful data science skills – such as cleaning and tidying data in preparation for data analysis, and elegant and efficient code writing – so that your code writing skills result in useful scripts that can be used in the future to repeat similar analyses on new scientific questions.
Students will become familiar with the following Python packages: NumPy (Numerical Python), GDAL (Geospatial Data Abstraction Library), SciPy (Scientific Python), (Geo)Pandas (Python Data Analysis Library – also relies on packages Shapely and Fiona), CartoPy, PySAL (Python Spatial Analysis Library), scikit-learn, Matplotlib and Seaborn. There will be an emphasis on remote sensing (satellite) data, climate reanalysis and modeling datasets.
We will meet in the Student Building Room 221 computing cluster and all classes will be lab focused where topics will be introduced with practical exercises. No previous programming
  
experience is required, but it would be helpful (for example GEOG-G 250/577, GEOG-G 488/588, SICE I210).
Course Goals and Learning Outcomes
Course goals:
Students who engage in this class will be equipped to use Python to develop their own scientific code to analyses large spatiotemporal data analyses that will be useful in their own research and careers in geospatial data analysis. Students will be given a grounding in the basic principles of algorithm development and the construction of scientific programs for analyzing data that can be transferred and widely applied outside the topics covered in the class.
Learning outcomes:
At the end of this course, students should:
• Understand the basics of scientific computing
• Have a good working knowledge of the Python programming language
• Know how to install commonly available scientific software packages
• Be able to develop code and construct scientific programs Python to perform data
manipulation tasks with large (high volume) geospatial datasets
• Be able to write efficient, well-structured and commented Python scripts for a range of
data analysis tasks.
• Be able to carry out a variety of analytical tasks on large, multi-layer spatiotemporal
datasets
• Understand technical issues with data visualization and geospatial data analysis and
approaches to solve those issues.
Python
Python is a high-level programming language that is freely available, relatively easy to learn and portable across different computing systems. In Python, you can rapidly develop code/programs to perform the analyses you may need to do both in your research and future career. Code written in Python is also easy to maintain, is (or should be) self-documented, and can easily be linked to code written in other languages.
Advantages of Python include:
• it is automatically compiled and executed
• code is portable provided you have the appropriate Python modules installed.
• there are many well-documented existing packages you can employ for you data
analysis needs
• there is an active user and development community, which means that there is a lot of
useful advice and documentation online. Within this community, new capabilities appear over time and there are many existing extensions and enhancements easily available to you.
I suggest you use the anaconda python distribution if you are using your own computer, but we can discuss options for installing on your own computer during class.
   
Optional texts
There are no required texts for this course. All the relevant material will be provided in the assignments on Canvas. When learning how to program there are often a lot of useful tutorials and websites with advice online. This is especially true for a freely available programming language such as Python. However, students may find the following textbooks useful. I will bring copies of these textbooks to class in the first few weeks so students can have a look and decide if they are worth buying themselves.
• McKinney, W. (2012). Python for data analysis: Data wrangling with Pandas, NumPy, and IPython. O'Reilly Media, Inc.
• Scopatz, A., & Huff, K. D. (2015). Effective computation in physics: Field guide to research with python. O'Reilly Media, Inc.
• Lawhead, J. (2015). Learning Geospatial Analysis with Python Second Edition. Packt Publishing Ltd.
• Grus, J. (2015). Data science from scratch: first principles with python. O'Reilly Media, Inc.
• Garrard, C. (2016). Geoprocessing with Python. Manning Publications.
The course page will also be updated with useful websites and articles specific to each topic
that will help us during each class.
Course Format and Grading
In-class exercises: At the beginning of each class we will review the concepts that we will be covering during that class. This will include developing a logical argument for the algorithm we develop during the class. The algorithm is essentially the method, or set of methods, we will use to complete our programming task/data analysis. We will then discuss together the Python code needed to put that algorithm into an executable Python script. Following this group discussion, you will each get time to write the script in a Jupyter Notebook (a commonly used open-source application for writing and executing code). In-class exercise assignments will be posted on Canvas. The assignment will be due by the beginning of the next class. Assignments (in the form of your Jupyter Notebook) will be uploaded to Canvas. Homework in the form of DataCamp.com tutorials may be set before each class to give an introductory overview of a given Python topic before covering that topic in more detail during the class. The homework will not be graded.
In-class assessments: There will be three in-class assessments to test your knowledge of the material learned so far in the course during the 2nd class in the 4th, 8th and 12th week of the semester. These will be silent but open-book assessments in which you can also search online for relevant python syntax, but you will need to complete the assessment during the 1h 15 minutes of the class and you will not receive any help from the instructor or other students on the course.
  
Final Project: The final project will be designed and carried out in Python by each student on a topic of their own choosing. This project will be completed in the final 4 weeks of the course. The student will use the data downloading, manipulation and analysis methods learned in the class to answer a scientific question pertaining to their own data analysis and research interests. More information about the final project will be provided at the start of the semester. Additional requirement for G589 students: the final project will be more extensive and based on your research interests. It will make up a greater percentage of your overall grade. More information will be given in class.
Please note: The final project deadline will be 11:59pm Sunday 15th December.
 Grading (489):
Grading (589):
Grading Scale
In-class exercises – 45% In-class assessments – 20% Final project – 30% Participation – 5%
In-class exercises – 35% In-class assessments – 20% Final project – 40% Participation – 5%
 
 
97% - 100% A+
 77%-<80% C+
93%-<97% A
73%-<77% C
90%-<93% A-
70%-<73% C-
87%-<90% B+
67%-<70% D+
83%-<87% B
63%-<67% D
80%-<83% B-
60%-<63% D-
 
 
< 60% F
 Grade Dissemination:
All grades will be posted on Canvas. Please make sure to track your own grades, as mistakes can occasionally occur. If you have received a grade by mistake, please see me for a correction in Canvas.
