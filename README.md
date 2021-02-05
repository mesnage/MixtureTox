# MixtureTox

Code for the study on pesticide mixture toxicity

The study metadata is a table containing all the study identifiers as File S1. 

#### Water consumption	

The daily water consumption per cage was measured before the start of the experiment, and weekly for all the duration of the treatment (13 weeks). Before the final sacrifice and after about 16 hours in metabolic cage, water consumption, was registered for each animal. The means of individual consumptions and related standard deviation were calculated for every group and for sex.

Raw data for water consumption is available as File S2

#### Food consumption

The daily food consumption per cage was measured before the start of the experiment, and weekly for all the duration of the treatment (13 weeks). Before the final sacrifice and after about 16 hours in metabolic cage, water consumption, was registered for each animal. The means of individual consumptions and related standard deviation were calculated for every group and for sex.

Raw data for food consumption is available as File S3.

#### Body weights

Body weight of experimental animals was measured before the start of the treatment, and then weekly for 13 weeks. All the experimental animals were weighted just before the sacrifice. Average body weights and related standard deviations were calculated for each experimental group.

Raw data for food consumption is available as File S4

#### Serum biochemistry
Serum biochemistry was performed under contract by IDEXX BioAnalytics (Stuttgart, Germany), an ISO 17025 accredited laboratory. Briefly, sodium and potassium levels were measured by indirect potentiometry. Albumin was measured by a photometric bromocresol green test. ALP was measured by IFCC with AMP-buffer method, glucose by Enzymatic UV-Test (hexokinase method), cholesterol by Enzymatic color test (CHOD-PAP), blood urea nitrogen by enzymatic UV-Test, gamma-glutamyl-transferase by Kinetic color test International Federation of Clinical Chemistry (IFCC), aspartate and alanine aminotransferase by kinetic UV-test (IFCC+ pyridoxal-5-phosphate), creatinine by kinetic color test (Jaffe’s method), lactate dehydrogenase by IFCC method, and triglycerides using an enzymatic color test (GPO-PAP) on a Beckman Coulter AU 480.

Raw data for food consumption is available as File S5

#### Serum metabolomics

Serum Metabolomics analysis was conducted under contract with Metabolon Inc. (Durham, NC, USA) on four independent instrument platforms as previously described: two different separate reverse phase ultrahigh performance liquid chromatography-tandem mass spectroscopy analysis (RP/UPLC-MS/MS) with positive ion mode electrospray ionization (ESI), a RP/UPLC-MS/MS with negative ion mode ESI, as well as by hydrophilic-interaction chromatography (HILIC)/UPLC-MS/MS with negative ion mode ESI.

- The raw data for the peak intensity is available as File S10. 
- The metadata describing annotation, mass and RI is available as File S9.
- The scaled and imputed data is available as File S11.
- The results are available as File S12

Scaled and imputed peak area values were log transformed, and statistical significance determined using a Welch’s two-sample t-test adjusted for multiple comparisons with FDR methods using the R package ‘qvalue’. The hypergeometric P-values were computed using the R package Hypergeo. We also used orthogonal partial least squares discriminant analysis (OPLS-DA) to evaluate the predictive ability of each omics approach. The R package ropls version 1.20.0 was used. This algorithm uses the nonlinear iterative partial least squares algorithm (NIPALS). Since PLS-DA methods are prone to overfitting, we assessed the significance of our classification using permutation tests (permuted 1,000 times).

