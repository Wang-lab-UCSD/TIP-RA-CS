# TIP-RA-CS
The code needed to reproduce the analysis of methylation array data in James, Holers, Iyer, Prideaux, et al. 2023.


## **Instructions**
Begin the analysis by first creating the conda environments found here: ~/Code/Environments/*.yml. 

The methylation data produced in this publication have been deposited in NCBI’s Gene Expression Omnibus and are accessible via the accession number GSE230446.  Please find the data at the following link: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE230446. Please download the data from GEO to the directory: ~/Data/Raw_Data/

Run Analysis Notebooks
- For each notebook in directory: ~/Code/
  - Launch the notebook
      - Select the appropriate conda environment
        - All notebooks EXCEPT ~/Code/06.DMG_reactome.ipynb use jupyter_TIP-RA-CS.yml
        - For ~/Code/06.DMG_reactome.ipynb use ~/Code/jupyter_reactome.yml
  - Change the filepath of the project_master_dir to the appropriate location on your system
  - Run all cells

Note: Run scripts in numerical order.  The results from preceding notebooks are required for later notebooks to run correctly.  Please ensure that you change the project_master_dir to the appropriate location on your system for each notebook before running.


## **System Requirements**
Script has been tested on system with following specifications:

Platform: x86_64-conda-linux-gnu
R version: R version 4.1.3 (2022-03-10)

Analysis has been performed on a high-performance cluster using the slurm job management system with at least 40GB of memory.

Required R packages are included in the below conda environment files and are loaded in each notebook.
