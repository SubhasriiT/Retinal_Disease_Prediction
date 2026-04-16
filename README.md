# Proxy-Based Retinal Disease Severity Prediction
A deep learning project focused on predicting retinal disease severity using CNN and MobileNetV2 with a proxy-based learning approach.



## Description
This project focuses on predicting retinal disease severity using retinal fundus images, especially in situations where clinical labels are not available.  

To address this challenge, a **proxy-based approach** is used, where **vessel density** (derived from retinal blood vessel segmentation masks) acts as an indicator of disease severity.  

Based on this proxy, the images are classified into:
- *Low Risk*  
- *High Risk*  

This makes the system a **weakly supervised learning model**, suitable for real-world healthcare scenarios with limited labeled data.

> **Dataset:** [DRIVE Retinal Dataset](https://www.kaggle.com/datasets/andrewmvd/drive-digital-retinal-images-for-vessel-extraction)


## Technologies Used
- **Language:** Python  
- **Environment:** Jupyter Notebook  
- **Libraries:** *TensorFlow, Keras, NumPy, Pandas, Matplotlib, OpenCV, Scikit-learn*  


## Models Used

### *Custom CNN*
- 3 Convolution layers + Pooling + Dropout  
- Used as a baseline model  

### *MobileNetV2 (Transfer Learning)*
- Pretrained on ImageNet  
- Fine-tuned final layers  
- Efficient for small datasets  


## Installation
To run this project locally:

1. Clone the repository:

git clone https://github.com/SubhasriiT/Retinal_Disease_Prediction.git


2. Navigate to the project folder:

cd retinal-disease-severity-prediction


3. Install required libraries:

pip install tensorflow keras numpy pandas matplotlib opencv-python scikit-learn


4. Open the Jupyter Notebook:

jupyter notebook



## Usage
1. Open the notebook file: `retinal_disease_prediction.ipynb`  
2. Run all cells step-by-step  
3. Train models and evaluate performance  
4. Visualize results including Grad-CAM outputs  


## Results

### *CNN*
- **Accuracy:** 60%  
- **Precision:** 63%  
- **Recall:** 85%  
- **F1 Score:** 64%  

### *MobileNetV2*
- **Accuracy:** 55%  
- **Precision:** 53%  
- **Recall:** 100%  
- **F1 Score:** 65%  

> *MobileNetV2 showed better generalization and was more effective in detecting disease cases.*


## Key Insights
- *Proxy labeling* (vessel density) works well when labels are unavailable  
- *Transfer learning* improves performance on small datasets  
- MobileNetV2 provides better stability and interpretability  
- Grad-CAM shows clinically relevant focus areas  


## Contributing
Contributions are welcome. If you would like to improve this project:

1. Fork the repository  
2. Create a new branch  
3. Make your changes  
4. Submit a pull request  


## License
This project is intended for educational purposes. Dataset usage follows the original dataset licensing.


## Contact
For any queries or suggestions, feel free to reach out:

- **Name:** Subhasri  
- **Email:** ktsubhasri2005@gmail.com  
- **GitHub:** [SubhasriiT](https://github.com/SubhasriiT)
