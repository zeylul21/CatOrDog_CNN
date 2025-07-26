# CatOrDog_CNN
🐱🐶 CNN-based image classifier that distinguishes between cat and dog images using TensorFlow.

This project is a Convolutional Neural Network (CNN)-based image classifier that distinguishes between cats and dogs. Built with TensorFlow/Keras, the model was trained on a dataset of 10,000 images and split into 80% training, 10% validation, and 10% testing.

---

## 📁 Project Structure

```
dataset/
├── train/
│   ├── cats/
│   └── dogs/
├── val/
│   ├── cats/
│   └── dogs/
└── test/
    ├── cats/
    └── dogs/
```

---

## ⚙️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab (optional)

---

## 🚀 How to Run

1. Install the required packages:

```bash
pip install -r requirements.txt
```

2. Place your `dataset.zip` file in the project directory and extract it:

```python
import zipfile
with zipfile.ZipFile("dataset.zip", 'r') as zip_ref:
    zip_ref.extractall()
```

3. Train the model (either in Jupyter Notebook or as a script):

```bash
python train.py
```

4. After training, a file named `cat_dog_cnn.h5` will be generated. Use it for predictions like this:

```python
model = tf.keras.models.load_model("cat_dog_cnn.h5")
predict_image("example.jpg", model)
```

---

## 📊 Results

The model achieved an accuracy of **%77** on the test set.  
(Replace with your actual test accuracy.)

---

## 📝 Notes

- **The dataset folder is not included in the repository** to keep the repo lightweight.
- The trained model file (`.h5`) is also excluded for size reasons.
- You can upload a sample image to test the model prediction function.

---

## 📌 License

MIT License.
