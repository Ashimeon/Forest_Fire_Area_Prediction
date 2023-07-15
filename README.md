# Forest_Fire_Area_Prediction
The goal of this challenging regression challenge is to forecast the burnt area of forest fires in Portugal's northeast region using meteorological and other data.
### (See details at: http://www.dsi.uminho.pt/~pcortez/forestfires)

For more information, read [Cortez and Morais, 2007].
   1. X - x-axis spatial coordinate within the Montesinho park map: 1 to 9
   2. Y - y-axis spatial coordinate within the Montesinho park map: 2 to 9
   3. month - month of the year: 'jan' to 'dec' 
   4. day - day of the week: 'mon' to 'sun'
   5. FFMC - Fine Fuel Moisture Code index from the FWI system: 18.7 to 96.20
   6. DMC - Duff Moisture Code index from the FWI system: 1.1 to 291.3 
   7. DC - Drought Code index from the FWI system: 7.9 to 860.6 
   8. ISI - Initial Spread Index index from the FWI system: 0.0 to 56.10
   9. temp - temperature in Celsius degrees: 2.2 to 33.30
   10. RH - relative humidity in %: 15.0 to 100
   11. wind - wind speed in km/h: 0.40 to 9.40 
   12. rain - outside rain in mm/m2 : 0.0 to 6.4 
   13. area - the burned area of the forest (in ha): 0.00 to 1090.84 
   (this output variable is very skewed towards 0.0, thus it may make
    sense to model with the logarithm transform).

# Supervised Learning
- Objective: To predict burned area through different parameters using various regression models with their hyper-tuned parameters.
- Error measurement: Using Root Mean Squared Error Calculation, Mean absolute error and R2 score.

# Conclusion
Random Forest Regressor was found to be the best model as it had minimum Rmse score of 1.418.