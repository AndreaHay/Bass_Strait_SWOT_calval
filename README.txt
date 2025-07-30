==============
ABOUT
==============

The zipped files "Bass_Strait_SWOT_calval_data.zip" and "Bass_Strait_SWOT_calval_software.zip" contain data and python jupyter notebooks supporting the research presented in Earth and Space Science publication "In Situ Geometric Validation of SWOT Satellite Observations in Bass Strait, Australia", Hay et al., 2025. The analysis is conducted with data from the Bass Strait altimetry validation facility during the SWOT fast sampling phase (FSP) from 2023-03-30 to 2023-07-10.  


NOTES
- All GNSS outputs are from the GipsyX processing software, except where 'TRACK' is specified.
- Contact Andrea Hay, andrea.hay@utas.edu.au for further information.


ACKNOWLEDGEMENTS
- This study was supported by Australia’s Integrated Marine Observing System (IMOS) Satellite Altimetry Calibration and Validation sub-Facility - IMOS is enabled by the National Collaborative Research Infrastructure Strategy (NCRIS). It is operated by a consortium of institutions as an incorporated joint venture, with the University of Tasmania as Lead Agent. 


ADDITIONAL DATASETS
- SWOT Level 2 KaRIn Low Rate Sea Surface Height data (SWOT project, 2023) is openly available and distributed by PODAAC (https://podaac.jpl.nasa.gov/dataset/SWOT_L2_LR_SSH_Expert_2.0). 
- The GNSS buoy data are openly available through the Australian Ocean Data Network (https://portal.aodn.org.au/). 


==============
DATA
==============

- Locations of GNSS buoys during FSP (WGS84 latitude and longitude, and UTM55 eastings and northings) and mean SSH over the FSP period: 
	- buoy_locations_FSP_latlon.csv
	- buoy_locations_FSP_UTM.csv
	- GNSS_mean_SSH.csv

- Co-deployed GNSS buoy SSH prior to the FSP for differential-SSH uncertainty estimation:
	- co-deployed_GNSS_buoys.nc 

- GNSS buoy data at SWOT overflight times:
	- GNSS_at_SWOT_times.nc
	- TRACK_GNSS_at_SWOT_times.nc 
	- GNSS_SWH_at_SWOT_times.nc

- GNSS derived cross-track corrections for SWOT:
	- GNSS_derived_xt_correction.nc

- SWOT observations at buoy locations:
	- SWOT_products_at_buoys.nc
	- SWOT_SWH_at_buoys.nc

- SSH data from GNSS and SWOT reformatted for double differecing analysis:
	- GNSS_at_SWOT_times_SSH_only.csv
	- TRACK_GNSS_at_SWOT_times_SSH_only.csv
	- SWOT_at_buoys_SSH_only.csv 
	- SWOT_unsmoothed_SSH_only.csv 


==============
NOTEBOOKS
==============

- To calculate the differential-SSH uncertainty of the GNSS buoys:
	- Co-deployed_GNSS_for_dSSH_precision.ipynb

- To calculate the in situ derived cross-track corrections for SWOT and assess the SWOT corrections:
	- GNSS_derived_cross-track_correction.ipynb
	- Cross-track_correction_assessment.ipynb

- To calculate the SWOT absolute SSH bias:
	- Absolute_SSH_bias.ipynb

- To calculate the SSH semivariogram for SWOT and GNSS:
	- Semivariograms.ipynb

- To calculate the double differenced SSH comparison results presented in the main text and supporting information:
	- Double_differenced_SSH.ipynb
	- TRACK_Double_differenced_SSH.ipynb

- To compare the SWOT and in situ SWH:
	- SWH_comparisons.ipynb
