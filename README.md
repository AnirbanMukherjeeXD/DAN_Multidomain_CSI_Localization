# Multi-domain CSI-based Indoor Localization with Deep Attention Networks (DAN) for MIMO JCAS system

**Authors**:  
Anirban Mukherjee, Praneeth Susarla , Pravallika Katragunta , S. S. Krishna Chaitanya Bulusu, Olli Silven , Markku Juntti, Dinesh Babu Jayagopi, and Miguel Bordallo Lopez 

📄 **Published in:** 2025 IEEE 5th International Symposium on Joint Communications & Sensing (JC&S)  
🔗 **Paper Link:** [IEEE Xplore](https://ieeexplore.ieee.org/document/10880643)  

---

This repository contains the source code and training scripts for the models presented in our research paper titled **"Multi-domain CSI-based Indoor Localization with Deep Attention Networks (DAN) for MIMO JCAS system"**.

We propose a deep learning-based approach to indoor localization using Channel State Information (CSI) from multiple domains — **Complex** and **Polar** representations across different subcarrier groups (domains). Our final model utilizes a deep attention-based architecture (DAN) to effectively fuse and learn from multi-domain CSI data.

---

## 🧠 Model Variants

| Model No. | Input Domains        | CSI Representation   | Description                          |
|-----------|----------------------|-----------------------|--------------------------------------|
| Model 1   | Domain 1 + 2         | Complex               |                                      |
| Model 2   | Domain 1 + 2         | Polar                 |                                      |
| Model 3   | Domain 1 + 2         | Complex + Polar       |                                      |
| Model 4   | Domain 2 + 3         | Complex               |                                      |
| Model 5   | Domain 2 + 3         | Polar                 |                                      |
| Model 6   | Domain 2 + 3         | Complex + Polar       |                                      |
| Model 7   | Domain 1 + 3         | Complex               |                                      |
| Model 8   | Domain 1 + 3         | Polar                 |                                      |
| Model 9   | Domain 1 + 3         | Complex + Polar       |                                      |
| Model 10  | Domain 1 + 2 + 3     | Complex               |                                      |
| Model 11  | Domain 1 + 2 + 3     | Polar                 |                                      |
| Model 12  | Domain 1 + 2 + 3     | Complex + Polar       |                                      |
| Model 13  | Domain 1 (C) + 2 (C+P)| Complex + Polar      | Benchmark model                      |
| **Model 14** | Domain 1 + 2 + 3 | Complex + Polar       | **DAN (Final proposed model)**       |

---

## 📁 Repository Structure

```
├── CSI_Localization_Multidomain_Data.ipynb    # Main Jupyter notebook with model training and evaluation
└── README.md                                  # Project documentation (this file)
```

---

## 🚀 Getting Started

### Prerequisites
- tensorflow==2.15

- ### Running the Notebook

To train and evaluate the models:

```bash
jupyter notebook CSI_Localization_Multidomain_Data.ipynb
```

## 📊 Evaluation

- The models are evaluated based on localization accuracy using multi-domain CSI features.
- Final performance comparisons between the 14 models are included in the paper.

---

## 🏆 Key Contributions

- Introduced a deep attention network (DAN) to fuse multi-domain CSI data effectively.
- Benchmarked 13 different combinations of domain and representation to validate the effectiveness.
- Demonstrated significant improvements in indoor localization accuracy using our DAN model.

---

## 📄 Citation

If you find this work helpful, please consider citing our paper:

**IEEE Xplore:** [https://ieeexplore.ieee.org/document/10880643](https://ieeexplore.ieee.org/document/10880643)  
**DOI:** [10.1109/ICASSP48485.2024.10880643](https://doi.org/10.1109/ICASSP48485.2024.10880643)
```
@inproceedings{mukherjee2025multi,
  title={Multi-domain CSI-based Indoor Localization with Deep Attention Networks for MIMO JCAS system},
  author={Mukherjee, Anirban and Susarla, Praneeth and Katragunta, Pravallika and Bulusu, SS Krishna Chaitanya and Silven, Olli and Juntti, Markku and Jayagopi, Dinesh Babu and Lopez, Miguel Bordallo},
  booktitle={2025 IEEE 5th International Symposium on Joint Communications \& Sensing (JC\&S)},
  pages={1--6},
  year={2025},
  organization={IEEE}
}

```

---
