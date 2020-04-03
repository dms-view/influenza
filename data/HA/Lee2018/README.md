# Deep mutational scanning of A/Perth/2008 (H3N2) influenza HA

The paper link is [Lee *et al.*, (2018)](https://www.pnas.org/content/115/35/E8276).

[4O5N_trimer.pdb](4O5N_trimer.pdb) is the crystal structure of the closely related A/Victoria/361/2011 H3N2 strain.

The following files are data files from [Lee *et al.*, (2018)](https://www.pnas.org/content/115/35/E8276).
See the [paper Github repo](https://github.com/jbloomlab/Perth2009-DMS-Manuscript) to instructions on finding or generating the files.

- [summary_avgprefs_rescaled_entropies.csv](summary_avgprefs_rescaled_entropies.csv): rescaled Perth09 prefs and calculated entropy/neffective
- [H3_alignment_frequences.csv](H3_alignment_frequences.csv): natural amino-acid frequencies. Note: these frequencies were curated in 2018 and has not been updated.
- [Perth09_HA_reference.fa](Perth09_HA_reference.fa): Perth09 reference sequence used in the experiment.
- [Perth_to_WSN_prefs_dist.csv](Perth_to_WSN_prefs_dist.csv): RMSD between Perth09 and WSN
- [H3renumbering_scheme.csv](H3renumbering_scheme.csv): numbering map between sequential Perth09 and H3 numbering.
- [Perth2009_compareprefs_renumber.csv](Perth2009_compareprefs_renumber.csv): numbering map from sequential Perth09 to sequential shared sites between Perth09 and WSN.



The Jupyter notebook [build_data.ipynb](build_data.ipynb) reads in the above supplemental data files and generates the data file for `dms-view`, [Lee2018.csv](Lee2018.csv).
