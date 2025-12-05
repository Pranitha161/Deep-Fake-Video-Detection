# Deep Fake Video Detection

## Problem Statement
With the rise of deep learning–based media generation, **deepfake videos** have emerged as a serious threat to digital authenticity and public trust. These synthetic manipulations can alter faces, voices, and expressions in highly realistic ways, making it difficult for the human eye to detect distortions.  
Such content poses risks across domains including:
- **Politics and journalism** → spreading misinformation and propaganda  
- **Cybersecurity and privacy** → identity misuse and fraud  
- **Social media** → erosion of trust in digital content  

Traditional detection methods (manual moderation, handcrafted features like blinking or head pose anomalies) are slow, error‑prone, and fail to generalize against modern GAN‑based deepfakes. There is a pressing need for an **automated, scalable, and accurate detection framework**.

---

## Our Approach
We designed a **deep learning–based pipeline** for detecting deepfakes at the frame level. The system leverages **Convolutional Neural Networks (CNNs)** to extract facial features from video frames and classify them as *real* or *fake*.  

### Key Steps
- **Frame Extraction**: Using OpenCV to parse video into individual frames.  
- **Preprocessing**: Resizing, normalization, and face detection to ensure consistent inputs.  
- **Feature Extraction**: Employing CNN architectures (e.g., Xception, InceptionV3) to capture subtle facial manipulations.  
- **Classification**: Training models to distinguish genuine vs. fake frames.  
- **Evaluation**: Measuring accuracy, precision, recall, and F1‑score for robust performance.  

### Highlights
- Modular pipeline → easy to extend with advanced models (GRUs, Transformers, 3D CNNs).  
- Baseline CNN achieves effective detection of frame‑level anomalies.  
- Future scope includes **temporal modeling**, **multimodal detection**, and **explainable AI** for improved trustworthiness.  

---

## Outcome
This project establishes a reproducible baseline for **real‑time deepfake detection**, contributing to the fight against misinformation and digital manipulation by harnessing AI for truth verification.
