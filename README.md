# SD_5HTTLPR
This GITHUB repository contains one directory and six additional files related to the publication:

**“Collaborative meta-analysis finds no evidence of a strong interaction between stress and 5-HTTLPR genotype contributing to the development of depression”**

DOI:10.1038/mp.2017.44      PubMed ID:28373689

(Coded for analyses using both 5-HTT Length Polymorphism and variant rs25531)
Scripts in this repository are licensed under GPL3.0


## included files:
### Directory: SD_5HTTLPR_v8.1/                  
Package containing the software and documentation bundle for distribution to individual sites participating in the meta-analysis. This directory contains:
> **Formatting_data_for_5-HTTLPR_meta-analysis_v8.1.pdf**    
Variable coding instructions distributed to all groups 

> **Script_and_R_instructions_v8.1.pdf**                     
Instructions for use of package distributed to all groups 

> **SD_5HTTLPR_script_v8.1.r**                               
The master script controlling the analyses of an individual data sets, with introductory section of queries regarding variables contained in the dataset (instruments used, time periods queried, etc...)

> **subscripts_v8.1/**                                       
A subdirectory of helper scripts called by the primary script SD_5HTTLPR_script_v8.1.r 

> **TEST_DATA.csv**                                          
A test dataset that verifies the script is correctly installed on the recipient computer

> **list_of_files_generated_by_TEST.txt**                    
List of files which should be generated by setup run on test dataset

> **list_of_files_generated.txt**                            
Master list of all possible files generated (if all variables present in a dataset)



### Additional files:

**README.md**                                       
this file 

**gpl-3.0.md**                                      
GNU Public License 3.0 

**Regression_parser.v5.pl**                         
Perl script to read in QCed returned results files and return ~1200 .csv input files with keys for specific analyses to be read in by rmeta_script.4.r 

**rmeta_caller.pl**                                 
Perl script to read in processed results files and call rmeta_script.4.r to generate all possible meta-analysis forest plots and heterogeneity measures, ordered to run highest priority meta-analyses first.  Filter constant ("$beta_filter") currently set to exclude studies with extreme magnitude linear regression coefficients (magnitude >= ~9.9).  Full run of all meta-analyses took ~40 days 

**rmeta_script.4.r**                                
R script to generate forest plots from intermediate hashes generated by rmeta_caller.pl with appropriate titles, axis labels, etc... 

**title_forestplot.R**                              
R function modification for forestplot() to allow insert of tailored titles and other formatting changes 

