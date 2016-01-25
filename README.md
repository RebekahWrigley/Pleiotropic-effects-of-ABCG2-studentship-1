# Pleiotropic-effects-of-ABCG2-studentship
*R scripts detailing file organisation/subsetting and regression commands used in the studentship.*

## Overview
The general aim of this studentship was to investigate the relationship of ABCG2 variants (rs2231142 and rs10011796) with the immune response in gout.  This was meant to follow on from the Multiplicative interaction of functional inflammasome variants in determining the risk of gout paper (McKinney, 2015).  At first I used the same data as used in this paper (NZ gout cases and controls, Eurogout, AGRIA, ARIC and FHS) but later Tony asked me to add NPH, CARDIA, and CHS datasets.  I genotyped rs10011796 in NZ cases and controls and rs2231142 in AGRIA and some Eurogout boxes.  

Association of rs2231142, rs10011796, and rs11942223 (as a comparison from SLC2A9) with gout using only hyperuricemic controls, both hyperuricemic and normouricemic controls, and with hyperuricemia was investigated using logistic regression.  Europeans, EP, EP with 3 or more Polynesian grandparents, and WP were analysed separately.  Further analyses were performed in males only and in BMI strata.  

Interaction of rs2231142 and rs10011796 was investigated by including an interaction term in the logisitc regression model and looking at association of combined genotypes (minor allele carrier status) with gout.  LD between rs2231142 and rs10011796 in Europeans was determined using SNAP- these SNPs are not linked.  

Association of rs2043211 and rs1143623 with gout or hyperuricemia and interaction of rs2231142 or rs10011796 with these SNPs was also investigated.  

Association of rs2231142 and rs10011796 with urate in urate quartiles in Europeans looking at males and females separately was also investigated. No obvious diferrences in association between urate quartiles were found.  It is possible that relatedness was a problem in this analysis since PCA1 and PCA2 were not adjusted for as a combined dataset including FHS, ARIC, CARDIA, and CHS was used.  

## Exclusion criteria
Excluded people with kidney disease, on urate lowering therapy, related people in FHS generation 3.  People on diuretics are included since associations including and excluding people with diuretics were compared and there were no major differences.

## Where I got datasets from
- Big file from Cushla containing NZ cases and controls, AGRIA, Eurogout, ARIC, and FHS (both generations) with rs2231142, rs10011796, rs2043211, and rs1143623 genotype info (for ARIC and FHS these SNPs were reimputed).  I manually deleted MAS gout box 10 and AGRIA ST Vincent since these did not have FULLCAUGTAFF column info (so was not certain that these were European).

- rs2231142 and rs10011796 info for CARDIA and CHS from Jaron

- rs1194223 info for CARDIA and CHS from Jaron

- rs1194223 info for NZ cases and controls and NPH from Mandy

- Diuretic and pre urate lowering therapy urate info from Mandy and diuretic info for CHS from Jaron (merged this info with other files).



