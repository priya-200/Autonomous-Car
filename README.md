# 🚗 Autonomous Driving Model using Unity Simulation 🎮🤖

Welcome to my Autonomous Driving project where a car learns to drive **by itself** using a model trained on **simulation data collected from Unity**!

This project blends the power of **machine learning**, **computer vision**, and **simulated environments** to build a self-driving car that can steer based on visual input.

---

## 📌 Project Overview

This project simulates a self-driving vehicle in a Unity environment, collects driving data, trains a deep learning model (CNN), and deploys it back in the simulation to autonomously control the car.

---

## 📷 Data Collection using Unity

Data was generated using a custom environment built in **Unity 3D**:

- 🖼️ Front-facing camera images (frames from simulation)
- 🔁 Steering angles
- ⛽ Throttle and brake values

Unity's scripting API was used to export this data in real-time during manual driving sessions.

---

## 🧠 Model Architecture

The model is a **Convolutional Neural Network (CNN)** that takes image frames as input and predicts the steering angle.

### 🔧 Model Highlights:
- Input shape: 66x200x3 (resized image)
- Convolutional layers for feature extraction
- Dense layers for regression output (steering angle)
- Trained using MSE (Mean Squared Error) loss

### 🏁 Training
- Framework: TensorFlow/Keras
- Loss Function: Mean Squared Error (MSE)
- Optimizer: Adam
- Epochs: 10 (I dont have GPU)

## Augmentations: Random brightness, flipping, cropping

Data was split into training and validation sets to monitor generalization.

## 🚘 Deployment in Unity
After training, the model was integrated back into Unity using a Python socket interface or TensorFlow model serving to control the car in real time.

The result? The car could:

 - Stay in lanes
 - Handle curves
 - Make basic turns

## 🎯 Key Learnings
 - Vision-based end-to-end control

 - Unity ML data pipeline

 - Model deployment in simulation

 - Real-time inference handling

## 🔍 To Do / Future Improvements
 - Add object detection (pedestrians, traffic signs)

 - Implement Reinforcement Learning for policy improvement

 - Sim2Real transfer learning for real-world testing

 - Model generalization to complex tracks
## 📌 Tech Stack
 - Unity 3D 🎮

 - Python 🐍

 - TensorFlow / Keras 🧠

 - OpenCV 📷

 - NumPy / Pandas 📊
 - Socket

