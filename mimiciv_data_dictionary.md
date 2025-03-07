# Assignment 1 MIMIC-IV Data Dictionary

## Overview

This dataset contains first-day ICU patient data from MIMIC-IV, designed for two predictive tasks:

1. **Classifying the most severe Acute Kidney Injury (AKI) stage** a patient will experience during their ICU stay.
2. **Predicting hospital mortality**.

### **Identifiers & Outcomes**

·    **id**: Unique patient identifier.

·    **hospital_mortality**: Binary indicator (0=alive, 1=deceased) of whether the patient died during hospitalization.

·    **aki_stage**: Most severe **Acute Kidney Injury (AKI) stage** the patient reached during ICU stay (0 = No AKI, 1-3 = Increasing severity levels).

### **Demographics**

·    **gender**: Patient’s gender.

·    **admission_age**: Age at hospital admission.

·    **race**: Self-reported racial/ethnic category.

### **Vital Signs**

·    **heart_rate_min, heart_rate_max, heart_rate_mean**: Heart rate (beats per minute).

·    **sbp_min, sbp_max, sbp_mean**: Systolic blood pressure (mmHg).

·    **dbp_min, dbp_max, dbp_mean**: Diastolic blood pressure (mmHg).

·    **mbp_min, mbp_max, mbp_mean**: Mean arterial pressure (mmHg).

·    **resp_rate_min, resp_rate_max, resp_rate_mean**: Respiratory rate (breaths per minute).

·    **temperature_vital_min, temperature_vital_max, temperature_vital_mean**: Body temperature (°C or °F).

·    **spo2_min, spo2_max, spo2_mean**: Oxygen saturation in the blood (%).

·    **glucose_vital_min, glucose_vital_max, glucose_vital_mean**: Bedside blood glucose (mg/dL).

### **Blood Gas Parameters (from Blood Gas Tests)**

·    **lactate_min, lactate_max**: Lactate levels (indicator of tissue hypoxia, mg/dL).

·    **ph_min, ph_max**: Blood pH (acidity or alkalinity of blood).

·    **so2_min, so2_max**: Oxygen saturation measured from blood gas (%).

·    **po2_min, po2_max**: Partial pressure of oxygen (mmHg).

·    **pco2_min, pco2_max**: Partial pressure of carbon dioxide (mmHg).

·    **aado2_min, aado2_max**: Alveolar-arterial oxygen gradient (mmHg, used to assess lung function).

·    **aado2_calc_min, aado2_calc_max**: Calculated alveolar-arterial oxygen gradient.

·    **pao2fio2ratio_min, pao2fio2ratio_max**: Ratio of arterial oxygen partial pressure to fractional inspired oxygen (assesses respiratory failure severity).

·    **baseexcess_min, baseexcess_max**: Base excess in blood (marker of metabolic acidosis/alkalosis).

·    **bicarbonate_bg_min, bicarbonate_bg_max**: Bicarbonate levels (key acid-base balance component, mmol/L).

·    **totalco2_min, totalco2_max**: Total carbon dioxide levels.

·    **hematocrit_bg_min, hematocrit_bg_max**: Percentage of red blood cells in blood.

·    **hemoglobin_bg_min, hemoglobin_bg_max**: Hemoglobin concentration (g/dL, oxygen-carrying protein in red blood cells).

·    **carboxyhemoglobin_min, carboxyhemoglobin_max**: Carboxyhemoglobin level (indicates carbon monoxide exposure or smoking history).

·    **methemoglobin_min, methemoglobin_max**: Methemoglobin level (abnormal hemoglobin form affecting oxygen transport).

·    **temperature_bg_min, temperature_bg_max**: Blood temperature (°C or °F).

·    **chloride_bg_min, chloride_bg_max**: Chloride levels (electrolyte balance, mmol/L).

·    **calcium_bg_min, calcium_bg_max**: Blood calcium levels (important for heart, muscle, and nerve function, mg/dL).

·    **glucose_bg_min, glucose_bg_max**: Blood glucose from blood gas analysis (mg/dL).

·    **potassium_bg_min, potassium_bg_max**: Potassium levels (electrolyte critical for heart and muscle function, mmol/L).

·    **sodium_bg_min, sodium_bg_max**: Sodium levels (electrolyte balance, mmol/L).

### **Laboratory Test Results**

·    **hematocrit_lab_min, hematocrit_lab_max**: Hematocrit percentage from lab tests.

·    **hemoglobin_lab_min, hemoglobin_lab_max**: Hemoglobin concentration from lab tests.

·    **platelets_min, platelets_max**: Platelet count (cells responsible for clotting, 10³/μL).

·    **wbc_min, wbc_max**: White blood cell count (immune response, 10³/μL).

