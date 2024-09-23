# HybPiperAnalysis

## Overview
Manually performing all of the steps necessary to complete a HybPiper analysis was faily combersome and time consuming.  The perl script consolidates all of the steps into a single application.  The script will run each of the following step to collect the necessary data, if needed, and run each of the HybPiper tasks:
  1) Create a standardized subdirectory structure for the DNA species analysis
  2) Download, if necessary, a DNA FASTQ Read file
  3) If necessary, "trim" the FASTQ file using Trimomatic
  4) UnZip the output from the Trimomatic processing
  5) Create a "NameList", which will be used in subsequent steps, based on the FASTQ read file name(s)
  6) Run HybPiper Assemble
  7) Run HybPiper Stats
  8) Run HybPiper Retrieve_Sequences
  9) Run HybPiper Paralog_Retriever
  10) Cleanup/delete HybPiper results files that do not contain any data


## Dependencies
### Computer
Apple M3 MacBook Pro, 18GB memory, 1TB storage  
(NOTE: If you have an Intel based Apple computer, use it!  There is no M series specific software for some of the products listed below.  However, on M series computers Apple will automatically AND slowly run the Intel based softare in an emulation mode.)

### Creating A Basic Development Environment
  1) Miniconda (v24.7.1 Apple M1) : https://docs.anaconda.com/miniconda/#miniconda-latest-installer-links
  2) Microsoft Visual Code : https://code.visualstudio.com/Download or whatever development environment you prefer

### Software Needed For This Project
  1) SRA Toolkit (v3.1.0 - MacOS x86-64bit) : https://github.com/ncbi/sra-tools/wiki/01.-Downloading-SRA-Toolkit  
  2) HybPiper (v2.3.0) : https://github.com/mossmatters/HybPiper/releases  
  3) U.PhyloMaker (v0.1.0) : https://github.com/jinyizju/U.PhyloMaker/blob/master/U.PhyloMaker_0.1.0.tar.gz  
  4) Trimmomatic (v0.39) : http://www.usadellab.org/cms/?page=trimmomatic
  5) JAVA - latest version (Trimmomatic is a java application)

