
# ELBO-KL-VLM-FlowMatching-DGM-HW4

## 📌 Table of Contents

- [Introduction](#introduction)
- [Course Information](#course-information)
- [Assignment Details](#assignment-details)
- [Sections Overview](#sections-overview)
  - [Vision-Language Models (VLM)](#vision-language-models-vlm)
  - [Flow Matching for Generative Modeling](#flow-matching-for-generative-modeling)
- [Implementation Details](#implementation-details)
- [Mathematical Derivations](#mathematical-derivations)
- [Training and Experimentation](#training-and-experimentation)
- [Submission Guidelines](#submission-guidelines)
- [Academic Integrity Policy](#academic-integrity-policy)
- [License](#license)

---

## 📝 Introduction

This repository contains **Homework 4** for the **Deep Generative Models** course at the **University of Tehran**. The assignment covers **cutting-edge generative models**, including:

- **Vision-Language Models (VLM)** using **PaliGemma**
- **Fine-tuning Vision-Language Models** for **image-based question answering**
- **Evaluating generative text models using ROUGE Score**
- **Flow Matching for continuous generative modeling**
- **Optimal transport in flow-based models**

This assignment provides **both theoretical and practical** components, allowing students to explore **state-of-the-art generative models** and implement them efficiently in Python.

---

## 🎓 Course Information

- **University**: University of Tehran
- **Department**: Electrical and Computer Engineering
- **Course**: Deep Generative Models
- **Instructor**: Dr. Mostafa Tavasoli
- **Term**: Fall 1403

---

## 🏆 Assignment Details

This homework consists of **two major sections**:

### 🔹 **1. Vision-Language Models (VLM)**

- **Understanding Multimodal Learning** (Vision + Language)
- **Fine-tuning PaliGemma for Image-Question Answering**
- **Optimizing memory usage with PEFT (LoRA, QLoRA)**
- **Evaluating models using ROUGE Score**

### 🔹 **2. Flow Matching for Generative Modeling**

- **Mathematical derivation of Flow Matching**
- **Optimal Transport in Flow-based Generative Models**
- **Continuous Normalizing Flows for data generation**

---

## 📂 Sections Overview

### 🔥 **Vision-Language Models (VLM)**

Vision-Language Models (VLMs) combine image and text processing to perform tasks such as **image-based question answering, caption generation, and visual reasoning**.

#### ✅ **Tasks:**

1. **Understanding Vision-Language Models (VLM)**

   - Explain how **PaliGemma** differs from standard text-based models.
   - Compare **PaliGemma, DALL·E, and Imagen** architectures.
2. **Implementing PaliGemma for Image-Question Answering**

   - Fine-tune **PaliGemma-3B** using the **CLEVR dataset**.
   - Use **LoRA and QLoRA** for memory-efficient fine-tuning.
3. **Evaluating Performance using ROUGE Score**

   - Compute **ROUGE Score** for evaluating **generated text responses**.
   - Compare performance before and after fine-tuning.
4. **Memory Optimization in Fine-Tuning**

   - Compare **full fine-tuning vs. LoRA fine-tuning** in memory usage.
   - Explain the benefits of **Quantization (NF4 datatype)** in reducing model size.

---

### 🔥 **Flow Matching for Generative Modeling**

Flow Matching models use **continuous-time transformations** to map a simple distribution (e.g., Gaussian noise) to a complex data distribution.

#### ✅ **Tasks:**

1. **Mathematical Analysis of Flow Matching**

   - Derive the **Flow Matching equation**.
   - Explain why Flow Matching **avoids iterative sampling**.
2. **Optimal Transport in Flow Matching**

   - Describe how **Optimal Transport** improves Flow Matching.
   - Compare Flow Matching to **Diffusion Models**.
3. **Implementing Flow Matching Models**

   - Implement a **Flow Matching generative model**.
   - Train the model using **ODE-based continuous transformations**.

---

## ⚙️ Implementation Details

### **🔹 Dataset**

- For **Vision-Language Models**: **CLEVR dataset** (for image-question answering).
- For **Flow Matching Models**: Synthetic data with **optimal transport properties**.

### **🔹 VLM Fine-Tuning**

| **Component**        | **Details** |
| -------------------------- | ----------------- |
| **Base Model**       | PaliGemma-3B      |
| **Optimizer**        | AdamW             |
| **Fine-Tuning**      | LoRA, QLoRA       |
| **ROUGE Evaluation** | Yes               |

### **🔹 Flow Matching Model Parameters**

| Parameter      | Value   |
| -------------- | ------- |
| Learning Rate  | 0.0002  |
| Batch Size     | 64      |
| Training Steps | 100,000 |

---

## 📊 Mathematical Derivations

### **1️⃣ Flow Matching Equations**

- Show how **Flow Matching avoids iterative sampling** in normalizing flows.

### **2️⃣ Why Use Optimal Transport?**

- Explain how **Optimal Transport** improves generative performance.

### **3️⃣ Computing ROUGE Score**

- ROUGE measures **text similarity** between generated responses and ground truth:
  $$
  ROUGE = \frac{\text{overlapping words}}{\text{total words in reference}}
  $$

---

## 🚀 Training and Experimentation

1. **Fine-tune PaliGemma** and evaluate performance on **CLEVR dataset**.
2. **Compare LoRA vs. QLoRA** for efficient fine-tuning.
3. **Train a Flow Matching model** and evaluate generated samples.

---
# ELBO_KL_VLM_FlowMatching_DGM_HW4
