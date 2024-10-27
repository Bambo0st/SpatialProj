# Plant Disease Detection using Machine Learning

This project is an implementation of automated plant disease detection using machine learning, leveraging feature extraction and classification models to achieve accurate predictions on plant health status.

## Project Overview

This project, completed at the International Institute of Information Technology Bangalore, uses the Plant Village dataset to detect plant diseases. The study involved feature extraction techniques and machine learning models, ultimately leading to significant accuracy improvements.

**Team Members:**
- Goutham U R (IMT2021045)
- Adithya Nagaraja Somasalle (IMT2021054)
- Meher Ashish Nori (IMT2021085)

## Table of Contents

1. [Dataset](#dataset)
2. [Methodology](#methodology)
3. [Feature Extraction Techniques](#feature-extraction-techniques)
4. [Models Used](#models-used)
5. [Results](#results)
6. [Installation](#installation)
7. [Usage](#usage)
8. [Conclusion](#conclusion)

## Dataset

We used the Plant Village dataset, which includes images of leaves from three plant species: Tomato, Potato, and Pepper Bell. Each species covers a variety of diseases, providing a robust dataset for training and evaluation.

- **Species and Diseases:** 
  - Tomato: Mosaic Virus, Late Blight, Leaf Mold, Bacterial Spot, etc.
  - Potato: Early Blight, Late Blight, Healthy
  - Pepper Bell: Bacterial Spot, Healthy

- **Use Cases:** 
  - Disease detection, yield prediction, crop monitoring, and agricultural research.

## Methodology

The project methodology follows three phases:
1. **Data Selection and Analysis:** Data pre-processing and feature extraction.
2. **Model Training:** Various machine learning models were tested.
3. **Evaluation and Optimization:** Model performance was optimized with feature extraction.

## Feature Extraction Techniques

1. **Canny Edge Detection:** Highlights edges, aiding in structural analysis of diseased areas.
2. **Color Histogram:** Represents the distribution of color intensities, capturing color patterns that differ between healthy and diseased plants.
3. **GLCM Texture Features:** The Gray Level Co-occurrence Matrix (GLCM) analyzes textural nuances, enhancing discrimination between disease types.

Libraries used: `cv2` for Canny Edge Detection and Color Histogram, and `mahotas` for GLCM Texture Features.

## Models Used

The following machine learning models were evaluated:
- **K-Nearest Neighbors (KNN)**
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **XGBoost Classifier**

## Results

| Plant    | Model           | Accuracy | F1 Score |
|----------|------------------|----------|----------|
| Tomato   | KNN              | 53.3%    | 0.53     |
| Tomato   | Random Forest    | 69%      | 0.68     |
| Tomato   | XGBoost          | 84.1%    | 0.84     |
| Potato   | XGBoost          | 94.2%    | 0.938    |
| Pepper   | XGBoost          | 94.5%    | 0.945    |

- **Best Model:** XGBoost classifier, achieving the highest accuracy (94.5%) with feature extraction.
