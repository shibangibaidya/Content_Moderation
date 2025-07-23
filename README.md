# Content Violation Detection for Set-Top Systems

This repository presents a lightweight AI-based content moderation system designed for real-time violence detection in television broadcasts, specifically targeting embedded environments such as set-top boxes. This project was developed as part of a research internship at the **Department of Computer Science and Engineering, NIT Calicut**, under the mentorship of **Dr. Joe Cheri Ross**.

## 🧠 Project Objective

The goal of this system is to **protect children from exposure to violent video content** by detecting and flagging scenes containing violence in a scalable, low-resource setup. The model is optimized for deployment on consumer set-top boxes with minimal hardware capabilities.

## 🔍 Technical Overview

- **Model**: MobileViT (Vision Transformer for lightweight inference)
- **Task**: Binary classification – violent vs. non-violent content
- **Framework**: PyTorch
- **Deployment Target**: Embedded platforms (e.g. set-top boxes)

## 🧰 Environment Setup

This project was developed and tested entirely in a **Google Colab CPU-only environment**, ensuring accessibility without the need for GPU acceleration.  
All experiments, frame sampling evaluations, and inference runs were performed using standard CPU resources provided by Colab.

> Note: While performance may vary across hardware setups, the pipeline is optimized to run efficiently without GPUs.


## 🎯 Sampling Techniques

To optimize inference latency and maintain accuracy, several **frame sampling strategies** were explored:

- Every 10th frame from the video stream  
- Initial 1 frame  
- Initial 2 frames  
- Initial 3 frames  
- Initial 4 frames  
- Initial 5 frames  

Each strategy was evaluated to find the right balance between computational efficiency and predictive performance.


## 🚀 Highlights

- Real-time content moderation for embedded systems
- Efficient frame sampling to reduce processing overhead
- Vision Transformer backbone optimized for speed
- Deployable solution for protecting young viewers from harmful content

