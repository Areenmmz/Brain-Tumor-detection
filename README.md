This project focuses on the classification of MRI scans to detect brain tumors, utilizing a dataset containing 4,065 images categorized into "Brain Tumor" and "Healthy" classes.

Dataset obtained: https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection

### Project Overview
The primary goal is to develop a machine learning pipeline capable of pre-processing raw medical imagery and accurately identifying the presence of tumors. The project encompasses the following key stages:

* **Data Pre-processing:** Raw images are converted to grayscale, resized to 256 256 resolution, and normalized to a floating-point range (0 to 1) to ensure feature consistency across the dataset.
* **Exploratory Data Analysis (EDA):** Initial analysis confirmed the dataset distribution with 3,282 training images, 395 test images, and 388 validation images.
* **Modeling:** The project implements a **Gaussian Naive Bayes (GaussianNB)** model, which was trained and optimized to provide automated diagnostics.
* **Evaluation:** The model's performance is measured using standard classification metrics, including accuracy, a detailed classification report, and a confusion matrix on the validation set.

### Key Technologies
* **Languages & Libraries:** Python, NumPy, PIL (Pillow), Scikit-image, Scikit-learn.
* **Model Deployment:** The final trained model is serialized using **Pickle** (`GaussianNB_model.pkl`) for potential integration into broader diagnostic applications.
