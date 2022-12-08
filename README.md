# focal_niche_divergence_analysis

#The R markdown files provided here allows reproduction of the analysis found in DePasquale et al, in revision at the American Naturalist. 

I provide 5 files:
1) "GLMMs_AmNat_Revised.Rmd"
2) "RMT_NDF.Rmd"
3) "RMT_no_NDF.Rmd"
4) "AmNat_Niche_Overlap.Rmd"
5) "AmNat_Figures.Rmd"

I detail each in turn below.

1) "GLMMs_AmNat_Revised.Rmd"

This file provides the code for the generalized linear mixed models and estimated marginal means reported in the manuscript. The GLMMs analyze bite count and grams of nutrient intake.

The data files necessary for running this script are:

"Complete_Bite_DF_July_1_2022.csv" --> dataframe containing bite counts per focal

"ColourCategoriesBroadFeb102022.csv" --> dataframe containing broad food categories (fruit versus invertebrate) for plotting

"Complete_Nutrition_DF_Jul1_2022.csv" --> dataframe containing grams of macronutrient intake per focal

2) "RMT_NDF.Rmd"

This file provides the code for the right angled mixture triangles (RMTs) that contain neutral detergent fiber, typically a feeding deterrent in primates. These RMTs can be found in the manuscript as Supplemental Figure 1.

The data files necessary for running this script are:

"food_RMT_NDF.csv" --> dataframe containing percentages of macronutrient contributions (carbs+fat, protein, fiber) to metabolizable energy for each food taxon

"Complete_Nutrition_DF_Jul1_2022.csv" --> dataframe containing grams of macronutrient intake per focal

3) "RMT_no_NDF.Rmd"

This file provides the code for the right angled mixture triangles that appear in the main manuscript as Figure 4. These RMTs visualize how the food items and the intake of the focal animals breakdown in terms of percent contributions of fat, carbs, and protein to metabolizable energy

The data files necessary for running this script are:

"food_RMT.csv" --> dataframe containing percentages of macronutrient contributions (carbs, fat, protein) to metabolizable energy for each food taxon

"Complete_Nutrition_DF_Jul1_2022.csv" --> dataframe containing grams of macronutrient intake per focal


4) "AmNat_Niche_Overlap.Rmd"

This file details the Pianka index analysis used to measure niche overlap. This script generates EMMs and explains how to use the EcoSimR Niche Overlap shell from http://www.uvm.edu/~ngotelli/EcoSim/EcoSim.html to generate Pianka indices for high and low fruit months using the following EMMs

The data files necessary for running this script are:

"RevisedPiankaEMM_Low_Jul12.csv" --> dataframe containing EMMs of bites taken by dichromats and trichromats of top 15 food taxa in low fruit months

"RevisedPiankaEMM_High_Jul12.csv" --> dataframe containing EMMS of bites taken by dichromats and trichromats of top 15 food taxa in high fruit months


5) "AmNat_Figures.Rmd"

This file generates Figure 1, displaying fruit biomass broken down by color classification, and Figure S2, displaying how bites and dry matter intake are proportioned in high and low fruit months

The data files necessary for running this script are:

"FruitBiomassByTaxon.csv" --> dataframe containing 2019 monthly fruit biomass scores for every taxon + their color classification + monthly fruit abundance category

"Bite_Percent_FigS1.csv" --> dataframe containing percentage of bites taken by dichromats and trichromats for different fruit + invert categories in high and low periods

"DM_Percent_FigS1.csv" --> dataframe containing percentage of dry matter intake consumed by dichromats and trichromats for different fruit + invert categories in high and low periods
