# GP_simulation
This repo contains code for running the GP simulation for sub pixel spatial variability of tundra snow
with the SMRT model. The Gaussian processes implementation is done with pymc3. 

## Snow Radiative transfer model
github.com/smrt-model/smrt

## From the paper
"Characterizing Tundra snow sub-pixel variability to improve brightness temperature estimation in satellite SWE retrievals"

Julien Meloche1,2, Alexandre Langlois1,2, Nick Rutter3, Alain Royer 1,2, Josh King4, Branden Walker5 

1 Centre d’Applications et de Recherche en Télédétection, Université de Sherbrooke, Sherbrooke, J1K 2R1, Canada
2 Centre d’études Nordiques, Université Laval, Québec, G1V 0A6, Canada
3 Department of Geography and Environmental Sciences, Northumbria University, Newcastle upon Tyne, NE1 8ST, UK
4 Environment and Climate Change Canada, Climate Research Division, Toronto, M3H 5T4, Canada
5 Cold Regions Research Centre, Wilfrid Laurier University, Waterloo, N2L 3C5, CanadaT

This paper is currently under review at https://tc.copernicus.org/preprints/tc-2021-156/

## library
* Python 3.7.6
* Numpy 1.16.4
* Pandas 0.25.1
* PyMC3 3.9.3
* scipy 1.3.1
* smrt 1.0

## How to use
* Use the GP_mean_simulation_Tb_CV.ipynb notebook to produce the GP simulation and mean simulation. The simulation output
are pickle objects. All *.csv files are used as input. 

* The Bias_simulation_mean_GP.ipynb notebook is used to calculate bias and rsme with measurement from the SSMIS satelitte sensor at 37GHz. Simualtion output objects and input. Tbh_measured.obj, Tbv_measured.obj are used as input.

* For the complete methodoloy, see the complete paper reference above.



