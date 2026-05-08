# Investigating how different factors influence used car prices

## Project objective

The goal of this project is to determine what factors influence the price of used cars. Our investigation uses a regression-based approach to model the behavior of used car prices as a function of these factors.

[Here is a link to the Jupyter notebook for this project.](<prompt_II.ipynb>)

## Data description

Our data, which comes from Kaggle dataset, can be found in the [data/vehicles.csv.zip](data/vehicles.csv.zip) file (the file is a compressed zip file).

Each data point corresponds to a sold used car. The data points contain the selling price, as well as the year and model of the car, total miles on the odometer, and state and city where the car was sold. Much of the data contains additional information about the car such as paint color, drive type, fuel type, transmission, condition of the car, etc.

## Findings

Below are some plots showing how used car prices varied for some different parameters.

- Year:
\
![](plots/predicted_price_vs_year.png)
\
From the graph, we see that predicted price is low at 1900, reaches a peak around 1935, goes down to another trough at 1990, then increases greatly until 2022.

- Odometer miles:
\
![](plots/predicted_price_vs_odometer_value.png)
\
From the graph, we see that predicted price decreases steadily with odometer miles. Therefore we suggest preferring used cars with low odometer values.

- Car type:
\
![](plots/predicted_price_vs_car_type.png)
\
From the graph, we see that pickups, offroad vehicles, and (especially) convertibles get higher prices. Therefore, we suggest focusing on carrying thesee in inventory.

- Car paint color:
\
![](plots/predicted_price_vs_paint_color.png)
\
From the graph, we see that black and yellow cars have higher prices, whereas green cars have lower prices, on average. Therefore, we suggest preferring black and yellow cars, and avoiding green cars.

- Car fuel type:
\
![](plots/predicted_price_vs_fuel_type.png)
\
From the graph, we see that diesel cars have higher prices, so we suggest preferring these in inventory.

## Recommendations

Based on the above findings, we propose the following decisions:
- Avoiding cars from around 1900 and 1990, but preferring cars close to 1935 or close to 2022.
- Preferring used cars with low odometer values.
- Focusing on carrying pickups, offroad vehicles, and (especially) convertibles in inventory.
- Avoiding green cars, and preferring black and yellow cars.
- Preferring cars of diesel type in inventory.

