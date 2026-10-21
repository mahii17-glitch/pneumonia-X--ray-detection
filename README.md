 Pneumonia Detection from Chest X-Ray Images Using Deep Learning

Project Overview
This project explores binary classification of chest X-ray images into NORMAL and PNEUMONIA categories using deep learning and transfer learning.

The project was developed as a learning project to gain practical experience with medical image classification, TensorFlow, and model evaluation.

Objectives
- Build a chest X-ray image classification model.
- Apply transfer learning using MobileNetV2.
- Evaluate model performance using accuracy, loss, precision, recall, F1-score, and a confusion matrix.
- Experiment with data augmentation and compare model versions.

 Technologies Used
- Python
- TensorFlow / Keras
- MobileNetV2
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

 Dataset
  The project uses the publicly available Chest X-Ray Images (Pneumonia) dataset from Kaggle.
  Dataset: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia
  The dataset contains chest X-ray images organized into NORMAL and PNEUMONIA classes.

 Methodology
1. Loaded and prepared the chest X-ray image dataset.
2. Resized images to 224 × 224 pixels.
3. Used MobileNetV2 with ImageNet pretrained weights for transfer learning.
4. Added global average pooling, dropout, and a sigmoid classification layer.
5. Trained the baseline model and evaluated it on the test dataset.
6. Experimented with data augmentation in a second model.
7. Compared the models using classification reports and confusion matrices.

Results

 Model AND Test Accuracy 

 Version 1 — Baseline | 83.49% |
 Version 2 — Data augmentation experiment | 75.00% |

Version 2 did not outperform the baseline model on the test dataset. Its classification report also showed that it incorrectly classified many NORMAL images as PNEUMONIA.
These results demonstrate why evaluation on unseen test data and class-specific metrics are important.

 Key Learning Outcomes
- Practiced transfer learning with a pretrained convolutional neural network.
- Learned to prepare image datasets for binary classification.
- Used confusion matrices and classification metrics to analyze model errors.
- Compared two model experiments and documented the limitations of the results.

Limitations
- The validation split used in the experiments was very small and should be improved in future work.
- Performance differed between validation and test data.
- The models have not been clinically validated and must not be used for medical diagnosis.

 Future Improvements
- Create a larger, representative validation split.
- Investigate class-specific performance and generalization.
- Compare additional evaluation metrics and training strategies.
- Improve reproducibility and document the complete workflow.

 Disclaimer
This project is for educational purposes only. It is not a medical device and must not be used to diagnose or guide treatment of any medical condition.
