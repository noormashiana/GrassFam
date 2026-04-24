# GrassFam data and scripts

## Description
This repository contains scripts and data from GrassFam: a comprehensive gene family resource for grasses manuscript:

### Abstract
Background: Accurate detection and structural annotation of protein-coding genes remains a limiting step in genome analysis, especially for large and complex genomes such as those of grasses (Poaceae). Inconsistent structural gene annotations with missing exons, truncating models, or misannotated pseudogenes create downstream challenges for functional analysis, comparative genomics, and trait association studies.
Since contemporary grasses are descended from a shared common ancestor ~80 Mya, we expect that the vast majority of their genes evolved from the genes of that ancestral grass by descent with modification. Leveraging this evolutionary history should enable higher quality gene annotation, the transfer of structural and functional information from established model grasses to emerging crops and ecologically important species, and ultimately the identification of bona fide gene novelties. 
Results: Here we present GrassFam 1.0, a collection of 21,795 families of orthologous protein-coding genes derived from sixteen diverse grass genomes, including rice, wheat, barley, sorghum, and maize. Each gene family aims to represent the descendants of a single gene in the most recent common grass ancestor, and includes (1) a set of family members, (2) a profile Hidden Markov Model (HMM) and consensus sequences derived from a subset of “core” family members, (3) a provisional gene family name/function, and (4) the identity of its ancestral grass chromosome. We show how this resource can be used to improve automated genome annotation, transfer functional information from other systems, and analyse conserved synteny and gene loss.
Conclusions: GrassFam provides a platform for integrating structural and functional information across grass genomes, and supports improved structural gene annotation, pseudogene detection, and the identification of novel or lineage-specific gene innovations. Framed as the descendants of single genes from the most recent common grass ancestor, GrassFams are expected to be stable as new grass genomes become available. The full resource, including HMMs and associated metadata, is publicly available to facilitate community use in genome annotation and comparative analysis. 


### File Structure

The files within this repo are organized broadly into three subdirectories: `software`, `source-data`, and `additional-data`: 

- `software/`: This subdirectory contains pipeline scripts used in this work.

- `GrassFam-data/`: This subdirectory contains the GrassFam HMM binaries, cluster information, multiple sequence alignments, consensus sequences, and more. 

- `Supplementary-data/`: This subdirectory contains supplementary data. It also includes data files used in GrassFam not avaiable in other public databases.
