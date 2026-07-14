# DFAN

Official PyTorch implementation of **DFAN**, a deep edge-detection network for the digital extraction of decorative motifs from Chinese women's robes dating from the late Qing Dynasty and early Republican period.

DFAN takes a garment image as input and predicts a pixel-level edge map that can be used to isolate and digitize decorative patterns.

<img width="830" height="420" alt="image" src="https://github.com/user-attachments/assets/36e05f39-8914-45de-9a48-ead1d1b27b35" />


## Repository structure

```text
DFAN/
├── main.py              # Training and inference entry point
├── model.py             # DFAN network definition
├── datasets.py          # Dataset loaders and preprocessing
├── losses.py            # Edge-detection loss functions
├── dexi_utils.py        # Image utility functions
├── utils/               # Visualization and result-saving helpers
├── dataset/             # Dataset notes
├── requirements.txt     # Python dependencies
└── LICENSE
```

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/sujianshuai/DFAN.git
cd DFAN
```

### 2. Create an environment

Python 3.8 or later is recommended.

```bash
conda create -n dfan python=3.10 -y
conda activate dfan
pip install -r requirements.txt
```

Main dependencies:

- PyTorch >= 1.9.0
- NumPy >= 1.19.0
- OpenCV >= 4.5.0
- Kornia >= 0.6.0
- TensorBoard >= 2.8.0

For GPU acceleration, install a PyTorch build compatible with your CUDA environment by following the [official PyTorch installation guide](https://pytorch.org/get-started/locally/).

## Citation

If you use this repository in academic work, please cite the associated paper. 

## Acknowledgements

This implementation builds on ideas and utilities from the deep edge-detection community, including the DexiNed/BIPED codebase.



