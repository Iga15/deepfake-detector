# deepfake-detector
Two-stream deepfake detection model combining CNN image features with facial landmark data (via MediaPipe).

## Overview
- Custom CNN trained on real and fake face images.
- Two inputs:
  - RGB face image (256×256)
  - 3D facial landmarks (21 selected points)
- Outputs a binary classification: Real / Fake.
- Includes training and inference notebooks.

## Project Structure
deepfake-detector/
├── configs/          # config files (paths, settings)
├── data/             # datasets (not included)
├── models/           # trained model weights
├── notebooks/        # training + inference notebooks
├── runs/             # outputs, saved arrays, logs
├── requirements.txt
└── README.md

## How to Run
1. Install dependencies  
   ```bash
   pip install -r requirements.txt

2.	Add your dataset under data/train, data/test, and data/validate.
3.	Run notebooks/advanced_deepfake_detector.ipynb to train.
4.	Run notebooks/deepfake_detector_final.ipynb to test or predict new images.