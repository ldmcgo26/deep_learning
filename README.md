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
Please choose a preferred setup option below (we strongly recommend Google Colab for ease of use and as that was our primary coding environment).

### Option 1: Run in Google Colab
1. Navigate to the `code/DeepLearning_Final.ipynb` file and download it to your device.
2. Now in Colab, open the file and make sure to connect to a runtime and select the "GPU" option.
3. Press "Run all" or walk through the notebook cell by cell.
4. See below for the data structure that should exist in your Colab environment after the initial data download steps:

```
VisDrone/
├── VisDrone2019-DET-test-dev/
│   ├── annotations/
│   └── images/
├── VisDrone2019-DET-train/
│   ├── annotations/
│   └── images/
├── VisDrone2019-DET-val/
│   ├── annotations/
│   └── images/
├── VisDrone2019-DET-test-dev.zip
├── VisDrone2019-DET-train.zip
└──  VisDrone2019-DET-val.zip
```

### Option 2: Run Locally via GitHub
1. First, clone the repository and navigate to the directory:
```
git clone https://github.com/ldmcgo26/deep_learning.git
cd deep_learning
```
2. *Important Note:* This code assumes a Windows computer and therefore `cuda` as the designated device GPU. If using a MacOS computer or `cuda` is not available, it will be necessary to manually switch device GPU setup to `mps`, `cpu`, or another option of your choice.
3. Install requirements (preferably within a virtual environment to limit system impacts).
```
pip install -r requirements.txt
```
4. Navigate to `code/dataset_setup.ipynb` and run the code to download the data directly from dropbox urls.
5. See below for the finalized project structure that should now exist on your local environment.
6. Navigate to `code/DeepLearning_Final(local).ipynb` and run the code.

```
deep_learning/
├── code/
│   ├── dataset_setup.ipynb 
│   ├── DeepLearning_Final(local).ipynb
│   ├── DeepLearning_Final.ipynb
│   ├── MS1_DataProcessing.ipynb
│   ├── MS2_Data&Baseline.ipynb
│   └── MS2_DeepLearningModel.ipynb
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
│   └── VisDrone2019-DET-val.zip
├── files/
│   ├── Deep Learning Final Presentation.pptx
│   ├── Deep Learning Final Report.pdf
│   ├── Deep Learning MS1.pptx
│   └── Deep Learning MS2.pptx
├── .gitignore
├── README.md
└── requirements.txt
```


## References
- https://github.com/VisDrone/VisDrone-Dataset?tab=readme-ov-file
- http://aiskyeye.com/home/
- https://pytorch.org/vision/master/models/faster_rcnn.html
- https://arxiv.org/abs/1506.01497


## Citation

This project uses the [VisDrone](http://aiskyeye.com/) dataset for object detection and tracking tasks. The following paper is cited:

**Detection and Tracking Meet Drones Challenge**  
Pengfei Zhu, Longyin Wen, Dawei Du, Xiao Bian, Heng Fan, Qinghua Hu, Haibin Ling  
*IEEE Transactions on Pattern Analysis and Machine Intelligence*, Vol. 44, No. 11, pp. 7380–7399, 2021. https://ieeexplore.ieee.org/document/9573394