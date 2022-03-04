##########################################################################
# ---------------------------------------------------------------------------------------------------------------------
# This is MATLAB code to produce IPCC AR6 WGI Figure 2.27
# Creator: Fabio Boeira Dias, University of Helsinki 
# Contact: fabio.boeiradias@helsinki.fi
# Last updated on: August 27, 2021
# --------------------------------------------------------------------------------------------------------------------
#
# - Code functionality: This code reads the Durack & Wijffels (2010) dataset and plots the (a) global sea surface salinity (SSS) trend and (b) global zonal mean surface salinity changes for the 1950-2019 period. Units are in Practical Salinity Scale 1978 (PSS-78).

# - Input data: Salinity mean (1950-2019, PSS), salinity change (1950-2019, PSS/70-years) and salinity change error (1950-2019, PSS/70-years) from Durack & Wijffels (2010, doi.org/10.1175/2010JCLI3377.1), available at insert link to CEDA

# - Output variables: The code provide the dataset to generate Figure 2.27, panel (a) and (b). The SSS maps (Fig. 2.27a) uses the SSS mean ("saltmean"), SSS trend ("saltchg") and mask for stippling ("mask_map", where salinity change error is greater than the saltinity change). Global zonal mean salinity (Fig. 2.27b) uses the salinity mean ("smean_dw10_glo"), salinity change ("schg_dw10_glo") and mask for stippling ("mask_sec1i" and "mask_sec2i", where salinity change error is greater than the salinity change)
#
# ----------------------------------------------------------------------------------------------------
# Information on  the software used
# - Software Version: MATLAB 2020b
# - Landing page to access the software: https://www.mathworks.com/products/matlab.html
# - Operating System: macOS Big Sur
# - Environment required to compile and run: m_map (https://www.eoas.ubc.ca/~rich/map.html) and stipple (https://www.mathworks.com/matlabcentral/fileexchange/68607-stipple)

#  ----------------------------------------------------------------------------------------------------
#
#  License: [insert here. Default license: Creative Commons Attribution 4.0 International License (http://creativecommons.org/licenses/by/4.0/)]*
#
# ----------------------------------------------------------------------------------------------------
# How to cite:
# When citing this code, please include both the code citation and the following citation for the related report component: 

[![DOI](https://zenodo.org/badge/438244314.svg)](https://zenodo.org/badge/latestdoi/438244314)


########################################################################
