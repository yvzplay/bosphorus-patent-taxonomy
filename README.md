# Bosphorus Patent Technology Taxonomy (v0.1)

*A Dual-Perspective Framework for Application-Oriented Patent Analytics.*

**Developed by:** Yavuz YILMAZ

## 🌉 The Concept: Why "Bosphorus"?
Just as the Bosphorus acts as a **bridge** between two continents, this taxonomy serves as a critical **bridge** between rigid, traditional patent classifications (like IPC/CPC) and dynamic, real-world market applications. 

Traditional classification systems are highly effective at categorizing the core technical mechanics of an invention. However, they often fail to capture modern, cross-disciplinary technologies (e.g., AI, Quantum Computing, LLMs) or their intended market uses. To solve this problem, I developed the **Bosphorus Taxonomy**—a bottom-up, empirical framework designed specifically for technology scouting, portfolio segmentation, and startup/corporate matchmaking.

## 🔍 What is this Taxonomy?
Instead of a single, flat hierarchy, the Bosphorus Taxonomy evaluates patents from two simultaneous perspectives:
1. **Core Technology:** What is the underlying technical invention?
2. **Application Area:** Where and how is this technology being used in the market?

Currently in its experimental release (v0.1), the framework consists of **16 main categories** and their respective subcategories. Rather than leaving these categories abstract, I enriched them with domain-expert keyword heuristics (in both English and Turkish) to make them machine-readable.

## 🤖 Automated Classification via NLP
This framework is not just a static theoretical table; it is designed to be NLP-ready. 

In this repository, you will find my Python implementation that automates the classification process. By utilizing the `intfloat/multilingual-e5-large-instruct` text embedding model, the script maps patent abstracts and claims against my taxonomy's keyword heuristics. This enables highly accurate, zero-shot/few-shot semantic matching without the need for massive labeled training datasets.

## 📂 Files in this Repository
* **`Bosphorus_Taxonomy_Whitepaper_v0.1.pdf`**: The technical note explaining the design principles, methodology, and the full framework.
* **`Bosphorus_Taxonomy_Full.xlsx`**: The complete dual-language taxonomy table for easy viewing.
* **`classifier_english.ipynb` & `classifier_turkish.ipynb`**: My implementation notebooks for automated patent classification using the `multilingual-e5` model.
* **`taxonomy_*.json`**: Raw data files (in English and Turkish) ready to be integrated into your own machine learning pipelines.

## 📄 Citation
If you use this taxonomy, the dual-perspective framework, or the provided NLP scripts in your research, commercial reports, or software pipelines, please cite the Zenodo DOI:

> Yilmaz, Yavuz. (2026). Bosphorus Patent Technology Taxonomy: A Dual-Perspective Framework for Application-Oriented Patent Analytics. Zenodo. https://doi.org/10.5281/zenodo.XXXXXXX
