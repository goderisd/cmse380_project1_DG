# cmse380_project1_DG
In the directory there are 3 notebook files
  project1_derekGoderisV2
  project1_derekGoderisV3
  project1_derekGoderis_visualization
2 CSV files for sources 
  flights_sample_3m
  WeatherEvents_Jan2016-Dec2022
and 3 output CSV files 
  Cancelled_flights_2022
  non_cancelled_flights_2022
  weatehr_data_2022

V2 is where I did most of my learnign on handling suchsa large data set, however I realized when that I performed the imputations incorrectly when I went to visualize.  THis was because I did not split the flights into cancelled in occured, which meant i was imputing values such as arrrival/departure time for flights that never occured.


The first thing you need to do to run the program is clown/download the flights data set and the weather data set:

Source for weather data set: https://www.kaggle.com/datasets/sobhanmoosavi/us-weather-events/suggestions?status=pending&yourSuggestions=true

Source for flight delay set: https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023

I uploaded the V2 to as a demonstrator for the learning that I, so please feel free to look but runnign it won't produce any usable outputs.

V3 is where I took the lessons learned on handling the massive flights data set, and started to work on just 2022 flight data.  To  excute this notebook run the cells in order and the 3 csv files that are needed for the next steps will write into you parent directory.  I chose to do this becuase computing the KNN on the data everytime is very computational expensive.  I also commmited the csv file outsputs to this project if you want ot just go directly to the streamlit/visualation without running my impuations and such


  Visualization is where the EDA largley has occured, I built many plots in there to visualize some of the trends that I could start to explore when we begin learning models 

  I attached the .py script to run a local streamlit app that can execute teh full 2022 flight data.

  Finally, for the hosted streamlit app there is a pyhton script in the other github repo attached in d2l which i wrote using pycharm. I ahd to down sample the final data files by 1% to get streanlit to accept the hosting, so the visuals for the hosted app dont look so clean. However, if ran on local machine it looks very good 
