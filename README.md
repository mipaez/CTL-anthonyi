# CTL-anthonyi
Data for research on thermal limits of Epipedobates anthonyi

This Paez-Vacas-and-Funk-2022_DATA_README.txt file was generated on 2022-08-01 by Monica Paez-Vacas

GENERAL INFORMATION

1. Title of Dataset: Data from Thermal limits along tropical elevation gradients: poison frog tadpoles show plasticity but maintain divergence across elevation

2. Author Information
	Corresponding Investigator 
		Name: Dr. Monica I. Paez-Vacas
		Institution: Universidad Tecnologica Indoamerica, Quito, Ecuador
		Email: monicapaez@uti.edu.ec

	Co-investigator 1
		Name: Dr W. Chris Funk
		Institution: Colorado State University, Fort Collins, CO, USA

3. Date of data collection: 2014-2015

4. Geographic location of data collection: Ecuador

5. Funding sources that supported the collection of the data: Secretaría Nacional de Educación Superior, Ciencia y Tecnología del Ecuador, and Graduate Degree Program of Ecology Research Grant

6. Recommended citation for this dataset: Paez-Vacas and Funk (2022), Data from: Data from Thermal limits along tropical elevation gradients: poison frog tadpoles show plasticity but maintain divergence across elevation

DATA & FILE OVERVIEW

1. Description of dataset

These data were generated to investigate the effect of temperature variation along elevational transects on population divergence in CTMAX and CTMIN of 934 tadpoles of a poison frog species, Epipedobates anthonyi, along two elevational gradients (200 – 1700 m asl) in southeastern Ecuador. We also tested if tadpoles could plastically shift their thermal limits in response to exposure to different temperatures treatments (20 °C, 24 °C, and 28 °C). 

Geographic coordinates data has not been included in the dataset as they contain contain information that could be used for illegal wildlife trade.

2. File List: 
	File 1 Name: Paez-Vacas-and-Funk-2022-data-thermal-limits-anthonyi.csv
	File 1 Description: Database with each individual ID code, population of origin, thermal limit, thermal limit estimate, temperature treatment, total length, body length, year of experiment, days in acclimation temperature, month of experiment, mean habitat temperature, standard deviation of habitat temperature.
	
METHODOLOGICAL INFORMATION

We studied six populations of Epipedobates anthonyi located at low, mid, and high elevations within each of two elevational transects (200 - 1700 m asl) in southwestern Ecuador. 
Every tadpole in this study was wild-caught and acclimated at a given temperature for at least five days so that field-sampled individuals living at diverse envi­ronmental temperatures were all acclimated at the same temperatures, which is standard protocol when estimating thermal limits. 
Instead of using a single acclimation temperature, we randomly assigned each tadpole to one of three different acclimation temperatures, to simultaneously test that acclimation temperature could influence thermal limits. 
The three temperature treatments were 20 °C, 24 °C, and 28 °C. Tadpoles were not fed for 1–2 days prior to the experiments to avoid expenditure of energy for digestion during thermal tolerance experiments. Only tadpoles in developmental Gosner stages 25-38 (Gosner, 1960) were used to minimize effects of developmental stage on thermal tolerance. To measure critical thermal limits, each tadpole was placed in an individual mesh container in a water bath in a different tank. Initial temperature was the same as the respective treatment temperature. After 1-minute baseline period, temperature was increased or decreased at a constant rate of 0.5 °C min-1. Temperature was recorded with a digital temperature logger (Omega, HH804) connected to an Ultra precise RTD sensor (Omega, P-M-A-1/8-12-O-G-3). Given the erratic movements of tadpoles, we recorded the temperature at which there was absence of response to a mechanical stimulus, which consisted of squirting water at the tadpole with a turkey baster. For CTMIN, we recorded the temperature when tadpole mobility ceased completely and they failed to respond to a mechanical stimulus. After reaching CTMAX or CTMIN, tadpoles were immediately (less than five seconds) placed in another water bath maintained at room temperature to allow recovery. We recorded total length, body length, and Gosner stage for each tadpole. Only data from tadpoles that appeared to recover immediately and that did not show signs of stress after one hour of observation were included in analyses. Each tadpole was tested only once. To evaluate if there were differences in thermal limits among populations from different elevations, and if tadpoles had the ability to shift their thermal limits in response to treatment temperature, we used linear mixed models. Models included elevation, (i.e., population of origin: high, mid, and low elevation populations from both transects) and acclimation temperature treatment as fixed effects. Size (body length, BL) and time in the treatment temperature (in days) were included as random effects. We chose to use only body length as a metric for size because it was highly correlated with total length and Gosner stage (Pearson’s r = 0.92, r = 0.85, respectively). For Transect 1, we also included year (2014 or 2015), and mean habitat temperature as random effects, because we wanted to include short-term temperature exposure obtained with dataloggers. Models were run using the lmer function in the lme4 package in R. Models were ranked using Akaike’s Information Criterion. A model was considered the best model if it had an AIC score two lower than the second-best model. If there were models with similar support, we chose the one with fewer parameters as the best model.

DATA-SPECIFIC INFORMATION FOR: Paez-Vacas-and-Funk-2022-data-thermal-limits-anthonyi.csv

1. Number of variables: 16

2. Number of cases/rows: 934 (without heading)

3. Variable List: 
	Population-name: population code with reference to the population geographic location
	Population: population code with elevation
	Transect: transect to which population belongs, Transect 1 or Transect 2
	Individual: Individual ID code (e.g JUBHTX001; JUB corresponds to Jubones; HT to higher treatment temperature which is 28C; X that CTmax was estimate in that tadpole; 001 tadpole number)
	Elevation: population code for each of the six populations studied at both elevational gradients
	Treatment: temperature acclimation treatment (20, 24, or 28 C)
	thermal-limit: either CTmax or CTmin
	CT-value: estimate of thermal limit
	TL: tadpole total length
	BL: tadpole body length
	STAGE: tadpole Gosner's stage
	Year: if the experiment was done in 2014 or 2015 (only for transect 1 because all experiments in transect 2 were done in 2015)
	Days: days tadpole was maintained at the acclimation temperature before the estimation of thermal limit
	Month: month in which experiments were carried out
	HabTemp: mean of habitat temperature obtained with dataloggers
	sdhab: standard deviation of habitat temperature obtained with dataloggers

4. Missing data codes: 
	NA

5. Abbreviations used: 
	CT-value: estimate of thermal limit
	TL: tadpole total length
	BL: tadpole body length

6. Other relevant information: 
	None
