# Location
Converted effect sizes can be found at ./data/converted.

# Raw data
For datasets with raw data (mean, sd, n), the t values and df were exactly computed. The two quantities can be used to calculate pcc, correct and wrong SE(pcc) accordingly.

These include **dat_r_lnRR_list.RDS** (original effect measure was lnRR) and **dat_r_SMD_list.RDS** (original effect measure was SMD or *d* family).

**Metadata:**
*"study_ID"* - study identity
*"T_mean"* - mean of the treatment group
*"C_mean"* - mean of the control group
*"T_sd"* - sd of the treatment group 
*"C_sd"* - sd of the control group
*"T_n"*  - sample size or replicate of the treatment group
*"C_n"* - sample size or replicate of the control group
*"t"* - t value
*"df"* - degrees of freedom

# Pre-processed data
For datasets with pre-processed data, the original authors provided only effect size estimates and corresponding sampling variances in their publications. 
The pcc and df were approximated for datasets using SMD the measure, assuming the primary studies used equal designs. The t values and df were exactly calculated for datasets using *Zr* as the measure. The two quantities can be used to calculate correct and wrong SE(pcc) accordingly.

These include **dat_p_SMD_list** (original effect measure was SMD or *d* family) and **dat_p_Zr_list** (original effect measure was *Zr*).

**Metadata:**
*"study_ID"* - study identity
*"es"* - point estimate of the original effect size 
*"var"* - variance of the original effect size
*"pcc"* - converted pcc      
*"df"* - degrees of freedom

