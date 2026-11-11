
# Rice Leaf Disease Detection

## Project Overview
This project focuses on classifying rice leaf diseases using Machine Learning and Deep Learning techniques.

The objective is to identify three major rice leaf diseases from leaf images.

## Disease Categories
1. Bacterial Leaf Blight
2. Brown Spot
3. Leaf Smut

## Dataset Information
- Total images: 119
- Bacterial Leaf Blight: 40
- Brown Spot: 40
- Leaf Smut: 39
- Image format: JPG
- Input image size: 224 x 224

## Exploratory Data Analysis
- Image dimensions and format analysis
- Image quality and integrity checks
- Duplicate image analysis
- RGB histogram analysis
- Background variation analysis
- Image visualization

## Models Implemented
1. HOG + Tuned SVM
2. Custom CNN
3. MobileNetV2
4. EfficientNetB0

## Model Comparison

| Model | Validation Accuracy |
|---|---:|
| HOG + Tuned SVM | 77.78% |
| Custom CNN | 77.78% |
| MobileNetV2 | 88.89% |
| EfficientNetB0 | 100.00% |

## Final Test Results

Selected model: EfficientNetB0

| Metric | Result |
|---|---:|
| Test Accuracy | 83.33% |
| Macro Precision | 85.71% |
| Macro Recall | 83.33% |
| Macro F1-score | 83.08% |

## Data Augmentation
Experimented with:
- Random Horizontal Flip
- Random Rotation
- Random Zoom
- Random Translation

The controlled augmentation experiment did not improve the Custom CNN validation performance.

## Technologies Used
- Python
- Jupyter Notebook
- TensorFlow and Keras
- Scikit-learn
- Scikit-image
- NumPy
- Pandas
- Matplotlib
- Pillow

## Installation

Install the required packages:

```bash
pip install -r requirements.txt
```

## How to Run the Project

1. Download or clone this repository.
2. Make sure the dataset folders are available inside the repository root.
3. Open a terminal in the parent directory of the repository.
4. Start Jupyter Notebook from that parent directory.
5. Open Rice_Leaf_Disease_Detection.ipynb.
6. Execute the notebook cells.

### Important Dataset Path Note

The notebook uses its existing working-directory-based dataset path.

For the supplied notebook code to work without modification, the cloned repository folder should be named:

Rice Leaf Disease using CNN

For example, clone it using:

```bash
git clone https://github.com/kalipindiprasanthsai1267-hub/Rice-Leaf-Disease-Detection.git "Rice Leaf Disease using CNN"
```

Then start Jupyter Notebook from the directory containing that folder.

## Project Limitations
The dataset contains only 119 images. Although EfficientNetB0 achieved 83.33% test accuracy, more diverse images and independent evaluation are required before real-world deployment.

## Author
Kalipindi Prasanth Sai
