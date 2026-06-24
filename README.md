# ECPD-SG-Processed-Data

Processed experimental data for ECPD-SG.

This repository provides the processed datasets used in the paper:

**ECPD-SG: An Emotion-Aware Contrastive Prototype Algorithm for Change Point Detection in Dynamic Social Graphs**

## Data Description

The released files are the final processed data objects used for the change point detection experiments. They are derived from publicly available source datasets, including Pheme, Weibo, and Enron.

The repository contains eight compressed files. Each `.rar` archive contains one processed PyTorch object (`.pt`) used as the model input.

| File          | Description                              |
| ------------- | ---------------------------------------- |
| `Pheme-1.rar` | Processed dynamic graph data for Pheme-1 |
| `Pheme-2.rar` | Processed dynamic graph data for Pheme-2 |
| `Pheme-3.rar` | Processed dynamic graph data for Pheme-3 |
| `Pheme-4.rar` | Processed dynamic graph data for Pheme-4 |
| `Pheme-5.rar` | Processed dynamic graph data for Pheme-5 |
| `Pheme-6.rar` | Processed dynamic graph data for Pheme-6 |
| `Weibo.rar`   | Processed dynamic graph data for Weibo   |
| `Enron.rar`   | Processed dynamic graph data for Enron   |

## Released Contents

Each `.rar` file contains a final processed PyTorch data object (`.pt`). After loading with `torch.load(...)`, the object is a dictionary with the following main fields:

* `dynamic_graph`: the processed dynamic graph sequence;
* `comments_with_vectors_plus_emoji`: processed text-derived representations and emotion-related attributes;
* `edge_indices_enhanced`: enhanced edge indices for dynamic graph snapshots;
* `edge_weights_enhanced`: emotion-aware edge weights used by ECPD-SG.

These files are the final processed inputs used by the proposed model. They already contain the processed dynamic network structure, text-derived features, emotion-related attributes, enhanced edge indices, and emotion-aware edge weights.

## Privacy Statement

The released files are processed experimental data for reproducibility. Node identifiers have been anonymized or re-indexed. The released data do not contain usernames, email addresses, or original user identifiers. Textual information is provided in processed feature form for reproducing the change point detection experiments.

## Source Datasets

The original public datasets are available from the following sources:

* Pheme: https://figshare.com/articles/dataset/PHEME_dataset_for_Rumour_Detection_and_Veracity_Classification/6392078
* Weibo: https://www.dropbox.com/s/46r50ctrfa0ur1o/rumdect.zip?dl=0
* Enron: https://www.cs.cmu.edu/~enron/

## Usage

The processed files are provided to support independent verification of the experimental results reported in the paper. Users may download and extract the `.rar` files, then load the contained `.pt` files using PyTorch:

```python
import torch

data = torch.load("example_dataset.pt", map_location="cpu")

dynamic_graph = data["dynamic_graph"]
comments_with_vectors_plus_emoji = data["comments_with_vectors_plus_emoji"]
edge_indices_enhanced = data["edge_indices_enhanced"]
edge_weights_enhanced = data["edge_weights_enhanced"]
```

## Citation

If you use these processed datasets, please cite the corresponding paper:

ECPD-SG: An Emotion-Aware Contrastive Prototype Algorithm for Change Point Detection in Dynamic Social Graphs.
