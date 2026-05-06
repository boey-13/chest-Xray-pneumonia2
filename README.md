# UECS2523 Group 1 - Pneumonia Classification

## Project Overview
This project uses deep learning to classify chest X-ray images into two classes: `NORMAL` and `PNEUMONIA`.

Main implementation file:

- `UECS2523_Group1_Source_Code.ipynb`

Included models:

- CNN baseline model
- EfficientNetB0 (Stage 1 frozen backbone + Stage 2 fine-tuning)

## Dataset
Dataset source:
[Chest X-Ray Images (Pneumonia) - Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)

Expected folder structure after download and extraction:

```text
data/
└── chest_xray/
    ├── train/
    │   ├── NORMAL/
    │   └── PNEUMONIA/
    ├── val/
    │   ├── NORMAL/
    │   └── PNEUMONIA/
    └── test/
        ├── NORMAL/
        └── PNEUMONIA/
```

## Environment Setup
Recommended:

- Python 3.10+
- TensorFlow / Keras
- NumPy
- pandas
- matplotlib
- seaborn
- scikit-learn
- Kaggle API (optional, for in-notebook download)

Install dependencies (example):

```bash
pip install tensorflow numpy pandas matplotlib seaborn scikit-learn kaggle
```

## How to Run
1. Open `UECS2523_Group1_Source_Code.ipynb`.
2. Prepare Kaggle API credentials or manually download the dataset.
3. Run all cells in order from top to bottom.
4. Review outputs including curves and evaluation metrics.

## Notebook Workflow
- Import dependencies
- Download and unzip dataset
- Data statistics and path check
- Part A: CNN training and evaluation
- Part B: EfficientNetB0 training and evaluation

Evaluation outputs include:

- Confusion matrix
- Classification report
- ROC / AUC
- Training and validation curves

## Key Hyperparameters
- Image size: `224 x 224`
- Batch size: `32`
- CNN optimizer: `Adam(learning_rate=1e-3)`
- EfficientNet fine-tuning optimizer: `Adam(learning_rate=1e-5)`

## Final Results (Fill In)
Use this section for final report submission.

- CNN Test Accuracy: `__`
- CNN AUC: `__`
- EfficientNetB0 Test Accuracy: `__`
- EfficientNetB0 AUC: `__`
- Best model selected: `__`
- Conclusion summary: `__`

## Security Note
Do not commit personal API keys or credentials into source files or notebook cells.

If credentials were previously exposed, revoke and regenerate them immediately.
