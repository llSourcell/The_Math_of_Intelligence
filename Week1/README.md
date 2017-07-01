# CODING CHALLANGE WINNER!

## Coding Challenge -- Due Date, Thursday June 22nd, 2017

This week's coding challenge is to implement **gradient descent** to find the line of best fit that predicts the relationship between
2 variables of your choice from a [kaggle](https://www.kaggle.com/datasets) dataset. By <a href="https://github.com/llSourcell/The_Math_of_Intelligence">Siraj Raval.</a>

The submission file is: <a href="https://github.com/alberduris/The_Math_of_Intelligence/blob/master/Week1/demo.ipynb">demo.ipynb</a>

## Dependencies for challenge

* numpy

## Dependencies for Full Notebook

* pandas (read the dataset)
* matplotlib (plotting)

## Live Plots

From the Github view of Jupyter Notebooks it's not possible to view the live plots, well, live. Just the last snapshot of the live plot is shown. To enjoy the live plot it is necessary to download the Jupyter Notebook and run it locally (If there's another way, tell me please :))

You can recognise a live plot with the presence of 
```
%matplotlib notebook
```
in the cell, that enables some matplotlib interactive features.

## Data

That's the least relevant thing but <a href="https://www.kaggle.com/reagentx/HLTVData">"CS:GO Dataset"</a> has been chosen.

From file 'ADRvsRating.csv' has been chosen the variables:
 - **ADR** : Average damage per round
 - **Rating** : HLTV Rating 2.0

## Overview/Summary

In this notebook, besides coding a **Gradient Descent** algorithm, other tasks are done, mainly related to visualizations.

### Visualize data

An overview of the data is done

![Data](https://github.com/alberduris/The_Math_of_Intelligence/raw/master/Week1/resources/data.png)


### SSE - Sum of Squared Error

A simple SSE algorithm for measuring error

```
def SSE(m,b,data):
    totalError = 0.0
    for i in range(numInstances):
        currentTarget = data[i,1]
        #y = mx + b
        currentOutput = m*data[i,0] + b
        #Compute squared error
        currentSquaredError = (currentTarget - currentOutput)**2
        totalError += currentSquaredError
    sse = totalError/numInstances
    return totalError
```
### Visualize data plus fitting line

An overview of the data with a fitting line

![Data plus fitting line](https://github.com/alberduris/The_Math_of_Intelligence/blob/master/Week1/resources/data_line.png)

### 3D Visualize Gradient Descent 

Each point in this two-dimensional space represents a line. The height of the function at each point is the error value for that line.

![Gradient Descent](https://github.com/alberduris/The_Math_of_Intelligence/blob/master/Week1/resources/gradient_descent_1.png)

### Live plot - Gradient Search & Intermediate lines

The current location of the **gradient descent search** and the path taken to get there and the **corresponding line** for the current search location. 

![Gradient Search & Intermediate Lines](https://github.com/alberduris/The_Math_of_Intelligence/blob/master/Week1/resources/live_plot_gs_il.png)

### Live plot - Error

The error changing as we move toward the minimum.

![Error](https://github.com/alberduris/The_Math_of_Intelligence/blob/master/Week1/resources/live_error.png)

### References

<a href="https://spin.atomicobject.com/2014/06/24/gradient-descent-linear-regression/">Siraj Raval - Youtube - Intro - The Math of Intelligence</a>

<a href="https://spin.atomicobject.com/2014/06/24/gradient-descent-linear-regression/">An Introduction to Gradient Descent and Linear Regression - MATT NEDRICH</a>
