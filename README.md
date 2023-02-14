# NMR-Log-Echo-Train-Inversion-in-Geolog-using-Scipy-Optimization
This repository uses NMR log echo train inversion using Scipy optimization using Tikhonov regularization, which adds a penalty term equal to the sum of the squares of the parameters. 

ChatGPT has become quite popular lately, so I decided to experiment with using this AI tool to perform NMR log T2 inversion using the SciPy optimization library in Python with Tikhonov regularization, which incorporates a penalty term based on the sum of the squared parameters. Although the initial code provided by ChatGPT required some fine-tuning, it was a great starting point.

This repository includes a Jupyter Notebook as well as a complete Geolog project with Geolog python loglans. 

>![Geolog_Image](NMR_log.gif)

We also allow you to choose between SciPy optimization or SciPy Curve_fit methods for the T2 inversion. Both methods were mentioned by chatGPT, but so far I am having trouble using regularization with the SciPy Curve_fit technique. This is work to be completed, and any advice will be well received. 
