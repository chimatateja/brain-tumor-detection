# ❤️ ECG-Based Cardiovascular Disease Detection

Deep learning framework for automated cardiovascular disease detection using ECG image classification. Ensemble of CNN architectures achieving **99.79% prediction accuracy**.

## Results

| Model | Accuracy |
|-------|----------|
| Baseline CNN | ~83% |
| VGG16 (Transfer Learning) | 94.1% |
| InceptionV3 (Transfer Learning) | 95.3% |
| MobileNet (Transfer Learning) | 93.8% |
| VGG16 + InceptionV3 + MobileNet Ensemble | **97.0%** |
| Lightweight Custom CNN | 98.23% |
| Final Ensemble (Naive Bayes + SVM + RF + K-NN) | **99.79%** |

## Tech Stack

- **Python** — core language
- **TensorFlow / Keras** — deep learning model training
- **Scikit-learn** — classical ML ensemble (Naive Bayes, SVM, Random Forest, K-NN)
- **NumPy / OpenCV** — image preprocessing (segmentation, noise reduction, contrast enhancement)
- **Matplotlib** — visualization and model performance analysis

## Dataset

ECG Heartbeat Categorization Dataset (publicly available on Kaggle):  
https://www.kaggle.com/datasets/shayanfazeli/heartbeat

## Project Structure

```
ecg-cardiovascular-detection/
├── ecg_cardiovascular_detection.ipynb   # Main notebook
├── README.md
└── requirements.txt
```

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook ecg_cardiovascular_detection.ipynb
```

## Key Steps

1. **Data Loading** — Load ECG signal/image dataset
2. **Preprocessing** — Segmentation, noise reduction, erosion, dilation, contrast enhancement
3. **Transfer Learning** — Fine-tune VGG16, InceptionV3, MobileNet on ECG data
4. **Custom CNN** — Lightweight architecture optimized for ECG classification
5. **Ensemble** — Combine classical ML classifiers on extracted features
6. **Evaluation** — Accuracy, PSNR, confusion matrix, classification report

## Author

Teja Chimata — [linkedin.com/in/chimatateja](https://linkedin.com/in/chimatateja)
