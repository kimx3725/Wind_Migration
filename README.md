# Arctic Tern Migration Wind Modeling 

## Codes 
### Wind Visualization 
- 0.wind_data_prep.Rmd
  - Extract wind data and store them per 10m grid map
  - Tidy the wind data and simulate daily speed and direction on the map 

- 1.tern_wind_visualization.Rmd:
  - extract the simulated fall migratory track data of the tern BF426
  - merge the tracking data with the filtered wind data 
  - simulate both track and wind speed & direction per day 

- 2.data_manipulation.Rmd:
  - regularize the track data and convert the data to trk object with 'amt' package 
  - calculate the wind cost based on Fellcislmo et al. 2008
  - extract wind covariates from the raster layers that match the tracking locations 
  
- 3.data_analysis.Rmd:
  - fit SSFs to the trk data including wind cost as a predictor 
  - create a coefficient plot
