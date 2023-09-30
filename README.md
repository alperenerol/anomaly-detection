# Unsupervised Anomaly Detection on Medical Images Project - Alperen Erol

This project repository contains two Jupyter Notebook files. The
guidance about the required processes, commands and libraries to test
and review these notebooks is provided below.

To download the Medical Segmentation Decathlon Dataset to the working
directory, please use this link:

https://msd-for-monai.s3-us-west-2.amazonaws.com/Task06_Lung.tar

In a Linux environment, it can be downloaded to the working directory
using this command:

wget https://msd-for-monai.s3-us-west-2.amazonaws.com/Task06_Lung.tar

To extract .tar file to the directory \>\> tar -xvf Task06_Lung.tar

Required libraries:

GenerativeModels

matplotlib 3.7.2

monai 1.2.0

nibabel 5.1.0

numpy 1.24.4

seaborn 0.12.2

session_info 1.0.0

skimage 0.21.0

sklearn 1.3.0

torch 2.0.1+cu117

tqdm 4.66.1

Assuming the existence of a Python environment and presence of a GPU,
required libraries can be installed using following commands:

pip install torch torchvision torchaudio -f
https://download.pytorch.org/whl/cu112/torch_stable.html

pip install nibabel matplotlib

pip install monai

pip install --upgrade monai

pip install seaborn

pip install "monai-weekly\[tqdm\]"

pip install scikit-learn

pip install scikit-image

GenerativeModels library should be cloned to the working directory
using:

git clone https://github.com/Project-MONAI/GenerativeModels.git

\*Note: GenerativeModels folder will also be provided as supplementary
material.

To install GenerativeModels after download, move into the
GenerativeModels directory and run this command:

python setup.py install

# Preparation of Dataset and Important Information

After the download of the LungCT dataset, 3D DecathlonDataset should be transformed to 2D Normal/Abnormal Images 
by using 'MSD-LungCT-Transform.ipynb' notebook. This notebook creates normal and abnormal 2D image slices directories in the working directory. To run the project notebook 'anomaly_detection_LungCT.ipynb', notebooks, GenerativeModels directory, dataset.json and 2D image slices directory should be located in the working directory.
