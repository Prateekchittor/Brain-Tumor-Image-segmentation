Brain Tumor Image Segmentation using FPN and 3D U-Net

This project focuses on automatic brain tumor segmentation from MRI scans using deep learning models — Feature Pyramid Network (FPN) and 3D U-Net.
It leverages the BRaTS 2020 dataset, enabling accurate detection and segmentation of tumor regions including whole tumor (WT), tumor core (TC), and enhancing tumor (ET).

<img width="753" height="477" alt="image" src="https://github.com/user-attachments/assets/a54a6dcd-e6c9-49ff-9c24-5d59b49202df" />


🚀 Overview

Accurate brain tumor segmentation is crucial for diagnosis, treatment planning, and monitoring.
This project uses encoder–decoder architectures that effectively capture both global context and fine spatial details in 3D medical images.



We train and compare FPN and 3D U-Net architectures on multi-modal MRI data to achieve high segmentation accuracy across different tumor regions.

🧩 Key Features

🧬 Multimodal MRI Inputs – Utilizes T1, T2, T1ce, and FLAIR modalities

🧠 3D U-Net Architecture – Captures volumetric spatial context efficiently

🏗️ Feature Pyramid Network (FPN) – Enhances multi-scale feature extraction for small tumor regions

🎯 Multi-class Segmentation – Segments WT, TC, and ET tumor subregions

📈 Evaluation Metrics – Dice Score, IoU, Precision, Recall

⚙️ Preprocessing Pipeline – Skull stripping, normalization, and patch extraction

💾 Dataset: BRaTS 2020 Challenge Dataset

🧠 Model Architectures
🧩 3D U-Net

Encoder–decoder architecture for volumetric data

Skip connections for spatial detail preservation

Handles 3D MRI scans directly using 3×3×3 convolutions

🧩 Feature Pyramid Network (FPN)

Built on a 2D/3D CNN backbone

Combines feature maps from multiple scales

Improves segmentation of small or diffuse tumor regions

🧮 Dataset – BRaTS 2020

Source: Multimodal Brain Tumor Segmentation Challenge 2020

Data: 369 subjects with multi-sequence MRI (T1, T2, T1ce, FLAIR)

Annotations: Manually labeled ground truth masks for 3 tumor regions

Preprocessing Steps:

NIfTI to NumPy conversion

Intensity normalization

Patch extraction and augmentation

Train/validation split (80/20)
