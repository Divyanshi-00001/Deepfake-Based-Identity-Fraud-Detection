# Deepfake-Based Identity Fraud Detection

![Python](https://img.shields.io/badge/python-3.11+-blue.svg)
![Framework](https://img.shields.io/badge/framework-PyTorch-red.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## Project Overview

Deepfake-Based Identity Fraud Detection is a deep learning-based system developed to identify manipulated facial images used for identity fraud. The project utilizes multiple state-of-the-art convolutional and vision transformer architectures to accurately classify images as **Real** or **Deepfake** while providing visual explanations through Grad-CAM.

The system is designed for applications requiring secure digital identity verification, including banking KYC, online examinations, recruitment platforms, government identity verification, and social media account protection.

By combining multiple deep learning backbones, the project aims to improve detection robustness against different types of AI-generated facial manipulations while maintaining efficient inference performance.

---

## Features

- Multiple Deep Learning Backbones using **timm**
- Deepfake Image Classification
- Grad-CAM Heatmap Visualization
- Interactive Web Interface
- Configurable Training and Inference Pipelines
- YAML-based Experiment Configuration
- Model Evaluation with Performance Metrics
- Confusion Matrix and ROC Curve Generation
- Modular Architecture for Easy Extension

---

## Supported Models

The project currently supports the following deep learning architectures:

- EfficientNet
- FasterViT
- EfficientFormerV2-S1

Each model offers a different balance between prediction accuracy, computational efficiency, and inference speed.

---

## Applications

- Digital Identity Verification
- Banking KYC Systems
- Online Examination Proctoring
- Video Interview Verification
- Government e-Governance Services
- Cybersecurity
- Social Media Identity Protection

---

## Project Workflow

```
Input Image
      │
      ▼
Image Preprocessing
      │
      ▼
Deep Learning Model
(EfficientNet / FasterViT / EfficientFormerV2)
      │
      ▼
Prediction
(Real / Deepfake)
      │
      ▼
Confidence Score
      │
      ▼
Grad-CAM Visualization
      │
      ▼
Final Result
```

---

## Project Structure

```
Deepfake-Based-Identity-Fraud-Detection/

├── config/
├── docs/
│   └── images/
├── orchestration/
├── trainers/
├── tests/
├── inference.py
├── train.py
├── web_ui.py
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/Divyanshi-00001/Deepfake-Based-Identity-Fraud-Detection.git
```

Move to the project directory

```bash
cd Deepfake-Based-Identity-Fraud-Detection
```

Create a virtual environment (optional)

```bash
python -m venv venv
```

Activate the virtual environment

Windows

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
source venv/bin/activate
```

Install the required dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Project

### Train Models

```bash
python train.py
```

This command trains the models defined in the training configuration file and saves the trained checkpoints.

---

### Model Evaluation

```bash
python inference.py
```

This command evaluates trained models, generates predictions, computes evaluation metrics, and saves confusion matrices and ROC curves.

---

### Launch the Web Interface

```bash
python web_ui.py --config config/inference.yaml
```

The interactive interface allows users to:

- Upload an image
- Detect whether it is Real or Deepfake
- View confidence scores
- Generate Grad-CAM heatmaps
- Compare predictions across multiple models

---

## Configuration

Project settings are managed through YAML configuration files located in the `config/` directory.

These configuration files allow customization of:

- Dataset location
- Model selection
- Hyperparameters
- Batch size
- Learning rate
- Image size
- Checkpoint paths
- Data augmentation
- Evaluation settings

---

## Output

After execution, the project generates:

- Trained model checkpoints
- Evaluation metrics
- Prediction results
- Confusion Matrix
- ROC Curve
- Grad-CAM visualizations
- Logs

---

## Future Enhancements

- Real-time webcam deepfake detection
- Video-level deepfake detection
- Face Anti-Spoofing integration
- Multi-modal deepfake detection
- Explainable AI dashboard
- Mobile application support
- Cloud deployment
- Blockchain-assisted identity verification
- Agentic AI for automated fraud investigation

---

## Research Applications

This project can be applied in:

- Identity Fraud Detection
- AI-generated Media Detection
- Digital Forensics
- Cybersecurity
- Biometric Authentication
- Trustworthy Artificial Intelligence
- Financial Technology (FinTech)

---

## License

This project is released under the MIT License.

---

## Acknowledgements

This project is developed for educational and research purposes. It utilizes open-source deep learning frameworks including PyTorch, timm, OpenCV, and Grad-CAM methodologies for explainable AI.