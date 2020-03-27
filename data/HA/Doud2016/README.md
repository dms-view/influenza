# Deep mutational scanning of A/WSN/1933 (H1N1) influenza HA

The paper link is [Doud and Bloom (2016)](https://www.ncbi.nlm.nih.gov/pubmed/27271655).

[1rvx_1trimer.pdb](1rvx_1trimer.pdb) is the crystal structure of the closely related A/PR/8/1934 (H1N1) HA with only one of the two trimers in the asymmetric unit retained.

The following files are supplemental data files from [Doud and Bloom (2016)](https://www.ncbi.nlm.nih.gov/pubmed/27271655):

  - [Supplemental_File_2_HApreferences.txt](Supplemental_File_2_HApreferences.txt): amino-acid preferences.
  - [Supplemental_File_3_HApreferences_rescaled.txt](Supplemental_File_3_HApreferences_rescaled.txt): re-scaled amino-acid preferences.
  - [Supplemental_File_6_WSN_to_H3_numbering_conversion.txt](Supplemental_File_6_WSN_to_H3_numbering_conversion.txt): mapping from sequential numbering of WSN HA to the H3 numbering scheme used in the PDB file.

The Jupyter notebook [build_data.ipynb](build_data.ipynb) reads in the above supplemental data files and generates the data file for `dms-view`, [Doud2016.csv](Doud2016.csv).
