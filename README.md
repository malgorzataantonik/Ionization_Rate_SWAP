# Ionization_Rate_SWAP
Ionization Rate of Interstellar Neutral Helium from New Horizons/SWAP Observations
Manuscript submitted to ApJ

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
  2. Download table A1 from [D. J. McComas et al 2022 ApJ 934 147](https://iopscience.iop.org/article/10.3847/1538-4357/ac7956#apjac7956t4).
  3. Update the default start/stop times in the script:
     
     ```time_start = "YYYY-MM-DDThh:mm"```
     ```time_stop = "YYYY-MM-DDThh:mm"```

  4. Update the default paths in the script:
  
     for the data files (by default, data is in directories named the same as DATA_SET_ID, for example, 'nh-x-swap-3-plutocruise-v3.0'):

     ```data_path = 'path/to/data'```

     for table with SWAP energy bins (Tab. A1 from D. J. McComas et al 2022 ApJ 934 147):

     ```bins_file_name='path/to/energy_bins_table'```

     and for output directory:
   
     ```results_path = 'path/to/results'```
   
# response_function.py

  > ## Requirements

   - Python 3.x
   - Libraries: numpy, scipy   
# solar_wind_parameters.py

  > ## Requirements

   - Python 3.9+
   - Libraries: numpy, astropy, scipy, pandas, torch, solarsystem, uncertainties
