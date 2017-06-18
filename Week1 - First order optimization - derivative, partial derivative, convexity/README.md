## Coding Challenge -- Due Date, Thursday June 22nd, 2017

This week's coding challenge is to implement gradient descent to find the line of best fit that predicts the relationship between
2 variables of your choice from a [kaggle](https://www.kaggle.com/datasets) dataset. Bonus points for detailed documentation. Good luck! Post your github link in the youtube comments section

## Dependencies for challenge

* numpy

## Dependencies for Full Notebook

* pandas (To read the dataset)
* matplotlib (Plotting)

## Overview/Summary

In this notebook, besides coding a **Gradient Descent** algorithm, other tasks are done, mainly related to visualizations.

### Visualize data

An overview of the data is done

[data.png]

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

[data_line.png]

### 3D Visualize Gradient Descent 

Each point in this two-dimensional space represents a line. The height of the function at each point is the error value for that line.

[gd.png]

### Live plot - Gradient Search & Intermediate lines

The current location of the **gradient descent search** and the path taken to get there and the **corresponding line** for the current search location. 

[]

### Live plot - Error

The error changing as we move toward the minimum.

[]










