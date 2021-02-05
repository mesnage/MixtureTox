## Code and data for the multi-omics phenotyping of the gut-liver axis after exposure to a low-dose pesticide mixture.

### Abstract
Health effects of pesticides are not always accurately detected using the current battery of regulatory toxicity tests. We compared standard histopathology and serum biochemistry measures and multi-omics analyses in a subchronic toxicity test of a mixture of six pesticides frequently detected in foodstuffs (azoxystrobin, boscalid, chlorpyrifos, glyphosate, imidacloprid and thiabendazole) in Sprague-Dawley rats. Analysis of water and feed consumption, body weight, histopathology and serum biochemistry showed little effects. Contrastingly, serum and caecum metabolomics revealed that nicotinamide and tryptophan metabolism were affected, which suggested the activation of an oxidative stress response. This was not reflected by gut microbial community composition changes evaluated by shotgun metagenomics. Transcriptomics of the liver showed that 257 genes had their expression changed. Gene functions affected included the regulation of response to steroid hormones and the activation of stress response pathways. Genome-wide DNA methylation analysis of the same liver samples showed that 4,255 CpG sites were differentially methylated. Overall, we demonstrated that in-depth molecular profiling in laboratory animals exposed to low concentrations of pesticides allows the detection of metabolic perturbations which could improve the health risk predictability of chemical assessment.

### Publication
Mesnage R, Teixeira M, Mandrioli D, Falcioni L, Ducarmon QR, Zwittink RD, Amiel C, Panoff J, Bourne B, Savage E, Mein CA, Belpoggi F, Antoniou MN (2020). Multi-omics phenotyping of the gut-liver axis allows health risk predictability from in vivo subchronic toxicity test of a low-dose pesticide mixture. BioRxiv. doi: https://doi.org/10.1101/2020.08.25.266528

A R Markdown document has been made available to ensure the full reproducibility of these results: https://mesnage.github.io/mixtox.html 

#### Water consumption	

The daily water consumption per cage was measured before the start of the experiment, and weekly for all the duration of the treatment (13 weeks). Before the final sacrifice and after about 16 hours in metabolic cage, water consumption, was registered for each animal. The means of individual consumptions and related standard deviation were calculated for every group and for sex.

