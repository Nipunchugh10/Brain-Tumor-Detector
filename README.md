# Brain Tumor Detector

A machine learning project that analyzes MRI brain scans to classify whether a given image indicates the presence of a brain tumor or a healthy brain. Built using Python and Jupyter Notebook, this project demonstrates the application of deep learning in the field of medical image analysis.

---

## Overview

Brain tumors are among the most critical medical conditions requiring early and accurate detection. Manual analysis of MRI scans is time-consuming and subject to human error. This project automates the detection process by training a convolutional neural network (CNN) on a labeled dataset of brain MRI images, enabling the model to distinguish between tumor and non-tumor cases with measurable accuracy.

---

## Dataset

The dataset used in this project is sourced from Kaggle:

**Brain MRI Images for Brain Tumor Detection**
https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection

It consists of MRI scan images organized into two categories:

- `yes` — MRI images showing the presence of a brain tumor
- `no` — MRI images of a healthy brain with no tumor

## Methodology

The notebook follows a structured machine learning pipeline:

1. **Data Loading** — MRI images are loaded from the dataset directory and labeled accordingly.
2. **Preprocessing** — Images are resized to a uniform dimension, normalized, and augmented to improve generalization.
3. **Model Architecture** — A Convolutional Neural Network (CNN) is constructed to extract spatial features from MRI images.
4. **Training** — The model is trained on the preprocessed dataset with appropriate loss functions and optimizers.
5. **Evaluation** — Model performance is assessed using accuracy, confusion matrix, and classification metrics on the test set.
6. **Prediction** — The trained model is used to predict the class (tumor / no tumor) of unseen MRI images.

---

## Technologies Used

- Python 3
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib / Seaborn
- OpenCV
- TensorFlow / Keras
- Scikit-learn

---

## Getting Started

### Prerequisites

Make sure you have Python 3 and pip installed. Then install the required dependencies:

```bash
pip install numpy pandas matplotlib seaborn opencv-python tensorflow scikit-learn jupyter
```

### Running the Notebook

1. Clone this repository:

```bash
git clone https://github.com/Nipunchugh10/Brain-Tumor-Detector.git
cd Brain-Tumor-Detector
```

2. Download the dataset from the Kaggle link above and place it inside the `brain_tumor_dataset/` folder, maintaining the `yes/` and `no/` subfolder structure.

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `BRAIN_TUMOR_DETECTION_USING_MRI_IMAGES.ipynb` and run all cells sequentially.

---

## Results

The model is evaluated on a held-out test set. Metrics such as accuracy, precision, recall, and F1-score are reported within the notebook. A confusion matrix is also visualized to provide a clear picture of true positives, false positives, true negatives, and false negatives.

---

## Disclaimer

This project is developed for academic and research purposes only. It is not intended for clinical use or as a substitute for professional medical diagnosis. Always consult a qualified medical professional for health-related decisions.

---

## Author

**Nipun Chugh**
GitHub: [Nipunchugh10](https://github.com/Nipunchugh10)

---

## License

This project is open-source and available under the [MIT License](LICENSE).
