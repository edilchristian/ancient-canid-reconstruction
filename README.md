# Ancient Canid Reconstruction

This project simulates an ancient DNA analysis pipeline from raw genome sequences to evolutionary and functional insights, modeled after workflows used in paleogenomics research (e.g., studies on the extinct dire wolf).

## Project Overview

The goal was to reconstruct a simplified version of an end-to-end bioinformatics pipeline that includes:

- Simulating ancient DNA fragments from reference genomes
- Aligning damaged fragments to modern genomes
- Constructing phylogenetic trees
- Predicting gene function based on sequence similarity

This was done entirely using classical computational biology techniques.

## Project Structure


- `1_data_preparation.ipynb` :  Load and inspect modern Dog and Wolf reference genomes |
- `2_simulate_ancient_dna.ipynb` : Generate synthetic ancient DNA fragments with damage and variability |
- `3_alignment.ipynb` : Perform pairwise local alignments of fragments to modern genome |
- `4_phylogeny.ipynb` : Construct phylogenetic tree from fragment similarity |
- `5_function_prediction.ipynb` : Predict functional similarity by comparing fragments to known genes |

## Data Sources

- Dog genome: NCBI RefSeq GCF_000002285.5
- Gray Wolf genome: NCBI GenBank GCA_905319855.2
- Simulated gene references: `data/known_dog_genes.fasta` (3 mitochondrial genes)

## Tools and Libraries

- Python 3.9
- Biopython
- Matplotlib
- SciPy
- PairwiseAligner (Biopython)
- Hierarchical clustering from SciPy

## Results

- Successfully simulated 1000 ancient Dog and Wolf fragments
- Aligned and scored similarity of fragments to their species' reference genomes
- Constructed trees using distance matrices based on alignment scores
- Performed function prediction by aligning fragments to known mitochondrial genes

## Author

Edil Christian

This project was inspired by recent coverage of the dire wolf's de-extinction research, featured in The New Yorker and TIME Magazine. That story raised questions for me about how scientists reconstruct evolutionary relationships and genetic functions from ancient, degraded DNA.

I built this project as a way to explore those questions using publicly available genome data, simulated DNA damage, and classical bioinformatics tools. It is intended as both a learning tool and a portfolio project, demonstrating end-to-end analysis from raw sequence to phylogenetic reconstruction and functional inference.
