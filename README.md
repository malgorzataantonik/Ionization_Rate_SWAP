# Ionization_Rate_SWAP
Ionization Rate of Interstellar Neutral Helium from New Horizons/SWAP Observations

## Main Files

- `SWAP_data.py` – program to read FITS files and save SWAP spectrum to .txt files
- `response_function.py` – program to calculate SWAP energy-angle response function for rotation-average FOV
- `solar_wind_parameters.py` – program to calculate parameters of solar wind from SWAP data

# SWAP_data.py

  > ## Requirements

   - Python 3.x
   - Libraries: numpy, astropy, pandas
   
   Make sure all required packages are installed.
  
  > ## Usage Instructions

  1. Download the New Horizons/SWAP and/or NH Kuiper Belt Extended Missions (KEM and KEM2)/SWAP calibrated data from [NASA PDS](https://pds-smallbodies.astro.umd.edu/data_sb/by_mission.shtml).
  2. Update the default start/stop times in the script:
   ```time_start = "YYYY-MM-DDThh:mm"```
   ```time_stop = "YYYY-MM-DDThh:mm"```

  3. Update the default paths in the script for the data files and output directory:

   ``` data_path = "path/to/data"```
   ```results_path = "path/to/results"```

   # response_function.py

     > ## Requirements

   - Python 3.x
   - Libraries: numpy, scipy
     
   # solar_wind_parameters.py

     > ## Requirements

   - Python 3.9+
   - Libraries: numpy, astropy, scipy, pandas, torch, solarsystem, uncertainties
