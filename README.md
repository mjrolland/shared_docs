<!-- ## 22-11-2019 meeting agenda & docs

Here are the different documents for the 22-11-19 meeting.

### 1. Sepages data

#### Imputation below LOD

* Previous doc justifying the fill-in method (no need to review): [imputation_below_lod_2019-11-20](docs/imputation_below_lod_2019-11-20.html)
* Validation of the fill-in method: [fill_in_vs_machine_reading_2019-11-20](docs/fill_in_vs_machine_reading_2019-11-20.html)

#### Correction for protocol variables

* phenols: [protocol_variables_vs_phenols_2019-11-20](docs/protocol_variables_vs_phenols_2019-11-20.html)
* phthalates: [protocol_variables_vs_phthalates_2019-11-20](docs/protocol_variables_vs_phthalates_2019-11-20.html)

### 2. BPA/BPS VS Growth 

* Variable coding document update: [variable_coding_2019-11-20](docs/variable_coding_2019-11-20.html)
* Preliminary results: [multivariate_model_2019-11-20](docs/multivariate_model_2019-11-20.html) 

# BPA/BPS growth - 12/12/19 meeting

Last version of multivariate models: [multivariate_model_2019-12-11](docs/multivariate_model_2019-12-11.html) -->

# Meeting Climathes 26/06/2020

## 1. Last version of the DAG

* Parity -> gest age?
* Pollution / humidity -> gest age?

![](docs/dagitty-model_2020-06-25.png)

## 2. Cohort comparison

[cohort_comparison_2020-06-25](docs/cohort_comparison_2020-06-25.html)

## 3. Temperature exposure description 

* Confirm we just use the `*_gro` files

[description_expos_2020-06-25](docs/description_expos_2020-06-25.html)

## 4. Discuss files

* adresses?
* difference between `Expo_prenat_*` and `Temp*` 

