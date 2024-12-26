# Brain Tumor Detection Using YOLOv8

## Overview

This project aims to develop an AI-based tool for detecting and segmenting brain tumors in medical images using **YOLOv8**, a state-of-the-art object detection and segmentation model. The primary goal is to assist healthcare professionals by automating the detection process, making it faster and more accurate. The project leverages a custom dataset for training the model and uses Roboflow for managing and deploying the dataset.

## Project Steps

1. **Dataset Preparation**:
   - The dataset used for training and evaluation is sourced from **Roboflow**, a platform that provides labeled medical images. The dataset includes brain tumor images, each annotated with pixel-level segmentation masks.
   
2. **Model Training**:
   - YOLOv8, specifically the segmentation variant (`yolov8s-seg.pt`), is fine-tuned on the custom brain tumor dataset. The training process helps the model learn to detect and segment tumors from MRI or CT scan images.
   
3. **Model Evaluation**:
   - After training, the model’s performance is assessed using common evaluation metrics such as confusion matrices and segmentation accuracy. This step helps ensure that the model is capable of correctly identifying tumor regions and minimizing errors.
   
4. **Inference and Prediction**:
   - The trained model is used to perform inference on new, unseen test images. The model generates segmentation masks that highlight the tumor regions in the test images.
   
5. **Model Deployment**:
   - The trained model is deployed to **Roboflow**, allowing it to be accessed via an API. This enables real-time predictions in cloud-based applications, making the model easily accessible for various users.

## Objective

The ultimate goal of this project is to provide healthcare professionals with an automated tool for detecting and segmenting brain tumors. By leveraging the power of deep learning, the tool can help speed up the diagnostic process and improve accuracy in identifying tumors in medical imaging scans.

## Key Features

- **Segmentation**: YOLOv8 performs not just detection but also segmentation, providing pixel-level accuracy for tumor localization.
- **Cloud Deployment**: The model is deployed via Roboflow’s API, allowing it to scale and be accessed in real-time.
- **Customizable**: The model can be retrained with new data as needed, allowing it to adapt to different types of brain tumor images or additional training data.
- **Open-Source**: The code is open-source, making it easy for researchers and developers to customize and contribute to the project.

## Future Work

- **Enhanced Dataset**: Include more diverse brain tumor types and additional medical image modalities (e.g., CT scans, MRIs) to improve model generalization.
- **Model Optimization**: Improve the model's performance in terms of accuracy, speed, and memory efficiency.
- **Clinical Integration**: Integrate the model into clinical settings, enabling healthcare professionals to utilize it in real-time decision-making.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- **YOLOv8**: For providing an efficient object detection and segmentation framework.
- **Roboflow**: For offering an easy-to-use platform to manage datasets and deploy models.
- **Open-Source Community**: For their continuous contributions to AI and machine learning advancements.
