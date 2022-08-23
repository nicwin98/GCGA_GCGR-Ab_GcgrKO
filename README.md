# GCGA, GCGR Ab, & GcgrKO
This repository contains the bioinformatic analyses used to analyze RNA sequencing data from a study comparing livers from:
- Female mice treated with a glucagon analogue (GCGA), NNC9204-0043, to a control group treated with PBS.
- Female mice treated with a glucagon receptor antibody (GCGR Ab), REGN1193, to a control group treated with a control antibody (Clt Ab), REGN1945.
- Glucagon receptor knock-out (GcgrKO) mice to wild-type littermates. 

## Data availability 
The raw FASTQ files and the salmon quant.sf files are available in the ArrayExpress database (http://www.ebi.ac.uk/arrayexpress) under accession numbers 
[E-MTAB-12040](https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-12040), [E-MTAB-12048](https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-12048), 
and [E-MTAB-12060](https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-12060) for GCGA, GCGR AB, and GcgrKO, respectively. 

## Session info for release v1.0.0

R version 4.1.0 (2021-05-18)
Platform: x86_64-apple-darwin17.0 (64-bit)
Running under: macOS Big Sur 10.16

Matrix products: default
BLAS:   /Library/Frameworks/R.framework/Versions/4.1/Resources/lib/libRblas.dylib
LAPACK: /Library/Frameworks/R.framework/Versions/4.1/Resources/lib/libRlapack.dylib

locale:
[1] da_DK.UTF-8/da_DK.UTF-8/da_DK.UTF-8/C/da_DK.UTF-8/da_DK.UTF-8

attached base packages:
[1] stats4    stats     graphics  grDevices utils     datasets  methods  
[8] base     

other attached packages:
 [1] GenomicFeatures_1.46.5      ggpubr_0.4.0               
 [3] writexl_1.4.0               xtable_1.8-4               
 [5] repr_1.1.4                  clusterProfiler_4.2.2      
 [7] org.Mm.eg.db_3.14.0         AnnotationDbi_1.56.2       
 [9] EnhancedVolcano_1.12.0      DESeq2_1.34.0              
[11] SummarizedExperiment_1.24.0 Biobase_2.54.0             
[13] GenomicRanges_1.46.1        GenomeInfoDb_1.30.1        
[15] IRanges_2.28.0              S4Vectors_0.32.3           
[17] BiocGenerics_0.40.0         MatrixGenerics_1.6.0       
[19] matrixStats_0.61.0          genefilter_1.76.0          
[21] hexbin_1.28.2               ggrepel_0.9.1              
[23] RColorBrewer_1.1-2          pheatmap_1.0.12            
[25] forcats_0.5.1               stringr_1.4.0              
[27] dplyr_1.0.8                 purrr_0.3.4                
[29] readr_2.1.2                 tidyr_1.2.0                
[31] tibble_3.1.6                ggplot2_3.3.5              
[33] tidyverse_1.3.1             tximeta_1.12.4             

loaded via a namespace (and not attached):
  [1] utf8_1.2.2                    tidyselect_1.1.2             
  [3] RSQLite_2.2.10                grid_4.1.0                   
  [5] BiocParallel_1.28.3           scatterpie_0.1.7             
  [7] munsell_0.5.0                 withr_2.5.0                  
  [9] colorspace_2.0-3              GOSemSim_2.20.0              
 [11] filelock_1.0.2                highr_0.9                    
 [13] ggalt_0.4.0                   knitr_1.37                   
 [15] rstudioapi_0.13               ggsignif_0.6.3               
 [17] DOSE_3.20.1                   Rttf2pt1_1.3.10              
 [19] labeling_0.4.2                tximport_1.22.0              
 [21] GenomeInfoDbData_1.2.7        polyclip_1.10-0              
 [23] farver_2.1.0                  bit64_4.0.5                  
 [25] downloader_0.4                treeio_1.18.1                
 [27] vctrs_0.3.8                   generics_0.1.2               
 [29] xfun_0.30                     BiocFileCache_2.2.1          
 [31] R6_2.5.1                      graphlayouts_0.8.0           
 [33] ggbeeswarm_0.6.0              locfit_1.5-9.5               
 [35] AnnotationFilter_1.18.0       gridGraphics_0.5-1           
 [37] bitops_1.0-7                  cachem_1.0.6                 
 [39] fgsea_1.20.0                  DelayedArray_0.20.0          
 [41] assertthat_0.2.1              vroom_1.5.7                  
 [43] promises_1.2.0.1              BiocIO_1.4.0                 
 [45] scales_1.1.1                  ggraph_2.0.5                 
 [47] enrichplot_1.14.2             beeswarm_0.4.0               
 [49] gtable_0.3.0                  ash_1.0-15                   
 [51] tidygraph_1.2.0               ensembldb_2.18.3             
 [53] rlang_1.0.2                   splines_4.1.0                
 [55] rstatix_0.7.0                 rtracklayer_1.54.0           
 [57] extrafontdb_1.0               lazyeval_0.2.2               
 [59] broom_0.7.12                  abind_1.4-5                  
 [61] BiocManager_1.30.16           yaml_2.3.5                   
 [63] reshape2_1.4.4                modelr_0.1.8                 
 [65] backports_1.4.1               httpuv_1.6.5                 
 [67] qvalue_2.26.0                 extrafont_0.17               
 [69] tools_4.1.0                   ggplotify_0.1.0              
 [71] ellipsis_0.3.2                jquerylib_0.1.4              
 [73] Rcpp_1.0.8                    plyr_1.8.6                   
 [75] base64enc_0.1-3               progress_1.2.2               
 [77] zlibbioc_1.40.0               RCurl_1.98-1.6               
 [79] prettyunits_1.1.1             viridis_0.6.2                
 [81] haven_2.4.3                   fs_1.5.2                     
 [83] magrittr_2.0.2                data.table_1.14.2            
 [85] DO.db_2.9                     reprex_2.0.1                 
 [87] ProtGenerics_1.26.0           patchwork_1.1.1              
 [89] hms_1.1.1                     mime_0.12                    
 [91] evaluate_0.15                 XML_3.99-0.9                 
 [93] readxl_1.3.1                  gridExtra_2.3                
 [95] compiler_4.1.0                biomaRt_2.50.3               
 [97] maps_3.4.0                    shadowtext_0.1.1             
 [99] KernSmooth_2.23-20            crayon_1.5.0                 
[101] htmltools_0.5.2               mgcv_1.8-39                  
[103] ggfun_0.0.5                   later_1.3.0                  
[105] tzdb_0.2.0                    aplot_0.1.2                  
[107] geneplotter_1.72.0            lubridate_1.8.0              
[109] DBI_1.1.2                     tweenr_1.0.2                 
[111] dbplyr_2.1.1                  proj4_1.0-11                 
[113] MASS_7.3-55                   rappdirs_0.3.3               
[115] car_3.0-12                    Matrix_1.4-0                 
[117] cli_3.2.0                     parallel_4.1.0               
[119] igraph_1.2.11                 pkgconfig_2.0.3              
[121] GenomicAlignments_1.30.0      xml2_1.3.3                   
[123] ggtree_3.2.1                  annotate_1.72.0              
[125] vipor_0.4.5                   bslib_0.3.1                  
[127] XVector_0.34.0                rvest_1.0.2                  
[129] yulab.utils_0.0.4             digest_0.6.29                
[131] Biostrings_2.62.0             rmarkdown_2.12               
[133] cellranger_1.1.0              fastmatch_1.1-3              
[135] tidytree_0.3.9                restfulr_0.0.13              
[137] curl_4.3.2                    shiny_1.7.1                  
[139] Rsamtools_2.10.0              rjson_0.2.21                 
[141] nlme_3.1-155                  lifecycle_1.0.1              
[143] jsonlite_1.8.0                carData_3.0-5                
[145] viridisLite_0.4.0             fansi_1.0.2                  
[147] pillar_1.7.0                  lattice_0.20-45              
[149] ggrastr_1.0.1                 KEGGREST_1.34.0              
[151] fastmap_1.1.0                 httr_1.4.2                   
[153] survival_3.3-1                GO.db_3.14.0                 
[155] interactiveDisplayBase_1.32.0 glue_1.6.2                   
[157] png_0.1-7                     BiocVersion_3.14.0           
[159] bit_4.0.4                     ggforce_0.3.3                
[161] stringi_1.7.6                 sass_0.4.0                   
[163] blob_1.2.2                    AnnotationHub_3.2.2          
[165] memoise_2.0.1                 ape_5.6-2
