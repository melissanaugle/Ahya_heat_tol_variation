# Ahya_heat_tol_variation
     
Data and scripts associated with: 
      
Naugle, MS. Denis, H. Mocellin, VJL. Laffy, PW. Popovic, I. Bay, LK. Howells, EJ., (2024) 
Environmental, host, and symbiont drivers of heat tolerance in a species complex of reef-building corals. 
biorxiv https://doi.org/10.1101/2024.01.31.575130
      
The repository is organized in multiple parts:    
    
## 1. Raw data:
 Includes raw environmental, heat tolerance, and ITS2 data.  
 
 Files include:  
    - Coral colony metadata...xlxs: Metadata associated with coral colonies sampled for RRAP ECT-1  
    - TideData.csv: data on tides at reef sites on sampling dates  
    - TotalChlorophyll.csv: data on lab-assayed chlorophyll  
    - SiteCharacteristics.csv: metadata associated with each reef site   
    - SeaSim_holdtemps.csv: temperatures of tanks in acute heat stress experiment   
    - ECT1_sites_environmental_data.csv: Environmental data associated with each colony  
    - ECT1_sites_environmental_data_depthsadjusted...csv: Environmental data associated with each colony, adjusted to colony depth    
    - full_iPAM_data...: raw iPAM data on the 569 genotypes measured in this project   
    - hyperspecdata...: raw NDVI values from hyperspectral data for 555 genotypes in this project     
    - Raw data associated with ITS2 analysis of Symbiodiniacae (in a directory)         

Raw WGS reads will be found on the NCBI Sequence Read Archive (SRA) database: PRJNA982441     
Raw ITS2 sequence data will be made available on the NCBI Sequence Read Archive (SRA) database soon.     
     
## 2. Clean data:
Includes cleaned heat tolerance trait data, environmental data associated with each colony, ITS2 data, and host cluster assignments. 

Files include:  
    - 2023_05_03_naturalbleachingnorthdirection_clust.csv: cluster identities of colonies sampled during a natural bleaching event and their color scores    
    - 2023_10_17_clust_data_edited.csv: cluster identities of colonies ran in acute heat stress     
    - Environmental_data_PCs...csv: environmental data with PC values to group similar categories of metrics     
    - EnvMetric_categories.csv: categories of environmental metrics      
    - ITS2_types_OTUs...csv: its2 type profiles and sequence variants associated with each colony      
    - pheno_metadata_clean...csv: phenotype and metadata for each colony     
    - iPAM (fv/fm): site- and colony-level ED50s and retained fvfm data     
    - NDVI: site- and colony-level ED50s and retained fvfm data      

## 3. Data processing:
Includes R scripts for processing raw data and data exploration.     

Scripts include:     
    - 1_Correct_colony_depth.Rmd: adjust colony depths using tide data     
    - 2_standardizeenvvra_depth.Rmd: standardize environmental variables to tide-adjusted depths    
    - 3_iPAM_generate_ed50_retention.Rmd: generate ED50s and retained fvfm phenotypic metrics      
    - 4_NDVI_generate_ed50_retention.Rmd: generate ED50s and retained NDVI phenotypic metrics      
    - 5_consolidate_phenos.Rmd: consolidate phenotypes and metadata, polish datasheets, quality control of data    
    - 6_Symbiont_dataprep.Rmd: prepare symbiont data, quality control, and early analyses     

## 4. Data analysis:
Includes R scripts for generating figures and results presented in the publication.   

Scripts include:     
    - Data_overview.Rmd: quality control steps and overview of data (**Figs 1, 2, S1, S2, S3; Table 1**)     
    - Boosted_Regression_trees.Rmd: to run boosted regression trees (**Fig 6**)      
    - Cryptic_spp_analysis.Rmd: to explore genomic cluster variation spatially and with phenotype (**Figs 4 and S4**)      
    - Environmental_analysis.Rmd: to explore environmental metric relationships to phenotype (**Fig S8**)      
    - ITS2_analysis.Rmd: to explore symbiodiniacae relationships to phenotype (**Figs 5, S5, S6, S7; Tables S4 and S5**)     
    - LMERs.Rmd: to run linear mixed effects models (**Fig S9; Table S6**)     

## 5. Outputs:
Includes figures in the publication as well as additional figures     
     
### For questions or additional data/scripts, contact Melissa Naugle: melissasnaugle@gmail.com
    