```
> fs::dir_tree(path = "data/expos/")
data/expos/
+-- Expo_prenat_EDEN
|   +-- expo_prenat_EDEN_SAFRAN_03062020.rds
|   +-- expo_prenat_EDEN_temp1km_03062020.rds
|   \-- expo_prenat_EDEN_temp200m_03062020.rds
+-- Expo_prenat_PELAGIE
|   +-- expo_prenat_PELAGIE_gro_SAFRAN_03062020.rds
|   +-- expo_prenat_PELAGIE_gro_temp1km_03062020.rds
|   +-- expo_prenat_PELAGIE_gro_temp200m_03062020.rds
|   +-- expo_prenat_PELAGIE_Q2_SAFRAN_03062020.rds
|   +-- expo_prenat_PELAGIE_Q2_temp1km_03062020.rds
|   +-- expo_prenat_PELAGIE_Q2_temp200m_03062020.rds
|   +-- expo_prenat_PELAGIE_Q6_SAFRAN_03062020.rds
|   +-- expo_prenat_PELAGIE_Q6_temp1km_03062020.rds
|   \-- expo_prenat_PELAGIE_Q6_temp200m_03062020.rds
+-- fichier_eden_pr_calcul_01062020.rds
+-- fichier_pelagie_grossesse_pr_calcul_01062020.rds
+-- fichier_pelagie_Q2_pr_calcul_01062020.rds
+-- fichier_pelagie_Q6_pr_calcul_01062020.rds
+-- NDVI_EDEN
|   \-- NDVI_EDEN_03062020.rds
+-- NDVI_PELAGIE
|   +-- NDVI_PELAGIE_gro_03062020.rds
|   +-- NDVI_PELAGIE_Q2_03062020.rds
|   \-- NDVI_PELAGIE_Q6_03062020.rds
+-- SAFRAN_EDEN
|   +-- EDEN_dates_01062020.rds
|   +-- EDEN_HA_01062020.rds
|   +-- EDEN_HR_01062020.rds
|   \-- EDEN_vent_01062020.rds
+-- SAFRAN_PELAGIE
|   +-- PELAGIE_gro_dates_01062020.rds
|   +-- PELAGIE_gro_HA_01062020.rds
|   +-- PELAGIE_gro_HR_01062020.rds
|   +-- PELAGIE_gro_vent_01062020.rds
|   +-- PELAGIE_Q2_dates_01062020.rds
|   +-- PELAGIE_Q2_HA_01062020.rds
|   +-- PELAGIE_Q2_HR_01062020.rds
|   +-- PELAGIE_Q2_vent_01062020.rds
|   +-- PELAGIE_Q6_dates_01062020.rds
|   +-- PELAGIE_Q6_HA_01062020.rds
|   +-- PELAGIE_Q6_HR_01062020.rds
|   \-- PELAGIE_Q6_vent_01062020.rds
+-- Temp1km_EDEN
|   +-- eden_temp_1km_matrices_dates_01062020.rds
|   +-- eden_temp_1km_matrices_tmax_01062020.rds
|   +-- eden_temp_1km_matrices_tmean_01062020.rds
|   \-- eden_temp_1km_matrices_tmin_01062020.rds
+-- Temp1km_PELAGIE
|   +-- PELAGIE_gro_temp_1km_matrices_dates_01062020.rds
|   +-- PELAGIE_gro_temp_1km_matrices_tmax_01062020.rds
|   +-- PELAGIE_gro_temp_1km_matrices_tmean_01062020.rds
|   +-- PELAGIE_gro_temp_1km_matrices_tmin_01062020.rds
|   +-- PELAGIE_Q2_temp_1km_matrices_dates_01062020.rds
|   +-- PELAGIE_Q2_temp_1km_matrices_tmax_01062020.rds
|   +-- PELAGIE_Q2_temp_1km_matrices_tmean_01062020.rds
|   +-- PELAGIE_Q2_temp_1km_matrices_tmin_01062020.rds
|   +-- PELAGIE_Q6_temp_1km_matrices_dates_01062020.rds
|   +-- PELAGIE_Q6_temp_1km_matrices_tmax_01062020.rds
|   +-- PELAGIE_Q6_temp_1km_matrices_tmean_01062020.rds
|   \-- PELAGIE_Q6_temp_1km_matrices_tmin_01062020.rds
+-- Temp200m_EDEN
|   +-- eden_temp_200m_matrices_dates_02062020.rds
|   +-- eden_temp_200m_matrices_tmax_02062020.rds
|   +-- eden_temp_200m_matrices_tmean_02062020.rds
|   \-- eden_temp_200m_matrices_tmin_02062020.rds
+-- Temp200m_PELAGIE
|   +-- PELAGIE_gro_temp_200m_matrices_dates_02062020.rds
|   +-- PELAGIE_gro_temp_200m_matrices_tmax_02062020.rds
|   +-- PELAGIE_gro_temp_200m_matrices_tmean_02062020.rds
|   +-- PELAGIE_gro_temp_200m_matrices_tmin_02062020.rds
|   +-- PELAGIE_Q2_temp_200m_matrices_dates_02062020.rds
|   +-- PELAGIE_Q2_temp_200m_matrices_tmax_02062020.rds
|   +-- PELAGIE_Q2_temp_200m_matrices_tmean_02062020.rds
|   +-- PELAGIE_Q2_temp_200m_matrices_tmin_02062020.rds
|   +-- PELAGIE_Q6_temp_200m_matrices_dates_02062020.rds
|   +-- PELAGIE_Q6_temp_200m_matrices_tmax_02062020.rds
|   +-- PELAGIE_Q6_temp_200m_matrices_tmean_02062020.rds
|   \-- PELAGIE_Q6_temp_200m_matrices_tmin_02062020.rds
+-- Urba_EDEN
|   +-- EDEN_urba_03062020.rds
|   \-- EDEN_urba_dates_03062020.rds
\-- Urba_PELAGIE
    +-- PELAGIE_gro_urba_03062020.rds
    +-- PELAGIE_gro_urba_dates_03062020.rds
    +-- PELAGIE_Q2_urba_03062020.rds
    +-- PELAGIE_Q2_urba_dates_03062020.rds
    +-- PELAGIE_Q6_urba_03062020.rds
    \-- PELAGIE_Q6_urba_dates_03062020.rds

```

## 5. To do/questions

* continue exposure description (what?)
* finalise Sepages variables (check notes from previous meeting with Johanna: marital status, country of birth etc)
* write to pelagie with the list of questions (cf. project log + [github note](https://github.com/users/matthieugold/projects/16))
* look at humidity, pollution, location (urbain/rural) 
* write analysis plan
  * define what indicators for temperature?
* do some methods bibliography


