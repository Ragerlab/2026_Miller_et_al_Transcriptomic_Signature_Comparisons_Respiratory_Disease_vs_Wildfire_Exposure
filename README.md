# 2026_Miller_et_al_Transcriptomic_Signature_Comparisons_Respiratory_Disease_vs_Wildfire_Exposure
Code associated with 'Transcriptomic signature comparisons identify conserved key events and respiratory disease signatures most similar to wildfire-relevant exposure' published in 2026 (PMID: tbd).

# Standard workflow:
1) A_WildfireSim_DataCleaning.Rmd -- This code reads in all source data associated with wildfire-relevant exposure in mice and respiratory disease in humans. Data cleaning steps include extracting and filtering data, consolidating duplicate genes across disparate source datasets, and converting exposure-associated mouse genes to their human orthologs to facilitate comparisons with human respiratory disease data.
2) B_WildfireSim_CountMatrix_MultipleMetrics_v2.Rmd -- This code defines each exposure- or disease-associated signature, combines these signatures into a binarized count matrix amenable to downstream analyses.
3) C_WildfireSim_MCA_v5.Rmd -- This code uses Multiple Correspondence Analysis (MCA) and other dimension reduction methods to analyze the aggregate exposure and disease signatures in addition to the subset of top shared genes identified as highly shared across both exposure and disease.
4) C_WildfireSim_PostAnalysisNeeds_MultipleMetrics_v2.Rmd -- This code 

# Sensitivity analyses:
## Alternative signature sizes workflow
1) A_WildfireSim_DataCleaning.Rmd -- See above.
2) B_WildfireSim_CountMatrix_MultipleMetrics_v2.Rmd -- See above.
3) CSupp_WildfireSim_PostAnalysisNeeds_MultipleMetrics_v2_SuppSigSizes.Rmd -- Same description as C_WildfireSim_PostAnalysisNeeds_MultipleMetrics_v2.Rmd above, but code has been modified to more easily read-out figures and files with prefixes that designate what signature size was used.

## LPS as a positive inflammatory control workflow
1) ASupp_WildfireSim_DataCleaning_addLPS.Rmd -- Same description as A_WildfireSim_DataCleaning.Rmd above, but code has been modified to accomodate the inclusion of LPS as an additional exposure signature.
2) BSupp_WildfireSim_CountMatrix_MultipleMetrics_v2_addLPS.Rmd -- Same description as B_WildfireSim_CountMatrix_MultipleMetrics_v2.Rmd above, but code has been modified to accomodate the inclusion of LPS as an additional exposure signature.
3) CSupp_WildfireSim_PostAnalysisNeeds_MultipleMetrics_v2_addLPS.Rmd -- Same description as C_WildfireSim_PostAnalysisNeeds_MultipleMetrics_v2.Rmd above, but code has been modified to accomodate the inclusion of LPS as an additional exposure signature.
