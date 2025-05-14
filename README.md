# Object Classification in Aerial Drone Footage

## *Computer Vision Crusaders*
- Jack Chin
- Liam McGoldrick
- Aidan Walker


## Contents
- [Overview](#overview)
- [Setup Instructions](#setup-intructions)
  - [Option 1: Colab](#option-1-run-in-google-colab)
  - [Option 2: Local](#option-2-run-locally-via-github)
- [Project Structure](#project-structure)
- [References](#references)
- [License](#license)


## Overview
The ability to accurately detect and classify objects from the air is of crucial interest to the rapidly expanding and evolving field of personal, official, and military drone use. The following project is based on the VisDrone dataset, a large repository of drone images and footage—adapted from the annual "Vision Meets Drones: A Challenge" hosted by Tianjin University—that has become a benchmark for a wide range of aerial-based computer vision projects. We use the FasterRCNN package from PyTorch, a groundbreaking model based on the research paper "Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks" by S. Ren et al., and intend to demonstrate the accuracy and effectiveness of our methods in potential real-world applications such as environmental monitoring, wildlife migration tracking, autonomous drone delivery, disaster response (search and rescue), and aerial surveillance.


## Setup Intructions
Please choose a preferred setup option below.

### Option 1: Run in Google Colab
1. Navigate to the `code/DeepLearning_MS2.ipynb` file and either download it to your device or select "Open in Colab" option at the top of the notebook.
2. Now in Colab, make sure to connect to a runtime and select the "GPU" option.
3. Press "Run all" or walk through the notebook cell by cell.

### Option 2: Run Locally via GitHub
1. First, clone the repository and navigate to the directory:
```
git clone https://github.com/ldmcgo26/deep_learning.git
cd deep_learning
```
2. This code assumes a MacOS computer and therefore `mps` as the designated device GPU. If using a Windows or Linux machine, it will be necessary to manually switch device GPU setup to `cuda`.
3. Install requirements (preferably within a virtual environment to limit system impacts).
```
pip install -r requirements.txt
```
4. Navigate to `code/dataset_setup.ipynb` and run the code to download the data directly from dropbox urls.
5. See below for the finalized project structure that should now exist on your local environment.


## Project Structure
```
deep_learning/
├── code/
│   ├── dataset_setup.ipynb 
│   ├── DeepLearning_MS1.ipynb
│   ├── MS2_Data&Baseline.ipynb
│   ├── MS2_DeepLearningModel.ipynb
│   └── PreviousVersionDeepLearningModel(for_reference).ipynb
├── data/
│   ├── VisDrone2019-DET-test-dev/
│   │   ├── annotations/
│   │   └── images/
│   ├── VisDrone2019-DET-train/
│   │   ├── annotations/
│   │   └── images/
│   ├── VisDrone2019-DET-val/
│   │   ├── annotations/
│   │   └── images/
│   ├── VisDrone2019-DET-test-dev.zip
│   ├── VisDrone2019-DET-train.zip
│   └──  VisDrone2019-DET-val.zip
├── presentations/
│   ├── Deep Learning MS1.pptx
│   ├── Deep Learning MS2.pptx
│   ├── Deep-Learning-MS1.txt
│   └── Deep-Learning-MS2.txt
├── .gitignore
├── README.md
└── requirements.txt
```


## References
- https://github.com/VisDrone/VisDrone-Dataset?tab=readme-ov-file
- http://aiskyeye.com/home/
- https://pytorch.org/vision/master/models/faster_rcnn.html
- https://arxiv.org/abs/1506.01497


## License
