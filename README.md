# Plant Disease Classification Using Deep Learning 🍅 

This project utilizes **Convolutional Neural Networks (CNN)** to classify **tomato leaf diseases** using the **Plant Village dataset** from Kaggle. The dataset includes **6,227 images** across **four classes** of healthy and diseased tomato leaves.

## 📌 Problem Explanation

Leaf diseases are a **major concern** for farmers worldwide, leading to **significant yield losses** and **economic damage**. Developing a **Deep learning model** to classify these diseases can aid **early detection, disease monitoring, and management strategies** for better agricultural outcomes.

## 🌿 Dataset Overview  

The dataset contains **high-quality images of tomato leaves** with different disease conditions.  

📌 **Dataset Source:** [PlantVillage Dataset on Kaggle](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset)  

### **📊 Classes in the Dataset**  
The dataset consists of **four** classes:

| Class                      | Number of Images |
|----------------------------|-----------------|
| **Tomato Bacterial Spot**  | **2,127**       |
| **Tomato Early Blight**    | **1,000**       |
| **Tomato Healthy**         | **1,591**       |
| **Tomato Late Blight**     | **1,909**       |

Total dataset size: **6,627 images**  

## 🛠️ Data Preprocessing  

Data processing is **an essential step** before training any model. Since we are dealing with **images**, we applied the following preprocessing steps:

- **Rescaling**: Normalize pixel values (0-255) to a range of (0-1).
- **Data Augmentation**: Applied **horizontal flipping** to enhance dataset variability.
- **Resizing**: Adjust all images to a standard **size of 224x224**.

## 📑 Data Splitting  

The dataset was split as follows:

| **Dataset Partition** | **Percentage** |
|----------------------|--------------|
| **Training Set**     | **60%**       |
| **Validation Set**   | **20%**       |
| **Testing Set**      | **20%**       |

## 🧠 CNN Model Architecture  

The model consists of **multiple convolutional layers**, **max pooling layers**, and a **dropout layer** to reduce overfitting.

## 📈 Results  

| ** Metric** | **value ** |
|-------------|------------|
| **Test loss**  | **0.2112** |
| **Test Accuracy**  | **90.76%** |

## 📌 Conclusion
This deep learning model successfully classifies plant diseases with 90.76% accuracy using CNNs.
Further improvements can be made by increasing dataset diversity and using transfer learning models.


## 📂 Project Structure  
```plaintext
📦 Plant Disease Classification
│-- 📜 README.md                    - Project documentation
│-- 📜 CNN_Model.ipynb              - Jupyter Notebook with model training code
│-- 📂 dataset/                     - Contains images of plant leaves (Download from Kaggle)
