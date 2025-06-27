# Sign Language Gesture Recognition with Mediapipe and Deep Learning

This project focuses on recognizing sign language gestures using hand landmarks extracted via [MediaPipe](https://google.github.io/mediapipe/) and a deep learning model built with TensorFlow/Keras.

## 🧠 Model Overview

The model uses 21 hand landmarks (x, y, z) as features to classify gestures into 37 categories (0–9, A–Z, and _). A dense neural network is trained on these landmarks to achieve high classification performance.

### 🔍 Performance

- **Accuracy**: `0.9888`
- **Loss**: `0.0521`

## 📁 Dataset

Dataset used: [Sign Language Gesture Images](https://www.kaggle.com/datasets/ahmedkhanak1995/sign-language-gesture-images-dataset)

Download it automatically using KaggleHub:
```python
import kagglehub
path = kagglehub.dataset_download("ahmedkhanak1995/sign-language-gesture-images-dataset")
```

## 🛠️ Dependencies

Install required packages with:

```bash
pip install -r requirements.txt
```

### Main Libraries:
- `TensorFlow`
- `OpenCV`
- `MediaPipe`
- `NumPy`
- `Matplotlib`
- `scikit-learn`

## 🏗️ Project Structure

- `sign_language_gesture_images.py`: Main training and evaluation script.
- `dataset/`: Path to download or place the dataset.
- `images/`: Optional folder for visualizations or hand landmark examples.

## 📸 Example Output

Sample input and extracted hand landmarks:

![original](images/original_image.jpg)
![landmarks](images/landmark_visualization.jpg)

## 🔮 Future Improvements

- Use temporal information (video frames) for dynamic gesture recognition.
- Integrate the model into a real-time sign language interpreter.
- Expand the dataset with more variations and users.

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

## 📄 License

[MIT](LICENSE)