·    **albumin_min, albumin_max**: Albumin (key blood protein, low levels indicate malnutrition or liver/kidney disease, g/dL).

·    **globulin_min, globulin_max**: Globulin (immune system protein, g/dL).

·    **total_protein_min, total_protein_max**: Total serum protein levels (g/dL).

·    **aniongap_min, aniongap_max**: Anion gap (used to detect acid-base disorders, mmol/L).

·    **bicarbonate_lab_min, bicarbonate_lab_max**: Bicarbonate from lab tests.

·    **bun_min, bun_max**: Blood urea nitrogen (marker of kidney function, mg/dL).

·    **calcium_lab_min, calcium_lab_max**: Blood calcium from lab tests.

·    **chloride_lab_min, chloride_lab_max**: Chloride from lab tests.

·    **creatinine_min, creatinine_max**: Creatinine levels (marker of kidney function, mg/dL).

·    **glucose_lab_min, glucose_lab_max**: Blood glucose from lab chemistry tests.

·    **sodium_lab_min, sodium_lab_max**: Sodium from lab tests.

·    **potassium_lab_min, potassium_lab_max**: Potassium from lab tests.

### **Complete Blood Count & Coagulation Markers**

·    **abs_basophils_min, abs_basophils_max**: Absolute basophil count (involved in allergic reactions).

·    **abs_eosinophils_min, abs_eosinophils_max**: Absolute eosinophil count (related to allergies and parasitic infections).

·    **abs_lymphocytes_min, abs_lymphocytes_max**: Absolute lymphocyte count (key immune cells).

·    **abs_monocytes_min, abs_monocytes_max**: Absolute monocyte count (inflammation and immune response).

·    **abs_neutrophils_min, abs_neutrophils_max**: Absolute neutrophil count (first-line infection fighters).

·    **inr_min, inr_max**: International Normalized Ratio (INR, blood clotting time measure).

·    **pt_min, pt_max**: Prothrombin time (PT, clotting function test).

·    **ptt_min, ptt_max**: Partial thromboplastin time (PTT, evaluates clotting disorder risk).

·    **d_dimer_min, d_dimer_max**: D-dimer (marker for blood clot formation, ng/mL).

·    **fibrinogen_min, fibrinogen_max**: Fibrinogen (clotting protein, mg/dL).

·    **thrombin_min, thrombin_max**: Thrombin time (clotting function test, seconds).

### **Liver & Cardiac Markers**

·    **alt_min, alt_max**: Alanine transaminase (ALT, liver enzyme, marker of liver damage).

·    **alp_min, alp_max**: Alkaline phosphatase (ALP, liver and bone enzyme).

·    **amylase_min, amylase_max**: Amylase (enzyme related to digestion, U/L).

·    **ast_min, ast_max**: Aspartate transaminase (AST, liver and heart enzyme).

·    **bilirubin_total_min, bilirubin_total_max**: Total bilirubin (indicator of liver function and red blood cell breakdown).

·    **bilirubin_indirect_min, bilirubin_indirect_max**: Indirect bilirubin (component of total bilirubin, mg/dL).

·    **ck_cpk_min, ck_cpk_max**: Creatine kinase (CK, muscle and heart damage marker).

·    **ck_mb_min, ck_mb_max**: CK-MB (Creatine kinase-MB, heart muscle damage marker, U/L).

·    **ggt_min, ggt_max**: Gamma-glutamyl transferase (GGT, liver enzyme, U/L).

·    **ld_ldh_min, ld_ldh_max**: Lactate dehydrogenase (LDH, tissue damage marker, U/L).

### **C**omplete Blood Count & Immature Cells

·    **a****typs_min, atyps_max**: Atypical lymphocytes (abnormal white blood cells, %).

·    **ba****nds_min, bands_max**: Band neutrophils (immature neutrophils, %, infection response marker).

·    **imm_granulocytes_min, imm_granulocytes_max: Immature granulocytes (early-stage white blood cells, %, inflammation marker).**

·    **metas_min, metas_max**: Metamyelocytes (immature neutrophils, %, infection response marker).

·    **nrbc_min, nrbc_max**: Nucleated red blood cells (abnormal RBC precursors, %, severe illness indicator).

### **Neurological & Anthropometric Data**

·    **gcs_min**: Glasgow Coma Scale total score (neurological function assessment).

·    **gcs_motor**: Glasgow Coma Scale motor response score.

·    **gcs_verbal**: Glasgow Coma Scale verbal response score.

·    **gcs_eyes**: Glasgow Coma Scale eye-opening response score.

·    **gcs_unable**: Indicator if GCS score was unable to be assessed.

·    **height**: Patient height (cm).

·    **weight_admit**: Admission weight (kg).