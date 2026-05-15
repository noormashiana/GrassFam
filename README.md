# GrassFam data and scripts

## Description
This repository contains scripts and data from GrassFam: a comprehensive gene family resource for grasses manuscript:

### Abstract
Background: Accurate detection and structural annotation of protein-coding genes remains a limiting step in genome analysis, especially for large and complex genomes such as those of grasses (Poaceae). Inconsistent structural gene annotations with missing exons, truncating models, or misannotated pseudogenes create downstream challenges for functional analysis, comparative genomics, and trait association studies.

Since contemporary grasses are descended from a shared common ancestor ~80 Mya, we expect that the vast majority of their genes evolved from the genes of that ancestral grass by descent with modification. Leveraging this evolutionary history should enable higher quality gene annotation, the transfer of structural and functional information from established model grasses to emerging crops and ecologically important species, and ultimately the identification of bona fide gene novelties.

Results: Here we present GrassFam 1.0, a collection of 21,795 families of orthologous protein-coding genes derived from sixteen diverse grass genomes, including rice, wheat, barley, sorghum, and maize. Each gene family aims to represent the descendants of a single gene in the most recent common grass ancestor, and includes (1) a set of family members, (2) a profile Hidden Markov Model (HMM) and consensus sequences derived from a subset of “core” family members, (3) a provisional gene family name/function, and (4) the identity of its ancestral grass chromosome. We show how this resource can be used to improve automated genome annotation, transfer functional information from other systems, and analyse conserved synteny and gene loss.

Conclusions: GrassFam provides a platform for integrating structural and functional information across grass genomes, and supports improved structural gene annotation, pseudogene detection, and the identification of novel or lineage-specific gene innovations. Framed as the descendants of single genes from the most recent common grass ancestor, GrassFams are expected to be stable as new grass genomes become available. The full resource, including HMMs and associated metadata, is publicly available to facilitate community use in genome annotation and comparative analysis.

## Description of GrassFam figures and Tables

Table 1: Table summarizing source of the 16 genome datasets
Table 2: GrassFam membership by species.

Supplementary Table S1: Data sources.
Supplementary Table S2: DETAILS. Distribution of genes and species across GrassFam (family level analysis).
Supplementary Table S3: Ancestral grass chromosomes are significant enrichment in Triticodae + Poodae losses (p<0.05, Fischer’s exact test for each AGK vs background, one sided greater missingness, P-value adjusted for false discovery by Benjamini-Hochberg test)
Supplementary Table S4: Summary of GrassFam consensus-to-genome alignments. Number of high-quality alignments found per species between GrassFam consensus sequences and the respective genomes using miniprot. High-quality alignments are defined as those with sequence coverage greater than 90% of the consensus, amino acid identity greater than 50%, and no frameshifts or premature stop codons.
Supplementary Figure S1. Panels showing, across species, the variation in number of GrassFams present per genome (a, core family, b, extended family)
Supplementary Figure S2. Boxplots showing variation in number of truncated/elongated peptide per species.
Supplementary Figure S3. Histogram of the fraction of genes in a family that are similar to RexDB genes.
Supplementary Figure S4. IQTREE3 Maximum likelihood estimated tree using multiple sequence alignment of conflicted Grassfam, GFAM005512, Figure 4c. Labeled with Species, gene ID and Panther Subfamily

Supplementary Data File (in repo): MSINENSIS. proteome and bed file mapping protein-coding sequences to genomic coordinates used in GrassFam.
Supplementary Data File 1 (MASTER_TABLE) (in repo): master csv of GrassFams, including panther and designation as TE, cp/mt, etc.
Supplementary Data File 2 (CONSENSUS) (in repo): master fasta files of grass, BOP, and PACMAD consensus sequences.
Supplementary Data File 3 (in repo): GRASSFAM HMMS.
Supplementary Data File 4 (in repo): CANDIDATES: csv file of candidate loci for “missing” non-TE GrassFams.
Columns: species, ID of “missing” (non-TE) GrassFam, functionally transferred name (Panther), chromosome of alignment, start and end coordinate of alignment.



### File Structure

The files within this repo are organized broadly into three subdirectories: `software`, `source-data`, and `additional-data`: 

- `software/`: This subdirectory contains pipeline scripts used in this work.

- `GrassFam-data/`: This subdirectory contains the GrassFam HMM binaries, cluster information, multiple sequence alignments, and more. This subdirectory also contains Supplementary Data File 2: fasta files of grass, BOP, and PACMAD consensus sequences. As well as, Supplementary Data File 3: GRASSFAM HMMS.

- `Supplementary-data/`: This subdirectory contains large supplementary data, including data files used to create GrassFam not avaiable in other public databases. This subdirectory also contains Supplementary Data File 1: master tsv of GrassFams, including panther and designation as TE, cp/mt, etc. As well as, Supplementary Data File 4: a csv file of candidate loci for “missing” non-TE GrassFams.
