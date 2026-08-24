# ATML — Assignment 0

Repository structure:

```
.
├── data/                       # shared datasets (CIFAR-10, MNIST, STL-10, etc.); gitignored
├── weights/                    # saved model checkpoints (.pt); gitignored
├── Task1_CNN/                  # ResNet-152: baseline, skip-connection ablation, feature hierarchies, transfer learning
│   └── Task1_ResNet152_CNN.ipynb
├── Task2_ViT/                  # Vision Transformer: classification, attention-map visualization, patch masking
├── Task3_CLIP/                 # CLIP: zero-shot classification, modality gap, Procrustes alignment
├── Task4_VAE/                  # Variational Autoencoder on MNIST
├── requirements.txt
└── README.md
```

## Setup

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Alternatively, you could use any existing venv/conda environment with the requirements installed.

Datasets are downloaded automatically by each notebook (via `torchvision.datasets`) into `data/`,
so this folder is excluded from version control (see `.gitignore`).

Model checkpoints saved during training are written to the shared `weights/` folder (e.g.
`weights/baseline_resnet152_head.pt`), also excluded from version control.

## Notebooks

- **Task1_CNN/Task1_ResNet152_CNN.ipynb** 
- **Task2_ViT/Task2_ViT.ipynb** 
- **Task3_CLIP/Task3_CLIP.ipynb** 
- **Task4_VAE/Task4_VAE.ipynb** 
