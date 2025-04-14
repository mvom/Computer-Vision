---

# Computer Vision

## INFO8010: Project Proposal  

---

## Section 1: Project Description

Crop diseases pose a major threat to food security, yet their rapid identification remains challenging in many regions due to limited infrastructure. The global proliferation of smartphones, combined with recent advancements in computer vision enabled by deep learning, opens up opportunities for smartphone-assisted diagnosis of crop diseases.

The aim of this project is to develop a deep neural network capable of analyzing images captured by smartphones to quickly and accurately identify crop diseases.

---

## Section 2: Data

We are working with a dataset of **54,306 images** of plant leaves, classified into **38 categories**, each representing a unique crop-disease pair. The objective is to predict the correct crop-disease label from the image of a plant leaf.

The dataset is publicly available here:  
🔗 [PlantVillage Deep Learning Dataset](https://github.com/digitalepidemiologylab/plantvillage_deeplearning_paper_dataset)

We utilize three different versions of the PlantVillage dataset in our experiments:

1. **Original (Color) Images**  
2. **Grayscale Images**  
3. **Segmented Leaf Images**

By comparing performance across these variants, we assess the robustness and generalization ability of our model in different visual conditions.

---

## Section 3: Computing Resources

To efficiently train our deep convolutional neural network on this large dataset, we require access to high-performance computing resources with **GPU capabilities**.

---

## Section 4: Neural Network Architecture

Our convolutional neural network (CNN) design is inspired by the **AlexNet** architecture introduced by Krizhevsky et al. in 2012, which has proven effective for image-based plant disease detection [1].

**AlexNet Overview:**
- **5 convolutional layers**
- **3 fully connected layers**
- **Max-pooling layers**
- **ReLU activation**
- **Dropout layers** (for regularization)
- **Batch normalization** (to accelerate training)

We will adapt this architecture to fit our specific task:
- Modifying the **output layer** to match our 38 crop-disease classes
- Fine-tuning **hyperparameters**
- Introducing potential **additional layers** to optimize performance

By leveraging and customizing AlexNet, we aim to create a robust and accurate model capable of real-time crop disease classification from smartphone-captured images.

---

### Reference

[1] Mohanty, S. P., Hughes, D. P., & Salathé, M. (2016).  
*Using deep learning for image-based plant disease detection*. Frontiers in Plant Science, 7, 215232.

---
