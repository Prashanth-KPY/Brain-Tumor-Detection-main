
# 🧠 Brain Tumor Detection and Classification

A full-stack deep learning project for detecting and classifying brain tumors from MRI scans using a pre-trained VGG16 model. Built with React.js, Flask/FastAPI, and deployed for public access. This system is designed to support faster and more accurate medical diagnoses.

---

## 🚀 Demo

🔗 [Live App](https://brain-tumor.netlify.app/)

![Screenshot 1](./Readme_resource/Image1.png)  
![Screenshot 2](./Readme_resource/Image2.png)  

🎥 [Demo Video](https://user-images.githubusercontent.com/64485885/228761355-885f5953-c953-4ae4-bbae-b3f1171f2801.mp4)

---

## 🛠️ Getting Started

### 1. Set up the environment
```bash
conda create -p venv python==3.10.6 -y
conda activate venv/
```
### 2. Install dependencies
```bash
pip install -r requirements.txt
```
### 3. Start the backend server
```bash
gunicorn app:app
```
### 4. Launch the frontend
```bash
cd client
npm install
npm start
```
You're good to go!

## 📌 Project Overview
Brain tumor detection is a critical challenge in medical imaging. This project aims to build an automated system that accurately classifies MRI scans as tumor or non-tumor using deep learning. The model is trained on a dataset of brain scans, enhanced through data augmentation to improve robustness and generalization.

The system includes:

A VGG16-based classifier trained on augmented MRI data

A REST API for real-time predictions

A React.js frontend for image upload and result display

Deployment via Netlify and Gunicorn

## 🧠 Machine Learning Model
Architecture: VGG16 (pre-trained)

Techniques: Data augmentation (rotation, flipping, scaling)

Training: Backpropagation with dropout and regularization

Accuracy: 99% on test set

Model saved using: pickle

The model was trained to classify brain scans as either tumor or non-tumor. Augmentation helped increase dataset diversity and improve model performance. The final model was serialized for deployment and integrated into the backend.

## 🔍 VGG16 Architecture Summary
Input: MRI image (3D pixel array)

Convolutional Layers: Extract features using filters

Pooling Layers: Reduce spatial dimensions

Flattening: Convert features to 1D vector

Fully Connected Layers: Classify image using softmax

Output: Probability scores for each class

## 🔗 Backend API (Flask + FastAPI)
Accepts image input and returns tumor prediction

Uses PIL for image preprocessing

Deployed with Gunicorn for concurrency

Returns JSON response with prediction and confidence

Easily deployable to cloud platforms like AWS or GCP

## 🎨 Frontend (React.js)
Upload MRI images via a clean UI

Displays prediction and confidence score

Shows loading spinner during processing

Responsive and user-friendly design

Styled with CSS for visual clarity

### 💡 Impact
This project demonstrates how deep learning can be applied to healthcare to improve diagnostic workflows. By combining VGG16 architecture with full-stack deployment, the system offers both technical depth and practical usability. It’s designed to be accessible to healthcare professionals and patients alike.

---
## 📫 Contact
For questions, feedback, or collaboration, feel free to reach out via  [LinkedIn](https://www.linkedin.com/in/prashanth-kpy/)  or open an issue on this repo.

---
