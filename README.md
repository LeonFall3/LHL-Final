# LHL-Final
Lighthouse Labs Final Project. Computer Vision Cancer Detection

## Summary
This project aims to create a robust and accurate computer vision-based model for breast cancer detection using digital mammography images. The model will leverage deep learning techniques, specifically Convolutional Neural Networks (CNNs), to analyze and classify mammogram images into benign and malignant categories. The model will be trained on a curated subset of the Digital Database for Screening Mammography (DDSM) dataset, which is publicly available on Kaggle.

## Project Structure

- `resnet50_classifier_model.pth`: Pre-trained ResNet-50 model weights for transfer learning.
- `data/df.pkl`: Pickled DataFrame containing image paths and labels.
- `data/csv/calc_case_description.csv`: CSV file containing information about calcification cases.
- `data/csv/mass_case_description.csv`: CSV file containing information about mass cases.
- `images/ConfusionMatrix.png`: Confusion matrix visualization of the model's performance.
- `notebooks/TabModel.ipynb`: Jupyter notebook for training and evaluating the model.
- `notebooks/data_importing.ipynb`: Jupyter notebook for data importing and preprocessing.
- `notebooks/models.ipynb`: Jupyter notebook for defining and testing different CNN architectures.
- `scripts/`: Directory containing Python scripts for data preprocessing, model training, and evaluation.

## Resources

### Data

- Rebecca Sawyer Lee, Francisco Gimenez, Assaf Hoogi, Daniel Rubin (2016). **Curated Breast Imaging Subset of DDSM [Dataset]**. The Cancer Imaging Archive. **DOI:** https://doi.org/10.7937/K9/TCIA.2016.7O02S9CY
- [CBIS-DDSM Breast Cancer Image Dataset](https://www.kaggle.com/datasets/awsaf49/cbis-ddsm-breast-cancer-image-dataset) on Kaggle

### Libraries and Tools

- Python 3.9
- PyTorch 1.13.1
- torchvision 0.14.1
- Jupyter Notebook
- Matplotlib 3.7.1
- Scikit-learn 1.3.0

### Installation

To set up the project, follow these steps:

1. Clone the repository: `git clone https://github.com/your-username/LHL-Final.git`
2. Navigate to the project directory: `cd LHL-Final`
3. Create a virtual environment (optional): `python -m venv venv` and activate it (`source venv/bin/activate` for Unix/Linux or `venv\Scripts\activate` for Windows)
4. Install the required libraries: `pip install -r requirements.txt`
5. Download the [CBIS-DDSM Breast Cancer Image Dataset](https://www.kaggle.com/datasets/awsaf49/cbis-ddsm-breast-cancer-image-dataset) and extract it into the `data/` directory.