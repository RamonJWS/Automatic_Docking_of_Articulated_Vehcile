<h1 align='center'> Automative Docking of an Articulated Vehicle using Fuzzy Logic </h1>

## Project Motivation

The need for autonomous vehicles has never been in higher demand, with the world population growing, traffic and frequency of road accidents has increased constantly over the years.

This autonomy is particularly useful for situations which require high skill and precision. Reverse docking an articulated vehicle in a tight space while also avoiding other vehicles and patestrians would require expensive training and constant retraining. However, a machine could be taught to do this job faster, safer, and at a reduced cost.

## Approach

After reviewing 28 achedemic papers it was clear that Fuzzy Logic would be the optimal machine learning choice to perform the desired task. It is worth mentioning that other systems such as Neural Networks paired with Fuzzy Logic also performed the task well, but with a marginal increase in performance and extensive increase in domain knowledge.

The system designed and modelled consists of 5 Fuzzy Logic controllers and a sysyem capible of mathematical modelling the vehiles responce. These Controllers can be divided into 2 categories, one for the control of the vehicle when driving forwards and one for the vehicle reversing. These forwards and reversing controllers require a Fuzzy Logic system to first determin the desired truck and trailer orientation for a given x,y position in the space, and then a second system to determin the steering anlge of the vehicle to achieve this disired orientation. For the reversing system an addiationl Fuzzy Logic controller was required to prevent the jack-knife phenomenon from occuring.

## Results

Using 10 linearly spaced starting positions, and 10 randomly chosen starting positions the vehicle was able to reverse park the vehicle faster and with a higher degree of acuracy than the average truck driver.

Below i have included two of the randomly chosen starting positions with the trucks initial orientation and position, its trajectory and its finaly position.
