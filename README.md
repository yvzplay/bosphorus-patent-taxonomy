# Bosphorus Patent Technology Taxonomy (v0.1)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20049463.svg)](https://doi.org/10.5281/zenodo.20049463)

*A Dual-Perspective Framework for Application-Oriented Patent Analytics.*

**Developed by:** Yavuz YILMAZ  
**Version:** v0.1 — Experimental Release

---

## 🌉 The Concept: Why "Bosphorus"?

Just as the Bosphorus acts as a **bridge** between two continents, this taxonomy serves as a bridge between traditional patent classification systems and real-world technology applications.

Established systems such as IPC and CPC are highly valuable for organizing patents according to technical subject matter. However, they may not always provide sufficient flexibility for analyzing emerging, cross-disciplinary, and market-oriented technologies such as artificial intelligence, quantum technologies, autonomous systems, digital health, advanced materials, or next-generation energy solutions.

The **Bosphorus Patent Technology Taxonomy** was developed as a bottom-up and empirical framework to support practical patent analytics, including technology scouting, portfolio segmentation, competitive intelligence, R&D strategy, and startup/corporate matchmaking.

---

## 🔍 What is this Taxonomy?

Instead of relying on a single classification hierarchy, the Bosphorus Taxonomy evaluates patents from two complementary perspectives:

1. **Core Technology**  
   What is the underlying technical invention?

2. **Application Area**  
   Where and how is this technology being used in the market?

In its experimental v0.1 release, the framework consists of **23 main categories**:

- **10 Core Technology categories**
- **13 Application Area / Sector categories**

Each main category is further supported by subcategories and bilingual keyword heuristics in **English and Turkish**. This structure allows the taxonomy to be used both as a manual analytical framework and as a machine-readable classification layer for NLP-based patent analytics.

---

## 🧭 Taxonomy Structure

### Core Technology Categories

1. Software, Data and Artificial Intelligence  
2. Electrical, Electronics and Embedded Systems  
3. Semiconductor and Microelectronics  
4. Network, Transmission and Connectivity Technologies  
5. Optics, Photonics and Imaging Technologies  
6. Mechanical, Mechatronic and Robotic Systems  
7. Chemistry, Materials and Surface Technologies  
8. Biotechnology and Life Sciences Technologies  
9. Energy and Environmental Technologies  
10. Quantum Technologies  

### Application Area / Sector Categories

1. Healthcare, Medicine and Life Sciences  
2. Automotive, Mobility and Transportation  
3. Industrial Manufacturing and Industry  
4. Energy, Infrastructure and Utilities  
5. Information Technologies and Digital Services  
6. Telecommunication Services and Network Operations  
7. Electronics and Smart Consumer Devices  
8. Construction, Building and Built Environment Technologies  
9. Agriculture, Food and Bioresource Systems  
10. Aerospace, Space and Defense  
11. Chemicals, Materials and Process Industries  
12. Textile, Apparel and Footwear  
13. Living Spaces and Consumer Products  

---

## 🤖 Automated Classification via NLP

This framework is not intended to be only a static taxonomy table. It is designed to be **NLP-ready**.

The repository includes Python-based classification workflows that use the `intfloat/multilingual-e5-large-instruct` text embedding model. The approach maps patent titles, abstracts, claims, and selected description fields into a semantic vector space and compares them against the taxonomy’s category and keyword representations.

This enables zero-shot or few-shot semantic classification without requiring a large manually labeled training dataset. The dual-perspective structure allows each patent to be analyzed both in terms of its underlying technical basis and its market or application context.

In practice, this makes the taxonomy useful for:

- Patent portfolio segmentation
- Technology-to-market mapping
- Competitive intelligence
- R&D and innovation strategy
- Startup and corporate technology matching
- Semantic clustering beyond IPC/CPC codes

---

## 📂 Files in this Repository

- **`Bosphorus_Taxonomy_Whitepaper_v0.1.pdf`**  
  Technical note explaining the motivation, design principles, methodology, limitations, and full framework.

- **`Bosphorus_Taxonomy_Full.xlsx`**  
  Complete bilingual taxonomy table, including main categories, subcategories, and keyword heuristics.

- **`classifier_english.ipynb`** and **`classifier_turkish.ipynb`**  
  Example implementation notebooks for automated patent classification using the `multilingual-e5` embedding model.

- **`taxonomy_*.json`** and **`keywords_*.json`**  
  Raw taxonomy and keyword data files in English and Turkish, ready for integration into machine learning or patent analytics pipelines.

---

## ⚠️ Status and Disclaimer

Bosphorus Patent Technology Taxonomy v0.1 is an **experimental release**.

The taxonomy is currently being tested on real-world patent data. Category boundaries, keyword coverage, similarity thresholds, and classification performance may be refined in future versions. The current release should therefore be considered a working version rather than a finalized standard.

Planned future improvements include:

- Expert-labeled validation datasets
- Category-level precision, recall, and F1-score evaluation
- Empirical optimization of multi-label classification thresholds
- Subcategory-level classification testing
- Comparison with IPC/CPC-based patent classifications
- LLM-assisted keyword expansion and taxonomy updates

---

## 📄 Citation

If you use this taxonomy, the dual-perspective framework, or the provided NLP scripts in your research, commercial reports, or software pipelines, please cite the Zenodo DOI:

**Yilmaz, Y. (2026). Bosphorus Patent Technology Taxonomy: A Dual-Perspective Framework for Application-Oriented Patent Analytics (v0.1). Zenodo. https://doi.org/10.5281/zenodo.11122606**
