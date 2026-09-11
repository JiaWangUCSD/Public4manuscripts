# Range-dependent Radar Reflectivity Innovations over the Contiguous United States

This repository contains the **plotting scripts** used to generate the figures in the manuscript:
> **Range-dependent Radar Reflectivity Innovations over the Contiguous United States**  
> *Authors: Jia Wang, Minghua Zheng, Jonathan Rutz, Luca Delle Monache, and Fred Martin Ralph*  
> *Journal: Geophysical Research Letters* 

## Manuscript Figures

The scripts in this repository reproduce the following figures from the manuscript:

| Figure | Description | Script | Dataset | Command |
|---|---|---|---|---|
| **Figure 1b** | Radar beam diameter at 1 km AGL                                                                                    | `f1.bsh`  | <details><summary>Show dataset</summary><br><code>HRRR_HRRR1and4kmAGL.GridRadarInfo.CONUS.nc</code></details> | <details><summary>Show command</summary><br><code>./f1.bsh CONUS HRRR HRRR1and4kmAGL CONUS</code></details> |
| **Figure 2**  | Spatial distribution of median reflectivity innovations during summer and winter                                   | `f2.bsh`  | <details><summary>Show datasets (2 files)</summary><br><ul><li><code>ZPH.OmBhrrr.Climatology_AllyearJJA.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.CONUS.fromFortran.nc</code></li><li><code>ZPH.OmBhrrr.Climatology_AllyearDJF.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.CONUS.fromFortran.nc</code></li></ul></details> | <details><summary>Show command</summary><br><code>./f2.bsh MergedReflectivityQCComposite MergedReflectivityQC PrecipRate 'AllyearJJA,AllyearDJF' 1 zOmB 100 calc.stats.ZPH.v1.f90 CONUS</code></details> |
| **Figure 3**  | Median reflectivity innovations as a function of radar beam diameter and distance from the HRRR freezing level     | `f3.bsh`  | <details><summary>Show dataset (4 files)</summary><br><ul><li><code>ZPH.OmBhrrr.Climatology_AllyearDJF.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.CONUS.fromFortran.nc</code></li><li><code>ZPH.OmBhrrr.Climatology_AllyearDJF.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.PNWCA.fromFortran.nc</code></li><li><code>ZPH.OmBhrrr.Climatology_AllyearDJF.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.NorthEast.fromFortran.nc</code></li><li><code>ZPH.OmBhrrr.Climatology_AllyearDJF.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.SouthEast.fromFortran.nc</code></li></ul></details> | <details><summary>Show command</summary><br><code>./f3.bsh MergedReflectivityQCComposite MergedReflectivityQC PrecipRate AllyearDJF 1 Zconus 100 calc.stats.ZPH.v1.f90 CONUS PNWCA NorthEast SouthEast</code></details> |
| **Figure 4**  | Median observed, analyzed, and simulated reflectivity                                                              | `f4.bsh`  | <details><summary>Show datasets (2 files)</summary><br><ul><li><code>ZPH.OmBhrrr.Climatology_AllyearJJA.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.CONUS.fromFortran.nc</code></li><li><code>ZPH.OmBhrrr.Climatology_AllyearDJF.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.CONUS.fromFortran.nc</code></li></ul></details> | <details><summary>Show command</summary><br><code>./f4.bsh MergedReflectivityQCComposite MergedReflectivityQC PrecipRate 'AllyearJJA,AllyearDJF' 1 'zO,zB' 100 calc.stats.ZPH.v1.f90 CONUS</code></details> |
| **Figure 5**  | Averaged observation-minus-background differences in reflectivity and composite reflectivity for two winter storms | `f5.bsh`  | <details><summary>Show datasets (2 files)</summary><br><ul><li><code>ZPH.OmBhrrr.Climatology_case2023Jan.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.CONUS.fromFortran.nc</code></li><li><code>ZPH.OmBhrrr.Climatology_case2026Jan.EveryLeadTime.MergedReflectivityQCComposite_PrecipRate.opt4thresh_1.CONUS.fromFortran.nc</code></li></ul></details> | <details><summary>Show command</summary><br><code>./f5.bsh MergedReflectivityQCComposite MergedReflectivityQC PrecipRate 'case2023Jan,case2026Jan' 1 'zOmB,mdbzOmB' 3 calc.stats.ZPH.v1.f90 CONUS</code></details> |


## Data Availability

The datasets required to reproduce the manuscript figures are archived on Zenodo:

**Zenodo:** https://zenodo.org/records/22698766


