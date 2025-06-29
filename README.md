# -Emotion-Detection-Using-CNN-FER2013-

# Emotion Detection Using CNN (FER2013)

This project builds a Convolutional Neural Network (CNN) to detect **emotions from facial expressions** using the [FER2013 dataset](https://www.kaggle.com/datasets/msambare/fer2013). It classifies images into 7 emotion categories:

- Angry  
- Disgust  
- Fear  
- Happy  
- Sad  
- Surprise  
- Neutral

---

## 🔍 Dataset

- Dataset Name: FER-2013 (Facial Expression Recognition)
- Source: [Kaggle - FER2013](https://www.kaggle.com/datasets/msambare/fer2013)
- Format: 48x48 grayscale facial images stored in folders by emotion label (`train/` and `test/`)

---

## 🧠 Model Architecture

A basic CNN model built using TensorFlow/Keras:

- `Conv2D(32) + MaxPooling2D`
- `Conv2D(64) + MaxPooling2D`
- `Conv2D(128) + MaxPooling2D`
- `Flatten + Dense(128) + Dropout(0.5)`
- `Dense(7, softmax)`

---

## 🏋️ Training

- **Epochs**: 10  
- **Batch Size**: 64  
- **Optimizer**: Adam  
- **Loss Function**: Categorical Crossentropy  
- **Validation Accuracy**: ~59%

---

## 🔧 Dependencies

```bash
tensorflow
keras
numpy
pandas
matplotlib
````

All are available in Colab or can be installed via:

```bash
pip install tensorflow keras numpy pandas matplotlib
```

---

## 🚀 How to Run (Google Colab)

1. Clone or download this repository
2. Upload `kaggle.json` for dataset access *(optional if using Kaggle environment)*
3. Run the notebook: `emotion_detection_cnn.ipynb`

---

## 📈 Future Improvements

* Add data augmentation
* Use transfer learning (e.g., MobileNetV2 or ResNet50)
* Implement real-time emotion detection using OpenCV
* Improve accuracy with batch normalization

---

## 📸 Sample Output

| Input Image                   | Predicted Emotion |
| ----------------------------- | ----------------- |
| ![sample1](samples/happy.png) | Happy             |
| ![sample2](samples/sad.png)   | Sad               |

---

## 🙌 Author

Speranza Deejoe 

```
