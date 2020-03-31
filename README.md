# Influenza virus deep mutational scanning data sets visualized by `dms-view`

## Data sets

### Hemagglutinin (HA)

- Mutational tolerance of the H1 HA from A/WSN/1933 as measured by [Doud and Bloom (2016)](https://www.ncbi.nlm.nih.gov/pubmed/27271655).
  [See here](https://dms-view.github.io/?markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Finfluenza%2Fmaster%2Fdata%2FHA%2FDoud2016%2FDoud2016.md&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Finfluenza%2Fmaster%2Fdata%2FHA%2FDoud2016%2FDoud2016.csv&condition=rescaled_measurements&site_metric=site_entropy_bits&mutation_metric=mut_preference&selected_sites=Y+98%2CG+134%2CV+135%2CT+136%2CV+137%2CS+138%2CS+145%2CW+153%2CT+155%2CH+183%2CP+185%2CS+186%2CE+190%2CL+194%2CD+225%2CQ+226%2CG+228&pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Finfluenza%2Fmaster%2Fdata%2FHA%2FDoud2016%2F1rvx_1trimer.pdb) for an interactive `dms-view` visualization that shows the mutational tolerance focusing on sites within 5 angstroms of the receptor.
  The raw data are [here](data/HA/Doud2016).
- Mutational Antigenic Profiling of A/WSN/1933 H1 HA from monoclonal antibodies measured by [Doud, Lee, and Bloom, 2018](https://research.fhcrc.org/content/dam/stripe/bloom/labfiles/publications/Doud2018.pdf).
[See here](https://dms-view.github.io/?markdown-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Finfluenza%2Fmaster%2Fdata%2FHA%2FDoud2018%2FDoud2018.md&pdb-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Finfluenza%2Fmaster%2Fdata%2FHA%2FDoud2018%2F1rvx_1trimer.pdb&data-url=https%3A%2F%2Fraw.githubusercontent.com%2Fdms-view%2Finfluenza%2Fmaster%2Fdata%2FHA%2FDoud2018%2FDoud2018.csv&condition=S139&site_metric=site_avg+excess+frac+survive&mutation_metric=mut_excess+frac+survive&selected_sites=156%2C158%2C193) for an interactive dms-view visualization focusing on the antibody S139.
The raw data are [here](data/HA/Doud2018).


## Adding data sets

1. Make a new branch or a fork of this repository.

2. Navigate to the [./data/](data) directory and create a subdirectory for the appropriate protein and study.
   Data are organized first by protein and then by study, with studies named by the first author and year, such as [./data/HA/Doud2016/](data/HA/Doud2016).

3. Within that subdirectory, add the three input files that are needed to visualize the data.
   As described in the [`dms-view` docs](https://dms-view.github.io/docs/), these are a CSV file of the data, a protein structure PDB file, and a Markdown metadata file.
   In general, you should name these with the CSV data file named according to the study name (e.g., [./data/HA/Doud2016/Doud2016.csv](data/HA/Doud2016/Doud2016.csv)), the PDB file simply being the PDB (e.g., [./data/HA/Doud2016/1rvx_1trimer.pdb](./data/HA/Doud2016/1rvx_1trimer.pdb)), and the Markdown metadata file also named according to the study name (e.g. [./data/HA/Doud2016/Doud2016.md](data/HA/Doud2016/Doud2016.md)).
   In addition, you should add a README within the subdirectory explaining the origin of the files (e.g., [./data/HA/Doud2016/README.md](data/HA/Doud2016/README.md)).
   In some cases (such as if the same data is mapped to multiple protein structures) you may need to extend or modify this naming scheme.
   If you need to process other rawer forms of the data (e.g., from paper supplements) into the final data file for `dms-view`, then include those rawer data and the processing scripts if possible, explaining in the subdirectory repo.

4. Make a pull request for your branch or fork to add the data.

5. In [this top-level README file](README.md) add a **short** description of the study and a link to an appropriate [dms-view](https://dms-view.github.io) view of the dataset.

6. Make a pull request for your branch or fork to add the link.
