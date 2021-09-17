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

Metadata for S1 and S2:
Column_headers. 

host_species: genus and species of host taxa 

code: unique identifier of host individual used in the analysis 

parasite_flux:  unit watts; temperature corrected parasite community flux following equation 6 in the main text; parasite flux = [(a*parasite body mass (kg) ^b)* exp((E_parasite/0.0000862)*(-((Temp_O+273.15)^-1) + ((Temp+273.15)^-1))))] * parasite abundance) and summed across all parasite species, where a = phylum specific normalization constant from table 1 in maint text and b = phylum specific scaling exponenet from table 1.  

mh_alpha: unit watts; temperature corrected host metabolic rate following equation 5 in the maint text; host metabolic rate = (a * host body mass (kg) ^ b) * exp((E_host/0.0000862)*(-((Temp_O+273.15)^-1) + ((Temp+273.15)^-1))))

mh_alpha_no_temp: unit watts; host metabolic rate following equation 5 in the maint text; host metabolic rate = (a * host body mass (kg) ^ b) 
mh: units grams; host body mass 

np: total parasite abundance, which is all parasite individuals within a host 

n: number of hosts dissected; using a min. of 15 individuals per host species

avg_alpha: unit watts; mean energy usage within a parasite community see main text for calculation (note this is not temp corrected)

host_taxon: host taxonomic group, pertains to metabolic scaling parameters in table 1

Temp_O: units celsius; environmental temperature during collection period (notes needs to transforemd to kelvin for temperature correction) 

Data_source: where the data came from, new data= unpublished data first used in this manuscript 

Data S3. 'DataS3.energy_flux_ecosystem'
This is a .csv file containing data pertaining to figure 3. 
In Figure 3A plotted are log_parasite_flux ~ log _host_flux + river
In Figure 3B plotted are log_parasite_biomass ~ log_host_biomass +river
Metadata for S3.:
Column_headers.

river: name of river ecosystem; Passaic, Raritan, Mullica

season: seaon fall, winter, spring, summer 

plot: site within river ecosystem 

log_parasite_flux: units watts/m^2; log10 transformed parasite community flux within a sample

log_host_flux: units watts/m^2; log10 transformed host community flux within a sample 

log_parasite_biomass: units g/m^2; log10 transformed parasite biomass density within a sample 

log_host_biomass: units g/m^2; log10 transformed host biomass density within a sample 

Data S4. 'DataS4.platyhelminthes_scaling'
This is a .csv file containing data used to estimate platyhelminthe metabolic scaling parameters given in Table 1, further details are provided in Appendix 1. 

Metadata for S4:
Column_headers.

species: parasite species; genus species

stage: parasite lifecycle stage; adult, larvae, sporocyst, redia 

Temperature C: temperature at which metabolic rate was taken in degrees celsius 

Body mass in original units: body mass of parasite in orignal units from study

Mass original units: units of mass  in study

Mean Respiration Rate in original units: metabolic rate in orignal units from study

respiration_units: units of metabolic rate in study

Notes on conversion: all conversions used

ln(body mass) (kg): units kg; natural log transformed body mass in wet weight 

ln(metabolic rate) (Watts): units watts;  natural log transformed metabolic rate

Source:	citation of study

Host type: host used in the study given as genus species/'free-living' indicates free living larval stage used 
