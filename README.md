# StitchSwitch

## 🧶 Crochet Pattern Translation Dataset

Welcome to the repository for the **StitchSwitch Crochet Pattern Translation Dataset**, a structured, open-source collection designed to support machine learning applications in the field of crochet pattern translation. This dataset was developed as part of a study exploring the use of **Large Language Models (LLMs)** to translate standard user-generated crochet patterns into the **CrochetPARADE** syntax.

## Overview

Crochet is a globally cherished craft, offering both creative expression and therapeutic benefits. However, creating and modifying crochet patterns can be challenging, especially for beginners, due to the spatial and structural understanding required.

[**CrochetPARADE**](crochetparade.org) is a visualisation tool designed to simplify this process, but it uses a custom syntax that may be unfamiliar to many crocheters. To bridge this gap, this dataset and accompanying research focus on **automatically translating** standard crochet notation into the CrochetPARADE format using LLMs.

### Pattern Variations

| **Class** | **Name**             | **Description**                                                                                                                                          |
|-----------|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| B         | Base Pattern         | Features from Subset A. Basic elements such as stitch names, repetition of a stitch, increasing and decreasing within a single stitch.                  |
| L         | Labels               | Marking a stitch, or group of stitches, to work into at a later point (e.g., `2sc.A`, where `.A` is defining the label).                                |
| A         | Attachment Points    | Using the `@` symbol to work into a specified stitch or into a defined label (e.g., `sc@A`, working a single crochet into the defined label).           |
| P         | Premature Endings    | Condensing a long string of repeating stitches into a shorter format (e.g., `[2sc, >, dc]*3` is equivalent to `2sc, dc, 2sc, dc, 2sc`).                |

---

## 📂 Dataset Contents

This repository includes:
- `StitchSwitchDataset.csv`: A CSV file containing the original patterns, translated patterns, the shape of pattern output, and the pattern variation. 
---

## Project Summary

This dataset was used to evaluate a range of machine learning strategies:

- **Baseline** inference with vanilla LLMs.
- **Few-shot** prompting using examples representative of all variations.
- **Fine-tuning** on the dataset using various LLMs.

📈 **Best-performing model:**  
Fine-tuned `DeepSeek-R1-Distill-Llama8b` - 74% Accuracy 

## 🧠 Citation

If you use this dataset in your research or project, please cite: SOON HOPEFULLY 

