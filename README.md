# ermine-tutorial
Tutorials for the analysis of single-particle tracking data with python and ermine (Estimate Reaction-rates by Markov-based Investigation of Nanoscopy Experiments).   

by Sebastian Malkusch (c) 2021  
Data Science| Klinische Pharmakologie  
Institut für Klinische Pharmakologie  
Goethe - Universität  
Theodor-Stern-Kai 7  
60590 Frankfurt am Main

## Installation
You need to install Ermine prior to usage.   
python -m pip install git+https://github.com/SMLMS/pyErmine

## Data
The data used within this study, together with experimental details, was published previously by Harwardt et al. () . It includes single-particle tracking data on the mobility of the membrane-bound Met receptor.

## Tutorial 01
In this tutorial, we will read in single-particle tracking raw data and calculate the jump widths of the molecules between two consecutive measurements. From the measured jump distances we will calculate the probability density distribution of the jump distances for a molecule within the measurement ensemble via kernel density estimation. The results are saved for use in upcoming tutorials.

## Tutorial 02
In this tutorial, we will use unsupervised machine learning to build a multimodal model that describes the probability density distribution of jump widths from Tutorial 01:

## Tutorial 03
In this tutorial, we will build a hidden Markov model that describes the probability density distribution of jump widths and learns the inter-mode transition probabilities by analyzing the temporal sequence of jump distances

## Tutorial 04
In this tutorial, we will label the temporal sequence of molecular jumps by associating each jump with a mobility mode of our hidden Markov model that was parameterized in tutorial 03.

## Tutorial 05
In this tutorial, we cover static errors due to Endesfelder et al. (https://pubmed.ncbi.nlm.nih.gov/24522395/) and dynamic errors due to Savin and Doyle (https://pubmed.ncbi.nlm.nih.gov/15533928/) that occur when measuring molecular jumps in single-particle tracking experiments.

## Tutorial 06
In this tutorial, we demonstrate how to perform in-silico single-particle tracking experiments using the ermine package.