The raw data is available in Metabolights, with the accession number MTBLS138 (https://www.ebi.ac.uk/metabolights/MTBLS138).

#### Caecum metabolomics

Caecum Metabolomics analysis was conducted under contract with Metabolon Inc. (Durham, NC, USA) on four independent instrument platforms as previously described: two different separate reverse phase ultrahigh performance liquid chromatography-tandem mass spectroscopy analysis (RP/UPLC-MS/MS) with positive ion mode electrospray ionization (ESI), a RP/UPLC-MS/MS with negative ion mode ESI, as well as by hydrophilic-interaction chromatography (HILIC)/UPLC-MS/MS with negative ion mode ESI.

The raw data for the peak intensity is available as File S7.
The metadata describing annotation, mass and RI is available as File S6.
The scaled and imputed data is available as File S8.
Results are available as file S13

Scaled and imputed peak area values were log transformed, and statistical significance determined using a Welch’s two-sample t-test adjusted for multiple comparisons with FDR methods using the R package ‘qvalue’. The hypergeometric P-values were computed using the R package Hypergeo. We also used orthogonal partial least squares discriminant analysis (OPLS-DA) to evaluate the predictive ability of each omics approach. The R package ropls version 1.20.0 was used. This algorithm uses the nonlinear iterative partial least squares algorithm (NIPALS). Since PLS-DA methods are prone to overfitting, we assessed the significance of our classification using permutation tests (permuted 1,000 times).

The raw data is available in Metabolights, with the accession number MTBLS138 (https://www.ebi.ac.uk/metabolights/MTBLS138).

#### S8	Caecum shotgun metagenomics
Shotgun metagenomics was performed by GenomeScan (Leiden, The Netherlands). The NEBNext® Ultra II FS DNA module (cat# NEB #E7810S/L) and the NEBNext® Ultra II Ligation module (cat# NEB #E7595S/L) were used to process the samples. The shotgun metagenomics data was pre-processed using the pre-processing package v0.2.2 (https://anaconda.org/fasnicar/preprocessing). In brief, this package concatenates reads, to remove Illumina adapters, discard low-quality (quality <20 or >2 Ns) or too short reads (< 75bp), remove phiX and rat genome sequences, and finally sorts and splits the reads into R1, R2, and UN sets of reads.

The raw data are available from the National Center for Biotechnology Information (NCBI), with BioProject accession no. PRJNA609596 (https://www.ncbi.nlm. nih.gov/bioproject/PRJNA609596).

Cleaned shotgun metagenomics reads were then processed for taxonomic and pathway profiling. Since there is no gold standard for computational analyses of shotgun metagenomics, we used a combination of approaches. We inferred the taxonomy with the RefSeq database on the metagenomics RAST server, IGGsearch (iggdb_v1.0.0_gut database), MetaPhlAn version 3.0 and Kaiju 1.0.1.

IGG species count data table: File S14
Phylum RefSeq: File S16
Species RefSeq: File S17 
Kaiju species table: File S19 
Metaphlan3 species table: File S21 
KO level 3 function table: File S23 
KO pathway table: File S25

We used ALDEx version 2 (ALDEx2) for differential (relative) abundance analysis of proportional data 56. Statistical analysis for taxa abundance was performed on a dataset corrected for asymmetry (uneven sequencing depths) using the inter-quartile log-ratio method, which identifies features with reproducible variance.

IGG statistical analysis with Adlex2: File S15 
Species RefSeq statistical analysis with Adlex2: File S18 
Kaiju statistical analysis with Adlex2: File S20 
KO level 3 statistical analysis with Adlex2: File S24 
KO pathway statistical analysis with Adlex2: File S22

Metaphlan3 statistical analysis was done using a kruskall-wallis test because the data was not counts but relative abundances values.

A multivariate analysis consisting in a non-metric multidimensional scaling (NMDS) plot of Bray-Curtis distances between samples. Statistical significance of the sample clustering was evaluated with a permutational ANOVA (PERMANOVA) analysis on the Bray-Curtis distances with adonis() from vegan v2.4-2.

#### S9	Metadata metabolomics serum
#### S10 Serum metabolomics raw data
#### S11 Serum metabolomics scaledinputdata
#### S12 Serum metabolomics results
#### S13 Caecum metabolomics results
#### S14 IGG species count data table
#### S15 IGG statistical analysis with Adlex2
#### S16 Phylum RefSeq
#### S17 Species RefSeq
#### S18 Species RefSeq statistical analysis with Adlex2
#### S19 Kaiju species table
#### S20 Kaiju statistical analysis with Adlex2
#### S21 Metaphlan3 species table
#### S22 Metaphlan3 statistical analysis with Adlex2
#### 23	KO level 3 function table
#### S24 KO level 3 statistical analysis with Adlex2
#### S25 KO pathway table
#### S26 KO pathway statistical analysis with Adlex2


