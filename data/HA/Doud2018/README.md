# Mutational Antigenic Profiling of A/WSN/1933 (H1N1) influenza HA monoclonal antibodies

The paper link is [Doud, Lee, and Bloom (2016)](https://research.fhcrc.org/content/dam/stripe/bloom/labfiles/publications/Doud2018.pdf).

[1rvx_1trimer.pdb](1rvx_1trimer.pdb) is the crystal structure of the closely related A/PR/8/1934 (H1N1) HA with only one of the two trimers in the asymmetric unit retained.

The following files are supplemental data files from [Doud, Lee, and Bloom (2016)](https://www.nature.com/articles/s41467-018-03665-3#Sec20):

  - antibody_*_median.csv (example: [antibody_C179_median.csv](Supplemental_File_2_HApreferences.txt)): excess fraction surviving for each mutation.
  - antibody_*_median_avgsite.csv (example: [antibody_C179_median_avgsite.csv](antibody_C179_median_avgsite.csv)): excess fraction surviving summarized at each site.
  - [numbering_map.csv](numbering_map.csv)): mapping from sequential numbering of WSN HA to the H3 numbering scheme used in the PDB file.

The Jupyter notebook [build_data.ipynb](build_data.ipynb) reads in the above supplemental data files and generates the data file for `dms-view`, [Doud2018.csv](Doud2018.csv).
