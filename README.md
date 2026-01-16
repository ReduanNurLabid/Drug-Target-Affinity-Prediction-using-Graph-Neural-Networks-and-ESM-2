# GraphDTA with ESM-2 and Cross-Attention

## 📌 Project Overview
This repository contains an advanced Deep Learning model for **Drug-Target Affinity (DTA)** prediction. The model integrates **Graph Neural Networks (GAT)** for molecular representation and **ESM-2 (Evolutionary Scale Modeling)** for protein sequence embeddings, fused via a **Bi-Directional Cross-Attention** mechanism.

The goal is to accurately predict the binding affinity between a drug molecule (SMILES) and a target protein sequence, addressing the cold-start problem (unseen drugs/targets) in drug discovery.

## 🚀 Key Features
- **Protein Encoder**: Utilizes **ESM-2 (650M parameter)** pre-trained protein language model for rich sequence representations.
- **Drug Encoder**: **Graph Attention Network (GAT)** to capture structural information of drug molecules.
- **Attention Mechanism**: **Bi-Directional Cross-Attention** (Drug-to-Protein & Protein-to-Drug) to model specific molecular interactions.
- **Robust Evaluation**: Implements **Cold-Drug** and **Cold-Target** generic splits to test generalization capabilities.
- **Metrics**: Evaluated using **MDSE (Mean Squared Error)** and **CI (Concordance Index)**.



## 📊 Performance
- **MSE**: ~0.46
- **Concordance Index (CI)**: ~0.79

## 🔗 References
- **ESM-2**: Lin et al., "Language models of protein sequences at the scale of evolution to structure optimization", 2022.
- **GraphDTA**: Nguyen et al., "GraphDTA: Predicting drug–target binding affinity with graph neural networks", 2021.
