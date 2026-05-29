# Multi-Class Garbage Classification Model

This project is a comprehensive Image Classification implementation developed as a submission for **Dicoding**, in collaboration with the **Pijar Camp x IBM SkillsBuild** program. The model is trained to classify images into 12 distinct types of garbage categories to support automated waste management systems.

## Project Background
As part of the AI & Machine Learning path supported by IBM SkillsBuild and Pijar, this project demonstrates the practical application of Deep Learning using TensorFlow and Keras. The main goal is to build an efficient Convolutional Neural Network (CNN) capable of high-accuracy predictions while maintaining a deployment-ready architecture.

## Model Performance & Architecture
* **Framework:** TensorFlow 2.x & Keras
* **Dataset Size:** >15,000 images spanning 12 different garbage classes.
* **Architecture:** Custom CNN featuring Sequential Convolutional layers, MaxPooling, and Dropout to optimize regularization and eliminate overfitting.
* **Optimization:** Fine-tuned using the Adam optimizer with a controlled learning rate (0.0001).
* **Evaluation Metrics:** Achieved an accuracy score of **85.65%** on the independent Testing Set, fully meeting the criteria for a high-tier certification.

## Deployment Formats Included
To fulfill modern deployment needs across different ecosystems, the trained model has been successfully exported into three mandatory formats:
1. **SavedModel (`/saved_model`):** Standard production format for server-side environments.
2. **TensorFlow.js (`/tfjs_model`):** Client-side format containing `model.json` and fragmented weight shards for direct browser-based deployment.
3. **TensorFlow Lite (`/tflite`):** Lightened mobile format containing `model.tflite` along with its corresponding `label.txt` for edge-device integration.

## Repository Structure
```text
├── saved_model/          # Server production model
├── tfjs_model/           # Web-ready deployment files
├── tflite/               # Mobile deployment file & labels
├── requirements.txt      # Environment dependencies
├── notebook.ipynb        # Complete training workflow pipeline
└── README.md                 # Project documentation
