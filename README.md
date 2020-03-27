# Influenza virus data sets visualized by `dms-view`

## Data sets

### Hemagglutinin

## Adding data sets

1. Make a new branch or a fork of this repository.

2. Navigate to the [./data/](data) directory and create a subdirectory for the appropriate protein and study.
   Data are organized first by protein and then by study, with studies named by the first author and year, such as [./data/HA/Doud2016/](data/HA/Doud2016).

3. Within that subdirectory, add the three input files that are needed to visualize the data.
   As described in the [`dms-view` docs](https://dms-view.github.io/docs/), these are a CSV file of the data, a protein structure PDB file, and a Markdown metadata file.
   In general, you should name these with the CSV data file named according to the study name (e.g., [./data/HA/Doud2016/Doud2016.csv](data/HA/Doud2016/Doud2016.csv)), the PDB file simply being the PDB (e.g., [./data/HA/Doud2016/1RVX.pdb](./data/HA/Doud2016/1RVX.pdb)), and the Markdown metadata file also named according to the study name (e.g. [./data/HA/Doud2016/Doud2016.md](data/HA/Doud2016/Doud2016.md)).
   In addition, you should add a README within the subdirectory explaining the origin of the files (e.g., [./data/HA/Doud2016/README.md](data/HA/Doud2016/README.md)).
   In some cases (such as if the same data is mapped to mutiple protein structures) you may need to extend or modify this naming scheme.

4. In [this top-level README file](README.md) add a **short** description of the study and a link to an appropriate [dms-view](https://dms-view.github.io) view of the dataset.

5. Make a pull request for your branch or fork.
