# Intro_to_the_Math_of_intelligence
This is the code for "Intro - The Math of Intelligence" by Siraj Raval on Youtube

## Coding Challenge -- Due Date, Thursday June 22nd, 2017

This week's coding challenge is to implement gradient descent to find the line of best fit that predicts the relationship between
2 variables of your choice from a [kaggle](https://www.kaggle.com/datasets) dataset. Bonus points for detailed documentation. Good luck! Post your github link in the youtube comments section

## Overview

This is the code for [this](https://youtu.be/xRJCOz3AfYY) video on Youtube by Siraj Raval. The dataset represents distance cycled 
vs calories burned. We'll create the line of best fit (linear regression) via gradient descent to predict the mapping. yes, I left out talking about the learning rate in the video, we're not ready to talk about that yet. 

Here are some helpful links:

#### Gradient descent visualization
https://raw.githubusercontent.com/mattnedrich/GradientDescentExample/master/gradient_descent_example.gif

#### Sum of squared distances formula (to calculate our error)
https://spin.atomicobject.com/wp-content/uploads/linear_regression_error1.png

#### Partial derivative with respect to b and m (to perform gradient descent)
https://spin.atomicobject.com/wp-content/uploads/linear_regression_gradient1.png

## Dependencies

* numpy

Python 2 and 3 both work for this. Use [pip](https://pip.pypa.io/en/stable/) to install any dependencies.

## Usage

Just run ``python3 demo.py`` to see the results:

   ```
Starting gradient descent at b = 0, m = 0, error = 5565.107834483211
Running...
After 1000 iterations b = 0.08893651993741346, m = 1.4777440851894448, error = 112.61481011613473
   ```

## Credits

Credits for this code go to [mattnedrich](https://github.com/mattnedrich). I've merely created a wrapper to get people started. 
