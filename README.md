# Bosphorus Patent Technology Taxonomy (v0.1)

A Dual-Perspective Framework for Application-Oriented Patent Analytics.

## Overview
Traditional patent classification systems (IPC/CPC) often fall short in capturing modern, application-oriented technology trends (e.g., AI, Quantum, LLMs). The **Bosphorus Taxonomy** introduces a bottom-up, empirical framework that classifies patents from two perspectives simultaneously: **Core Technology** and **Application Area**. 

This repository contains the v0.1 experimental release of the taxonomy in both English and Turkish, along with the keyword heuristic data and automated classification scripts.

## Automated Classification via NLP
We utilize the `intfloat/multilingual-e5-large-instruct` text embedding model to map patent abstracts and claims into our 16 main categories and their respective subcategories using zero-shot/few-shot semantic matching.

## Files in this Repository
* **`Bosphorus_Taxonomy_Whitepaper_v0.1.pdf`**: The technical note explaining the methodology and framework.
* **`Bosphorus_Taxonomy_Full.xlsx`**: The complete dual-language taxonomy table.
* **`classifier_english.ipynb` & `classifier_turkish.ipynb`**: Implementation codes using the `multilingual-e5` model.
* **`taxonomy_*.json`**: Raw data files for integration into machine learning pipelines.

## Citation
If you use this taxonomy or the scripts in your research or reports, please cite the Zenodo DOI (See the whitepaper for the full citation link).
