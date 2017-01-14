## SD_5HTTLPR
Gene-Stress Interaction Analysis Package for "Collaborative meta-analysis finds no evidence of a strong interaction between stress and 5-HTTLPR genotype contributing to the development of depression"
DOI:PENDING PubMed ID:PENDING

(Using both 5-HTT Length Polymorphism and Variant rs25531)

# included files:
README.md						* this file *

gpl-3.0.md						* GPL 3.0 license *

Formatting_data_for_5-HTTLPR_meta-analysis_v8.1.pdf	* Variable coding instructions distributed to all groups *

Script_and_R_instructions_v8.1.pdf			* Instructions for use of package distributed to all groups *

SD_5HTTLPR_v8.1/					* package distributed to all groups *

rmeta_script.4.r					* R script to generate forest plots from intermediate hashes generated by rmeta_caller.pl *

rmeta_caller.pl						* Perl script to read in QCed returned results files and call rmeta_script.4.r to generate all possible meta-analysis forest plots and heterogeneity measures, ordered to run highest priority meta-analyses first.  Filter constant ("$beta_filter") currently set to exclude studies with extreme magnitude linear regression coefficients (magnitude >= ~9.9).  Full run of all meta-analyses took ~40 days *


