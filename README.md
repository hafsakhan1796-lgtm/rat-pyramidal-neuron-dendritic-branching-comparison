# Rat Pyramidal Neuron Dendritic Branching Comparison

Python analysis comparing dendritic branching patterns in rat hippocampal vs. 
neocortical pyramidal neurons, using real neuron reconstructions from 
[NeuroMorpho.org](https://neuromorpho.org).

*Paper title: "Similar Branching, Different Reach: Dendritic Cable Length 
Distinguishes Hippocampal and Neocortical Pyramidal Neurons in Rats"*

## Summary

This project compares dendritic branching complexity between rat hippocampal 
and neocortical pyramidal neurons using real, publicly available neuron 
reconstruction data. Twenty neurons per region were analyzed in Python, 
measuring branch count, terminal branch (leaf) count, total dendritic cable 
length, and a derived branches-per-length ratio. Neocortical neurons showed 
significantly greater total cable length than hippocampal neurons (Welch's 
t-test, p < 0.001), while branch count did not differ significantly between 
groups (p = 0.83). These results suggest that hippocampal and neocortical 
pyramidal neurons achieve similar branching complexity through different 
structural strategies — compact, densely-packed branching in the hippocampus 
versus longer-reaching branches in the neocortex.

## Contents

- **Paper (PDF)** — full written report: introduction, methods, results, discussion, and references
- **`rat_neuron_dendritic_branching_analysis.ipynb`** — Python analysis notebook (data retrieval, metrics extraction, statistics, visualization)
- **`boxplot.png`** — cable length comparison figure
- **`hippo_morphology.png`, `neocortex_morphology.png`** — representative neuron morphology renderings
- **`table1_branching_metrics.png`** — summary statistics table

## Tools used

Python, pandas, navis, scipy, matplotlib

## Data source

[NeuroMorpho.org](https://neuromorpho.org), accessed via the `navis` Python library.
