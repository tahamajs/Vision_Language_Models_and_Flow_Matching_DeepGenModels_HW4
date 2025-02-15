
# **Vision-Language Models and Flow Matching - Deep Generative Models HW4**

**University of Tehran** | **Department of Electrical and Computer Engineering**

 **Course** : Deep Generative Models |  **Instructor** : Dr. Mostafa Tavasoli |  **Term** : Fall 1403

 **Author** : *Taha Majlesi*

 **Email** : [taha.maj4@gmail.com](mailto:taha.maj4@gmail.com) | [tahamajlesi@ut.ac.ir](mailto:tahamajlesi@ut.ac.ir)

 **Profiles** : [LinkedIn](https://www.linkedin.com/in/tahamajlesi/) | [GitHub](https://github.com/tahamajs) | [Hugging Face](https://huggingface.co/tahamajs/plamma)

---

## **Table of Contents**

* [Introduction](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#introduction)
* [Course Information](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#course-information)
* [Assignment Details](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#assignment-details)
* [Sections Overview](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#sections-overview)
  * [Vision-Language Models (VLM)](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#vision-language-models-vlm)
  * [Flow Matching for Generative Modeling](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#flow-matching-for-generative-modeling)
* [Implementation Details](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#implementation-details)
* [Mathematical Derivations](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#mathematical-derivations)
* [Training and Experimentation](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#training-and-experimentation)
* [Results and Analysis](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#results-and-analysis)
* [Submission Guidelines](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#submission-guidelines)
* [License](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#license)
* [Project Structure](https://chatgpt.com/c/67b0eae8-c268-8007-9df3-33d28ab21913#project-structure)

---

## **Introduction**

This repository contains **Homework 4** for the **Deep Generative Models** course at the  **University of Tehran** . The assignment explores  **cutting-edge generative models** , focusing on:

* **Vision-Language Models (VLMs)** , particularly **PaliGemma**
* **Fine-tuning large-scale models for Image-Question Answering (IQA)**
* **Evaluating generative models using ROUGE Score**
* **Flow Matching for continuous-time generative modeling**
* **Optimal Transport in generative models**

This assignment provides **both theoretical and practical** components, allowing students to explore  **state-of-the-art generative techniques** .

---

## **Course Information**

* **University** : University of Tehran
* **Department** : Electrical and Computer Engineering
* **Course** : Deep Generative Models
* **Instructor** : Dr. Mostafa Tavasoli
* **Term** : Fall 1403

---

## **Assignment Details**

This homework consists of  **two major sections** :

### **1. Vision-Language Models (VLM)**

* Understanding multimodal learning (vision + language)
* Fine-tuning **PaliGemma** for **image-based question answering**
* Optimizing memory usage with **LoRA and QLoRA**
* Evaluating models using **ROUGE Score**

### **2. Flow Matching for Generative Modeling**

* Mathematical derivation of **Flow Matching**
* Understanding **Optimal Transport in Flow-Based Generative Models**
* Implementing **Continuous Normalizing Flows (CNFs) for data generation**

---

## **Sections Overview**

### **Vision-Language Models (VLM)**

VLMs integrate **image and text** to perform tasks such as  **image-based question answering, caption generation, and visual reasoning** .

#### **Tasks:**

1. **Understanding Vision-Language Models (VLMs)**
   * Explain how **PaliGemma** differs from standard text-based models.
   * Compare **PaliGemma, DALL·E, and Imagen** architectures.
2. **Fine-Tuning PaliGemma for Image-Question Answering**
   * Fine-tune **PaliGemma-3B** using the  **CLEVR dataset** .
   * Utilize **LoRA and QLoRA** for memory-efficient fine-tuning.
3. **Evaluating Performance using ROUGE Score**
   * Compute **ROUGE Score** for evaluating  **generated text responses** .
   * Compare model performance before and after fine-tuning.
4. **Memory Optimization in Fine-Tuning**
   * Compare **full fine-tuning vs. LoRA fine-tuning** in memory usage.
   * Explain the benefits of **Quantization (NF4 datatype)** in reducing model size.

---

### **Flow Matching for Generative Modeling**

Flow Matching models use **continuous-time transformations** to map a simple distribution (e.g., Gaussian noise) to a complex data distribution.

#### **Tasks:**

1. **Mathematical Analysis of Flow Matching**
   * Derive the  **Flow Matching equation** .
   * Explain why  **Flow Matching avoids iterative sampling** .
2. **Optimal Transport in Flow Matching**
   * Describe how **Optimal Transport** improves Flow Matching.
   * Compare  **Flow Matching to Diffusion Models** .
3. **Implementing Flow Matching Models**
   * Implement a  **Flow Matching generative model** .
   * Train the model using  **ODE-based continuous transformations** .

---

## **Implementation Details**

### **Dataset**

* **Vision-Language Models** : **CLEVR dataset** (for image-question answering).
* **Flow Matching Models** : **Synthetic data** with  **optimal transport properties** .

### **VLM Fine-Tuning**

| **Component**        | **Details** |
| -------------------------- | ----------------- |
| **Base Model**       | PaliGemma-3B      |
| **Optimizer**        | AdamW             |
| **Fine-Tuning**      | LoRA, QLoRA       |
| **ROUGE Evaluation** | Yes               |

### **Flow Matching Model Parameters**

| Parameter      | Value   |
| -------------- | ------- |
| Learning Rate  | 0.0002  |
| Batch Size     | 64      |
| Training Steps | 100,000 |

---

## **Mathematical Derivations**

1. **Flow Matching Equations**
   * Show how **Flow Matching avoids iterative sampling** in normalizing flows.
2. **Why Use Optimal Transport?**
   * Explain how **Optimal Transport** improves generative performance.
3. **Computing ROUGE Score**
   * ROUGE measures **text similarity** between generated responses and ground truth:
     ROUGE=overlapping wordstotal words in referenceROUGE = \frac{\text{overlapping words}}{\text{total words in reference}}

---

## **Training and Experimentation**

1. **Fine-tune PaliGemma** and evaluate performance on  **CLEVR dataset** .
2. **Compare LoRA vs. QLoRA** for efficient fine-tuning.
3. **Train a Flow Matching model** and evaluate generated samples.

---

## **License**

This project is licensed under the  **MIT License** .

For more details, see the [LICENSE](https://chatgpt.com/c/LICENSE) file.

---
