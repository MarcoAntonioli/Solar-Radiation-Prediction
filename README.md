# Solar-Radiation-Prediction

Project developed alongside Edoardo Botta and Elia Torre for the Hackathon of the Bocconi Students for Data Science.

The dataset "train_set.csv" is related to the level of solar radiation on earth registered from 11/9/2016 to 31/12/2016. With all the sensor data related to solar radiation, we had to predict a continuous variable related to the quantity of variation for a specificied instant. 

Let’s try to dive into this dataset and let me denote the units of the following columns.

  1. UNIX time: seconds since Jan 1, 1970
  2. The date
  3. The local time of day
  4. Solar radiation: watts per meter squared (Label variable, to be predicted)
  5. Temperature: degrees Fahrenheit
  6. Humidity: percent
  7. Barometric pressure: Hg
  8. Wind direction: degrees
  9. Wind speed: miles per hour
  10. Sunrise: Hawaii time
  11. Sunset: Hawaii time
  
 The training set has all the 11 columns described above, while "test_set.csv”, the test set misses the label column, the one called “Solar Radiation”, and on this dataset our ML model was tested.
 
 We decided to tackle the problem using a voting regressor between some tree based model. 
 For our work, which predicted the solar radiation with a mean squared error in the test set of 5569, we have been crowned winners of the competition. The analysis, with the neccessary comments and explanations can be found in the "Solar_Radiation_Prediction.ipynb" file.
