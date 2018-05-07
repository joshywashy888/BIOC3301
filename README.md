# **BIOC3301: Analysis of 16S rRNA reads**

The following repository contains the four bash scripts used to analyse 16S rRNA reads using Qiime v1.9.1. My scripts were used to compare the differences in taxonomic assignment between Greengenes asd SILVA as the reference database, however individual elements can be taken and run independently :+1:

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. Minicoinda 2 is required to run the Qiime environment, details on installation can be found here: http://qiime.org/install/install.html . The scrips will only work with Qiime 1 so be ensure to only activate the Qiime1 environment.



## The Scripts

There are four scripts, two for the use with Greengenes and two for SILVA. When running the scripts, it is important to ensure you are in the correct working directory and all file paths are correct. **My file paths will not be tha same as yours**

**Greengenes**

There are two scripts for using Greengeens as the reference database

The first (Greengenes_open_OTU) processes and then assigns taxonomies to the OTUs. The script can be run as one as all output files are required.

The secondary script (analysis_Greengenes) is the script for analysing the data output from Greengenes_open_OTU. The analyses can be picked and run independently. DO NOT RUN THE ENTIRE ANALYSIS SCRIPT. The file paths will be off, and an error will be returned. 

**SILVA**

There are two scripts for using SILVA as the reference database. The latest release of SILVA is used.

The first (SILVA_open_OTU) processes and then assigns taxonomies to the OTUs. The script can be run as one as all output files are required. As part of this file, the paramater file (silva-132-params) must be placed in an appropriate directory and referenced correctly under the -p parameter under the *pick_open_refs.py* command. The parameter file must also have the filepaths updated to mathch those on your machine. If this is not done, the script will not run.

The secondary script (analysis_SILVA) is the script for analysing the data output from SILVA_open_OTU. The analyses can be picked and run independently. DO NOT RUN THE ENTIRE ANALYSIS SCRIPT. The file paths will be off, and an error will be returned. 


## Contributors

Thank you to Qiime for the scripts and a thank you to Dr Baron for the Qiime workflows.
