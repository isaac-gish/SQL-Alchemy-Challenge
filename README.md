# SQL-Alchemy-Challenge
Module 10 Challenge


All code for this challenge can be found in the climate_starter.ipynb file. 

All code for this challenge was created by me except for this excerpt of code: 
  "active_station = session.query(measurement.station).group_by(measurement.station).order_by(func.count(measurement.station).desc()).first()[0]


# Calculate the lowest, highest, and average temperature for the most active station
lowest_temp = session.query(func.min(measurement.tobs)).filter(measurement.station == active_station).scalar()
highest_temp = session.query(func.max(measurement.tobs)).filter(measurement.station == active_station).scalar()
average_temp = session.query(func.avg(measurement.tobs)).filter(measurement.station == active_station).scalar()
"

This excerpt was pulled from Chat GPT, in order to help increase the speed at which this assignment was finished. 

I do understand why this code works, and all credit for it's creation should go to Chat GPT. 

