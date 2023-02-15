# NMR-Log-Echo-Train-Inversion-in-Geolog-using-Scipy-Optimization
This repository employs NMR log echo train inversion using Scipy least_squares or optimization using Tikhonov regularization, which adds a penalty term equal to the sum of the squares of the parameters. 

We would like to thank Tim Putnam for introducing us to chatGPT. ChatGPT has become quite popular lately, so we decided to experiment with using this AI tool to perform NMR log T2 inversion using the SciPy least_squares and optimization libraries in Python with Tikhonov regularization, which incorporates a penalty term based on the sum of the squared parameters. Although the initial code provided by ChatGPT required some fine-tuning, it was a great starting point.

This repository includes a Jupyter Notebook as well as a complete Geolog project with Geolog python loglans, layouts and Geolog project structure.  

To create our echo train we are using the 8 bin porosities supplied with the NMR MRIL type of log to create an echo train with a TE of 1.2msec and 200 echoes. We then add random noise to create a realistic echo train as shown in the image below. It is common to stack the echoes to reduce some noise prior to the T2 inversion in this example.  

>![Geolog_Image](NMR_log.gif)

We allow you to choose between the SciPy least_squares, optimization or curve_fit methods for the T2 inversion. All methods were mentioned by chatGPT, but the SciPy least_squares method appears to be the best using the alpha regularization. An alpha of 0 is no regularization.  

We would suggest that you start with the Jupyter Notebook as a sort of help file with some documentation to better understand the workflow. The Geolog project can also be used with Geolog20+ where you have python installed for Geolog. 

>![Geolog_Image](Geolog_loglan.png)

Let us know if there are any issues. 
