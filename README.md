# ECPD-SG-Processed-Data
Processed and anonymized experimental data for ECPD-SG.

This repository provides the processed experimental datasets used in the paper:

**ECPD-SG: An Emotion-Aware Contrastive Prototype Algorithm for Change Point Detection in Dynamic Social Graphs**

## Data Description

The released files are processed and anonymized data used for the change point detection experiments. They are derived from publicly available source datasets, including Pheme, Weibo, and Enron.

The repository contains the following processed datasets:

| File          | Description                              |
| ------------- | ---------------------------------------- |
| `Pheme-1.zip` | Processed dynamic graph data for Pheme-1 |
| `Pheme-2.zip` | Processed dynamic graph data for Pheme-2 |
| `Pheme-3.zip` | Processed dynamic graph data for Pheme-3 |
| `Pheme-4.zip` | Processed dynamic graph data for Pheme-4 |
| `Pheme-5.zip` | Processed dynamic graph data for Pheme-5 |
| `Weibo.zip`   | Processed dynamic graph data for Weibo   |
| `Enron-1.zip` | Processed dynamic graph data for Enron-1 |
| `Enron-2.zip` | Processed dynamic graph data for Enron-2 |

## Released Contents

Each processed dataset may include:

* anonymized dynamic graph snapshots;
* edge lists or adjacency information;
* emotion-aware edge weights;
* processed emotion features;
* snapshot metadata;
* ground-truth change-point labels.

## Privacy Statement

The released data do not contain raw message texts, raw email contents, usernames, email addresses, or original user identifiers. Node identifiers have been anonymized or re-indexed for experimental reproducibility.

## Source Datasets

The original public datasets are available from the following sources:

* Pheme: https://figshare.com/articles/dataset/PHEME_dataset_for_Rumour_Detection_and_Veracity_Classification/6392078
* Weibo: https://www.dropbox.com/s/46r50ctrfa0ur1o/rumdect.zip?dl=0
* Enron: https://www.cs.cmu.edu/~enron/

## Usage

These processed files are provided to support independent verification of the experimental results reported in the paper. Users may download the files and use them to reproduce the change point detection experiments.

## Citation

If you use these processed datasets, please cite the corresponding paper:

ECPD-SG: An Emotion-Aware Contrastive Prototype Algorithm for Change Point Detection in Dynamic Social Graphs.
