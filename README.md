# Object Classification in Aerial Drone Footage

## Computer Vision Crusaders
Liam McGoldrick, Aidan Walker, Jack Chin

## Abstract
The ability to accurately detect and classify objects from the air is of crucial interest to the rapidly expanding and evolving field of personal, official, and military drone use. The following project is based on the VisDrone dataset, a large repository of drone images and footage—adapted from the annual "Vision Meets Drones: A Challenge" hosted by Tianjin University—that has become a benchmark for a wide range of aerial-based computer vision projects. We use the FasterRCNN package from PyTorch, a groundbreaking model based on the research paper "Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks" by S. Ren et al. We intend to demonstrate the accuracy and effectiveness of our methods in potential real-world applications such as environmental monitoring, wildlife migration tracking, autonomous drone delivery, disaster response (search and rescue), and aerial surveillance.

## Milestone 2 Updates
According to the assignment description, the codebase has been updated (primarily in DeepLearning_MS2.ipynb) to fulfill the requirements. 

## GitHub Repo Structure

deep_learning/
├── code/
│   ├── DeepLearning_MS1.ipynb
│   └── DeepLearning_MS2.ipynb
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
├── presentations/
│   ├── Deep Learning MS1.pptx
│   ├── Deep Learning MS2.pptx
│   ├── Deep-Learning-MS1.txt
│   └── Deep-Learning-MS2.txt
├──.gitignore
└── README.md

## References
- https://github.com/VisDrone/VisDrone-Dataset?tab=readme-ov-file
- http://aiskyeye.com/home/
- https://pytorch.org/vision/master/models/faster_rcnn.html
- https://arxiv.org/abs/1506.01497
