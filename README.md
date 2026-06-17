# 🧠 Brain Tumor Detection using CNN

Deep learning system for automated brain tumor detection and classification from MRI images using Convolutional Neural Networks (CNNs). Classifies tumors as **benign** or **malignant** with advanced image preprocessing techniques.

## Results

| Model | Accuracy |
|-------|----------|
| Baseline CNN | 87.4% |
| CNN + Image Preprocessing | 92.1% |
| CNN + Augmentation | 94.8% |
| **Optimized CNN (Final)** | **96.5%** |

## Tech Stack

- **Python** — core language
- **TensorFlow / Keras** — CNN model building and training
- **OpenCV** — image preprocessing (segmentation, noise reduction, erosion, dilation, contrast enhancement)
- **NumPy / Pandas** — data manipulation
- **Matplotlib / Seaborn** — visualization and performance analysis
- **Scikit-learn** — evaluation metrics and data splitting

## Dataset

Brain MRI Images for Brain Tumor Detection (publicly available on Kaggle):  
https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection

## Project Structure

```
brain-tumor-detection/
├── brain_tumor_detection.ipynb   # Main notebook
├── README.md
└── requirements.txt
```

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook brain_tumor_detection.ipynb
```

## Key Steps

1. **Data Loading** — Load MRI brain scan images
2. **Preprocessing** — Segmentation, noise reduction, erosion, dilation, contrast enhancement
3. **Data Augmentation** — Rotation, flipping, zoom to balance classes
4. **CNN Architecture** — Custom CNN with BatchNormalization and Dropout
5. **Training** — EarlyStopping and ReduceLROnPlateau callbacks
6. **Evaluation** — Accuracy, PSNR, confusion matrix, classification report
7. **Visualization** — GUI-based interactive tool for healthcare analysis

## Author

Teja Chimata — [linkedin.com/in/chimatateja](https://linkedin.com/in/chimatateja)
