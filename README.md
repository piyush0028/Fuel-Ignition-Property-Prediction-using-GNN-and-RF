# Molecular Property Prediction Using GNN

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat&logo=PyTorch&logoColor=white)](https://pytorch.org/)
[![RDKit](https://img.shields.io/badge/RDKit-Chemoinformatics-blue)](https://www.rdkit.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Advanced Graph Neural Networks for multi-task prediction of fuel properties (DCN, MON, RON) from molecular structures with 92%+ R² accuracy.**

## 🚀 Key Features

- **Multi-task Learning**: Simultaneous prediction of DCN, MON, RON from SMILES strings
- **Graph Neural Networks**: Native molecular structure representation
- **Superior Performance**: 0.92+ R² scores vs 0.65-0.70 for Random Forest
- **End-to-End Pipeline**: Complete workflow from SMILES to predictions
- **Comprehensive Benchmarking**: Comparison with traditional ML methods

## 📊 Performance Highlights

| Property | R² Score | MAE | Improvement over RF |
|----------|----------|-----|-------------------|
| **DCN** | 0.918 | 3.32 | +66% |
| **MON** | 0.921 | 6.41 | +39% |
| **RON** | 0.927 | 6.45 | +42% |
| **Mean** | **0.922** | **5.39** | **+41%** |

## 🛠 Installation

```bash
# Clone repository
git clone https://github.com/piyush0028/Molecular-Property-Prediction-Using-GNN.git
cd Molecular-Property-Prediction-Using-GNN

# Create conda environment
conda create -n molecular-gnn python=3.8
conda activate molecular-gnn

# Install dependencies
pip install -r requirements.txt

# Install PyTorch Geometric
pip install torch torchvision torchaudio
pip install pyg-lib torch-scatter torch-sparse -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
pip install torch-geometric