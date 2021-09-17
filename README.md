# parasite_energetics_AmNat2021
Code and data to reproduce analyses and graphics for 'Host energetics explains variation in parasite productivity'

Four datasets are providing as .csv files. 

Data S1. 'DataS1.parasite_community_abundance_data'
This is a .csv file containing data pertaining to Figure 1.
In Figure 1 plotted are the partial residuals of the linear model: np ~ avg_alpha + mh_alph_no_temp 
Note. Data S1 is filtered by absolute maximum community abundance; see Table S2 for comparison of model coeffs.  

Data S2. 'DataS2.parasite_community_flux_data'
This is a .csv file containing data pertaining to Figure 2.
In Figure 2 plotted is parasite_flux ~ mh_alpha
Note. Data S2 is filtered by absolute maximum community flux; see Table S3 for comparison of model coeffs.   

Data S3. 'DataS3.energy_flux_ecosystem'
This is a .csv file containing data pertaining to figure 3. 
In Figure 3A plotted are log_parasite_flux ~ log _host_flux + river
In Figure 3B plotted are log_parasite_biomass ~ log_host_biomass +river

Data S4. 'DataS4.platyhelminthes_scaling'
This is a .csv file containing data used to estimate platyhelminthe metabolic scaling parameters given in Table 1, further details are provided in Appendix 1. 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Metadata_S1-4.txt 
Provides column headers for Data S1-S4

parasite_energetics_MS_analyses_Aug2021.Rmd
Rmarkdown file to reproduce graphics and analyses 