- Raw data for water consumption is available as [File S2](https://github.com/mesnage/MixtureTox/blob/main/mixture_S02.csv) 

#### Food consumption

The daily food consumption per cage was measured before the start of the experiment, and weekly for all the duration of the treatment (13 weeks). Before the final sacrifice and after about 16 hours in metabolic cage, water consumption, was registered for each animal. The means of individual consumptions and related standard deviation were calculated for every group and for sex.

- Raw data for food consumption is available as File S3.

#### Body weights

Body weight of experimental animals was measured before the start of the treatment, and then weekly for 13 weeks. All the experimental animals were weighted just before the sacrifice. Average body weights and related standard deviations were calculated for each experimental group.

- Raw data for food consumption is available as File S4

#### Serum biochemistry
Serum biochemistry was performed under contract by IDEXX BioAnalytics (Stuttgart, Germany), an ISO 17025 accredited laboratory. Briefly, sodium and potassium levels were measured by indirect potentiometry. Albumin was measured by a photometric bromocresol green test. ALP was measured by IFCC with AMP-buffer method, glucose by Enzymatic UV-Test (hexokinase method), cholesterol by Enzymatic color test (CHOD-PAP), blood urea nitrogen by enzymatic UV-Test, gamma-glutamyl-transferase by Kinetic color test International Federation of Clinical Chemistry (IFCC), aspartate and alanine aminotransferase by kinetic UV-test (IFCC+ pyridoxal-5-phosphate), creatinine by kinetic color test (Jaffe’s method), lactate dehydrogenase by IFCC method, and triglycerides using an enzymatic color test (GPO-PAP) on a Beckman Coulter AU 480.

- Raw data for food consumption is available as File S5

#### Serum metabolomics

Serum Metabolomics analysis was conducted under contract with Metabolon Inc. (Durham, NC, USA) on four independent instrument platforms as previously described: two different separate reverse phase ultrahigh performance liquid chromatography-tandem mass spectroscopy analysis (RP/UPLC-MS/MS) with positive ion mode electrospray ionization (ESI), a RP/UPLC-MS/MS with negative ion mode ESI, as well as by hydrophilic-interaction chromatography (HILIC)/UPLC-MS/MS with negative ion mode ESI.

- The raw data for the peak intensity is available as File S10. 
- The metadata describing annotation, mass and RI is available as File S9.
- The scaled and imputed data is available as File S11.
- The results are available as File S12

The raw data is available in Metabolights, with the accession number MTBLS138 (https://www.ebi.ac.uk/metabolights/MTBLS138).

#### Caecum metabolomics

Caecum Metabolomics analysis was conducted under contract with Metabolon Inc. (Durham, NC, USA) on four independent instrument platforms as previously described: two different separate reverse phase ultrahigh performance liquid chromatography-tandem mass spectroscopy analysis (RP/UPLC-MS/MS) with positive ion mode electrospray ionization (ESI), a RP/UPLC-MS/MS with negative ion mode ESI, as well as by hydrophilic-interaction chromatography (HILIC)/UPLC-MS/MS with negative ion mode ESI.

- The raw data for the peak intensity is available as File S7.
- The metadata describing annotation, mass and RI is available as File S6.
- The scaled and imputed data is available as File S8.
- Results are available as file S13

The raw data is available in Metabolights, with the accession number MTBLS138 (https://www.ebi.ac.uk/metabolights/MTBLS138).

#### S8	Caecum shotgun metagenomics
Shotgun metagenomics was performed by GenomeScan (Leiden, The Netherlands). The NEBNext® Ultra II FS DNA module (cat# NEB #E7810S/L) and the NEBNext® Ultra II Ligation module (cat# NEB #E7595S/L) were used to process the samples. The shotgun metagenomics data was pre-processed using the pre-processing package v0.2.2 (https://anaconda.org/fasnicar/preprocessing). In brief, this package concatenates reads, to remove Illumina adapters, discard low-quality (quality <20 or >2 Ns) or too short reads (< 75bp), remove phiX and rat genome sequences, and finally sorts and splits the reads into R1, R2, and UN sets of reads.

The raw data are available from the National Center for Biotechnology Information (NCBI), with BioProject accession no. PRJNA609596 (https://www.ncbi.nlm. nih.gov/bioproject/PRJNA609596).

Cleaned shotgun metagenomics reads were then processed for taxonomic and pathway profiling. Since there is no gold standard for computational analyses of shotgun metagenomics, we used a combination of approaches. We inferred the taxonomy with the RefSeq database on the metagenomics RAST server, IGGsearch (iggdb_v1.0.0_gut database), MetaPhlAn version 3.0 and Kaiju 1.0.1.

Metagenome data.
- IGG species count data table: File S14
- Phylum RefSeq: File S16
- Species RefSeq: File S17 
- Kaiju species table: File S19 
- Metaphlan3 species table: File S21 
- KO level 3 function table: File S23 
- KO pathway table: File S25

Results.
- IGG statistical analysis with Adlex2: File S15 
- Species RefSeq statistical analysis with Adlex2: File S18 
- Kaiju statistical analysis with Adlex2: File S20 
- KO level 3 statistical analysis with Adlex2: File S24 
- KO pathway statistical analysis with Adlex2: File S22


#### Liver transcriptomics
RNA-seq data was analysed with Salmon. This tool was used to quantify transcript abundance by mapping the reads against a reference transcriptome (Ensembl Release Rattus Norvegicus 6.0 cDNA fasta). Mapping rate was 82.0 ± 4.4% on a rat transcriptome index containing 31,196 targets. The Salmon output was then imported in R as described in this Markdown using the Bioconductor package tximport.

The files generated using Salmon are available.

- Transcriptome abundance: File S27
- Transcriptome counts: File S28
- Transcriptome length: File S29 
- Transcriptome gtf_file: File S30 
- Transcriptome sampleinfo: File S31
- DESeq_normalized_counts: File S32 
- Transcriptome statistical analysis: FileS33
- Transcriptome pathway enrichment KEGG: File S34 
- Transcriptome GO enrichment: File S35

#### Liver methylation
DNA methylation calls from RRBS data were extracted with Bismark. The output from Bismark was then imported in R and analysed with Methylkit. DNA methylation calls were annotated using RefSeq gene predictions for rats (rn6 release) with the package genomation. Other annotations were retrieved using the genome wide annotation for rat tool org.Rn.eg.dbR package version 3.8.2. Statistical analysis was performed with logistic regression models fitted per CpG using Methylkit functions. P-values were adjusted to Q-values using SLIM method.

The raw data from the RRBS analysis is available at GEO accession number GSE157551.

The output from Bismark is downloaded from GitHUb. Note that 5 files were over the 25Mb size limit for GitHub. In order to allow their use, they have been broken down for their storage on GitHub. A bashscript is included in this Markdown to concatenate back the outputs of the 5 files.


