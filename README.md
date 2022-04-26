# README

This repository contains the data and code used in Muscatt et al., 2022 ([preprint](https://www.biorxiv.org/content/10.1101/2022.04.22.488307v1)). Post-QC reads are available from the European Nucleotide Archive (ENA) under the Study Accession PRJEB49313. dsDNA vOTU genome sequences were deposited to ENA under Sample Accession SAMEA12363644. ssRNA phage vOTU genome sequences were deposited to ENA under Sample Accession SAMEA11777518. FASTA nucleotide files containing vOTU genomes, FASTA amino acid files containing vOTU genes, vOTU gene annotations, FASTA amino acid files containing ssRNA phage core protein sequences, Newick tree file containing ssRNA phage phylogeny, and vConTACT2 network input and output files are available from [figshare](https://figshare.com/XXX).

------------------------------------------------------------------------

The `Scripts` directory holds the R markdown script `figures_and_tables.Rmd` which can be used to generate all the main and supplementary figures and tables in the paper. Each figure/table is contained within chunks which are intended to be run sequentially i.e., later chunks will require the supplementary tables to have been loaded into the R environment at the beginning. The script is not intended to be knitted, rather each figure/table will be saved to file within the `Figures` or `Tables` directory.

Note: **Figure 1**, **Figure S1**, and **Table S1** were not generated in R.

The `Data` directory holds the raw and processed data files to be loaded into the R environment by `figures_and_tables.Rmd`:

-   `16S_OTUs.csv` contains *16S rRNA OTU data* including read counts.
-   `core_protein_concatenation_tree` is a Newick tree file containing *ssRNA phage phylogeny*.
-   `dsDNA_vOTUs_reads.csv` contains *dsDNA vOTU data* including read counts.
-   `dsDNA_vOTU_distances.tab` contains *pairwise genome distances* between 1,059 dsDNA vOTUs and reference phage genomes.
-   `gene_reads.csv` contains *viral gene read counts*.
-   `ssRNA_phage_vOTUs_reads.csv` contains *ssRNA phage vOTU data* including read counts.
-   `nodes.csv.gz` contains network *node information* from vConTACT2 analysis.
-   `edges.csv.gz` contains network *edge information* from vConTACT2 analysis.
-   `viral_cluster_overview.csv` contains *viral cluster information* from vConTACT2 analysis.
-   `green_genes.csv` contains Greengenes *bacterial taxonomy list*.

The `Figures` directory serves as a location for main and supplementary figures created by the script `figures_and_tables.Rmd` to be exported into.

The `Tables` directory serves as a location for supplementary tables created by the script `figures_and_tables.Rmd` to be exported into.

This README and `figures_and_tables.Rmd` was written by George Muscatt (g.s.muscatt(at)warwick.ac.uk).
