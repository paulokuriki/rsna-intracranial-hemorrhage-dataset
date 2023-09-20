# RSNA Intracranial Hemorrhage Dataset

This repository contains code for preprocessing and exploring the RSNA Intracranial Hemorrhage Detection dataset. 

The main goal is to understand the dataset's distribution, visualize the data, and prepare smaller datasets for learning purposes.

## Dataset Overview

The dataset is sourced from the RSNA Intracranial Hemorrhage Detection challenge and consists of CT scan images labeled with different types of hemorrhages or identified as normal.

## Contents

1. **Data Loading**: Read the dataset's annotations and images.
2. **Exploratory Data Analysis (EDA)**: Visualize the dataset's distribution, including the count of normal and hemorrhage cases.
3. **Data Cleaning**: Remove cases with more than one type of hemorrhage to simplify the problem.
4. **Data Visualization**: Visual sample CT scan images for each type of hemorrhage.
5. **Preprocessing**: Convert DICOM images to PNG, resize them, and apply the appropriate windowing for brain scans.
6. **Dataset Splitting**: Create a balanced test set to ensure each class is fairly represented.

## Prerequisites

- `Python 3.11`
- `pandas`
- `pydicom`
- `tqdm`
- `matplotlib`
- `PIL` from `Pillow`

## Cloning this repository:
`git clone https://github.com/paulokuriki/rsna-intracranial-hemorrhage-dataset.git`

## Downloading the Dataset

1. Set up a Kaggle account at https://www.kaggle.com/.
2. Navigate to the [RSNA Intracranial Hemorrhage Detection Challenge](https://www.kaggle.com/competitions/rsna-intracranial-hemorrhage-detection/data) page and download the dataset.
3. Unzip the downloaded dataset.

## Setting Up the Dataset Path

In the Jupyter Notebook `prepare_dataset.ipynb`, locate the line:

`DATASET_DIR = '/media/paulo/Backup/rsna-intracranial-hemorrhage-detection/'`

Replace the path with the directory where you've unzipped the Kaggle dataset.

## Results
After running the script, the CT scan images will be processed, resized, and saved in the PNG format in a structured directory. This data will be ready for further modeling or deep learning tasks.

## Acknowledgements
Thanks to the RSNA (Radiological Society of North America) for providing the dataset.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.