# Analyzing Relationship Between Glomerular Properties and Clinical Metadata - Client Project

This repository contains the code and documentation for a client-facing project as a part of ENGR-E 583 course undertaken at IUB as a part of Master's in Data Science. It is aimed at investigating the variation in size, shape, and distribution of glomeruli in the kidneys of donors, and how they relate to clinical metadata such as race, age, sex, body surface area (BSA), and body mass index (BMI).

## Project Overview:
The goal of this project was to analyze a dataset of 20 microscopic images of sections of donor kidneys, provided by the HuBMAP project [7], and annotated with glomerular and cortical borders in associated segmentation masks. The polygonal vertices of the glomerular and cortex annotations were processed to yield glomerular area (GA) and shape data (eccentricity, ECC) for the glomeruli and area data for the cortex. This data was processed to give measures as statistical data regarding GA and ECC as well as glomerular area ratio (GAR) (total glomerular area/cortical area) and glomerular density (GD) (count of glomeruli/cortical area) for each donor.

The data was then compared across the 12 donors and their demographics (age, race, body mass index (BMI), body surface area ( BSA), medical history) with visualizations made using Power BI. The comparison focused on parameters affecting renal function such as age, race, sex, and medical history. No measure of renal function such as glomerular filtration rate (GFR) or serum creatinine (SCreat) was in the dataset, so a portion of the Modification of Diet in Renal Disease (MDRD) equation was used to estimate renal function independent of SCreat.

## Project Findings
The main findings of the project were:

* GA decreases with age
* BMI and BSA did not correlate with any of the measures 
* Trends relating race and sex were postulated but not significant
* linear combinations of age power curve from GA, race, and sex simulated the MDRD equation with significance
* hypertension (HTN) likely reduces GAR.

The scripts and the documentation of the summarized results, analysis and conclusions can be found in the above repository.
