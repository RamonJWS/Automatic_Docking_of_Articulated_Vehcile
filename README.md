<h1 align='center'> Automatic Docking of an Articulated Vehicle using Fuzzy Logic </h1>

## Project Motivation

The need for autonomous vehicles has never been in higher demand, with the world population growing, traffic and frequency of road accidents has increased constantly over the years.

This autonomy is particularly useful for situations which require high skill and precision. Reverse docking an articulated vehicle in a tight space while also avoiding other vehicles and pedestrians would require expensive training and constant retraining. However, a machine could be taught to do this job faster, safer, and at a reduced cost.

## Approach

After reviewing 28 academic papers it was clear that Fuzzy Logic would be the optimal machine learning choice to perform the desired task. It is worth mentioning that other systems such as Neural Networks paired with Fuzzy Logic also performed the task well, but with a marginal increase in performance and extensive increase in domain knowledge.

The system designed and modelled consists of 5 Fuzzy Logic controllers and a system capable of mathematical modelling the vehicles response. These Controllers can be divided into 2 categories, one for the control of the vehicle when driving forwards and one for the vehicle reversing. These forwards and reversing controllers require a Fuzzy Logic system to first determine the desired truck and trailer orientation for a given x, y position in the space, and then a second system to determine the steering angle of the vehicle to achieve this desired orientation. For the reversing system an additional Fuzzy Logic controller was required to prevent the jack-knife phenomenon from occurring.

## Results

Using 10 linearly spaced starting positions, and 10 randomly chosen starting positions the vehicle was able to reverse park the vehicle faster and with a higher degree of accuracy than the average truck driver.

Below i have included two of the randomly chosen starting positions with the truck’s initial orientation and position, its trajectory and its finally position.

<p align="center">
  <img src="https://github.com/RamonJWS/Automatic_Docking_of_Articulated_Vehcile/blob/master/fuzzy1.PNG" width=1000>
</p>

<p align="center">
  <img src="https://github.com/RamonJWS/Automatic_Docking_of_Articulated_Vehcile/blob/master/fuzzy2.PNG" width=1000>
</p>

## Future Improvements

During robustness testing it was found that increasing the vehicles length more than 0.6m would drastically reduce system performance and could take the system up to 12 manoeuvres to successfully dock the vehicle. Having a system that works for all articulated vehicles might be possible. If the project was improved the system would be designed with a larger variance in vehicle size in mind.

The system currently only works for a specific parking space. Some of the papers I reviewed used Neural Networks and Fuzzy Logic to allow for multiple parking lots to be used. If the project was to be improved this should be included.
