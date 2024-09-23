# HybPiperAnalysis

## Overview
Manually performing all of the steps necessary to complete a HybPiper analysis was faily combersome and time consuming.  The perl script consolidates all of the steps into a single application.  The script will run each of the following step to collect the necessary data, if needed, and run each of the HybPiper tasks:
  1) Create a standardized subdirectory structure for the DNA species analysis
  2) Download, if necessary, a DNA FASTQ Read file
  3) If necessary, "trim" the FASTQ file using Trimomatic
  4) UnZip the output from the Trimomatic processing
  5) Create a "NameList", which will be used in subsequent steps, based on the FASTQ read file name(s)
  6) Run HybPiper Assemblel
  7) Run HybPiper Stats
  8) Run HybPiper Retrieve_Sequences
  9) Run HybPiper Paralog_Retriever
  10) Cleanup/delete HybPiper results files that do not contain any data


## Dependencies
### Creating A Basic Development Environment
  Anaconda (Anaconda3-2024.02-1 MacOSX-x86_64) : https://www.anaconda.com/download  
  Python (pycharm-community-2023.2.5) -- https://www.jetbrains.com/edu-products/download/download-thanks-pce.html  
  R (4.3.3 -- Angel Food Cake (for Mac Intel) package: R-4.3.3-x86_64.pkg) -- A) https://www.r-project.org/ B) Select "download R"  
### Software Needed For This Project
  SRA Toolkit (v3.1.0 - MacOS x86-64bit) : https://github.com/ncbi/sra-tools/wiki/01.-Downloading-SRA-Toolkit  
  HybPiper (v2.1.6) : https://github.com/mossmatters/HybPiper/releases  
  U.PhyloMaker (v0.1.0) : https://github.com/jinyizju/U.PhyloMaker/blob/master/U.PhyloMaker_0.1.0.tar.gz  
  Trimmomatic (v-.039) : http://www.usadellab.org/cms/?page=trimmomatic  

