This document describes the bar minimum set of concepts about the Trapview second version api


General functioning


Nightly, weather data from Spain are downloaded according to the locations of 600 points that have been initially randomly placed on the map during the creation of the Climatenormals (i.e. the 15 years averages over Spain).

The Climatenormals are not supposed to change frequently and will stay "as is" per at least 5 years

With the weatherdata the ML models for Degree days prediction are created (firstly for climate and and those are not updated), then for weather (and these are updated nightly)

The apicall will use info from weather models and climate models to

a) generate per every point in the map the DegreeDays of a given pest for a point defined by lat/lon (should be in Spain NB)
b) generate the events for the pest (i.e. flights) and simulate the readings according to that peak


reading are now not using any trap readings from the partner (when available another set of tools should be used)




