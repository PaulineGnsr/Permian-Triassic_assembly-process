# Welcome to this repository! 

Here are gathered the input and output material used in Guenser _et al._ (accepted in Lethaia) and associated datapaper [Guenser _et al._ (in review in PCI Paleo)](https://hal.science/hal-04951445). With this material you can:

- reproduce the results/figures from the two publications
- reuse the dataset and/or the script for your own analyses

Don't forget there are two other repositories specifically for the [Occurrence Ratio Profile](https://github.com/PaulineGnsr/ORP_analysis) (ORP) and the [Bootstrap Spanning Network](https://github.com/PaulineGnsr/BSN_analysis) (BSN) analyses.

Please, do not hesitate to contact me if you want to report any bug, inconsistency, or typo.

# Description of the folders

## _Database conodonts_

In this folder you will find the database of terminal Permian-Early Triassic conodont occurrences. These information are available in three different formats (CSV, TXT, XLSX).

For an exhaustive description of the database, please refer to the datapaper [Guenser _et al._ (in review in PCI Paleo)](https://hal.science/hal-04951445)

This database has been built with informations published before 2023. It will be updated yearly with new publications and the new version of the database will be uploaded with a specific name.  

## _Dataset ammonoids_
In this folder you will find the presence/absence matrices (in CSV format) of terminal Permian-Early Triassic ammonoid genera in basinal regions following [Dai & Song (2020)](https://doi.org/10.1017/pab.2020.40). 
There are five incidence matrices entitled _ammo_Ch_, _ammo_Gr_, _ammo_Di_, _ammo_Sm_ and _ammo_Sp_ respectively for the Changhsingian, the Griesbachian, the Dienerian, the Smithian and the Spathian.
The CSV file _ammo_paleocoord_ comprises the paleocoordinates of the regions where ammonoid occurred.

## _Datapaper_PCI Paleo_
In this folder you will find the graphical outputs from the datapaper [Guenser _et al._ (in review in PCI Paleo)](https://hal.science/hal-04951445). The R code to produce these figures is available in the rmarkdown file _Conodont_analyses.rmd_.

## _Rmarkdown scripts_
In this folder you will find the R code used to perform the analyses on conodont and ammonoid datasets, as well as outputs (data and figures).
  
### _Conodont_
- _Conodont_analyses.rmd_: R script used to analyse conodont occurrences
- _Low_Trias.csv_: Absolute ages of Early Triassic substages

#### _Output_: graphical and data outputs from the R script
- DATA (CSV files):
  - _Section_paleocoord_conodont_: list of conodont sections and their associated paleocoordinates. Their resulting region is added manually in the light of the UPGMA classification to build Table S2.
  - _Incidence matrix_no singleton_conodont_...: output presence/absence matrix of conodonts
  - _PCoA axes_conodont_: variance percentages for each axis from PCoA analyses performed on conodonts [Figure 4]
  - _BSN_data_conodont_...: raw output of the BSN analyses performed on conodonts [Figure 4]
  - _SIMPER_data_conodont_...: raw outputs of SIMPER analyses performed on conodonts [Figure 6]
  - _DNCI_data_conodont_: raw output of the DNCI analyses performed on conodonts [Figure 10]
- GRAPHICS (SVG files):
  - _paleomap_sectons_raw_conodont_: raw paleomapping of conodont sections from the database [Figure S1]
  - _paleomap_sections_clean_conodont_: paleomapping of conodont sections after revising the paleolocation of Japanese, Timor and Bulgarian sections [Figure S1]
  - _UPGMA_tree_section_conodont_: dendrogram of conodont sections used to define regions [Figure S2]
  - _paleomap_regions_conodont_: mapping of mean regions paleocoordinates from conodont occurrences [Figure 1A]
  - _Species accumulation curve_conodont_: from conodont occurrences [Figure S3A]
  - _Sampling coverage_conodont_: from conodont occurrences [Figure S3B]
  - _ORP_conodont_: graphic output of ORP anayses on conodonts [Figure 3]
  - _PCoA_UPGMA_conodont_no singleton_: graphic output of combined PCoA and UPGMA classification performed on conodonts [Figure 4]
  - _BSN_conodont_...: graphic output of BSN analyses on conodonts [Figure 4]
  - _SIMPER_conodont_...: graphic outputs of the SIMPER analyses performed on conodonts [Figure 6]
  - _DNCI_conodont_: graphic output of DNCI analyses on conodonts [Figure 10]

### _Ammonoid_
- _Ammonoid_analyses.rmd_: R script used to analyse ammonoid occurrences

#### _Output_: graphical and data outputs from the R script
- DATA (CSV files):
  - _PCoA axes_ammonoid_: variance percentages for each axis from PCoA analyses performed on ammonoids [Figure 7]
  - _BSN_data_ammonoid_...: raw output of the BSN analyses performed on ammonoids [Figure 7]
  - _SIMPER_data_ammonoid_...: raw outputs of SIMPER analyses performed on ammonoids [Figure 9]
  - _DNCI_data_ammonoid_: raw output of the DNCI analyses performed on ammonoids [Figure 10]
- GRAPHICS (SVG files):
  - _paleomap_sectons_raw_ammonoid_: paleomapping of ammonoid regions from Dai & Song (2020) and additional revisions (see Material & Methods from Guenser _et al._ 2025) [Figure 1B]
  - _ORP_ammonoid_: graphic output of ORP anayses on ammonoids [Figure 3]
  - _PCoA_UPGMA_ammonoid_no singleton_: graphic output of combined PCoA and UPGMA classification performed on ammonoids [Figure 7]
  - _BSN_ammonoid_...: graphic output of BSN analyses on ammonoids [Figure 7]
  - _SIMPER_ammonoid_...: graphic outputs of the SIMPER analyses performed on ammonoids [Figure 9]
  - _DNCI_ammonoid_: graphic output of DNCI analyses on ammonoids [Figure 10]

## _Supplementary_
In this folder you will find supplementary tables and output BSN data used in Guenser _et al._ (accepted in Lethaia):
  - _Table S1_List of synonymes and discarded species.xls_
  - _Table S2_Section_paleocoord_regions_conodont.csv_
  - _Table S3_paleocoord_regions_ammonoids.csv_
  - CSV files _BSN_data_: output values from the BSN analyses performed on conodonts and ammonoids. The bootstrap support values might lightly differ from those available in the subfolder Rmarkdown scripts > Conodont > Output, because of the bootstrap resampling. However, these differences do not change the interpretation of the results.
