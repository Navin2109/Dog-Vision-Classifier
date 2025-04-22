
# 🐶 Dog Vision Classifier

A deep learning project that classifies images of dogs into 120 different breeds using **EfficientNetB0** and **transfer learning** via TensorFlow Hub. This project is built for the Kaggle Dog Breed Identification Challenge and demonstrates scalable image classification in real-world settings such as pet recognition systems, veterinary diagnostics, and shelter automation.

---

## 🚀 Project Highlights

- 📷 **Image Classification** using pre-trained EfficientNetB0 (TensorFlow Hub)
- 🔁 **Transfer Learning** to fine-tune on a 120-class dataset
- ⚙️ Optimized **tf.data pipeline** for large dataset handling
- 🎨 Applied **data augmentation** for better generalization
- 🧠 Fine-tuned **custom classification head**
- 🧾 Outputs prediction CSV in Kaggle submission format

---

## 📂 Dataset

- Source: [Kaggle - Dog Breed Identification](https://www.kaggle.com/competitions/dog-breed-identification)
- Training Images: 10,222
- Test Images: 10,357
- Number of Classes: 120 dog breeds
- Data Format: JPEG images with class labels in a CSV

---

## 🛠 Tech Stack

| Technology     | Usage                          |
|----------------|--------------------------------|
| Python         | Programming Language           |
| TensorFlow 2.x | Deep Learning Framework        |
| TensorFlow Hub | Transfer Learning (EfficientNetB0) |
| NumPy, Pandas  | Data Handling & Manipulation   |
| Matplotlib     | Visualization                  |
| Google Colab   | Training Environment (GPU)     |

---

## 🔧 Model Architecture

```python
EfficientNetB0 (Pre-trained, Frozen) +
GlobalAveragePooling2D +
Dropout +
Dense(120, activation='softmax')
```

- Loss Function: Categorical Crossentropy
- Optimizer: Adam
- Evaluation: Accuracy, CSV Predictions

---

## 🧪 Training Pipeline

1. Load & preprocess images using `tf.data`
2. Apply data augmentation (flip, zoom, rotate)
3. Train EfficientNetB0 with custom head
4. Generate predictions and format output
5. Evaluate using validation accuracy

---

## 📈 Results

- ✅ Achieved high validation accuracy
- ⚡️ Trained efficiently with minimal compute
- 🧠 Able to distinguish visually similar breeds
- 🐾 Scalable to other classification domains (wildlife, agriculture, etc.)

---

## 📁 Project Structure

```
dog-vision-classifier/
│
├── dataset/                  # Train & Test images
├── dog_vision.ipynb          # Main notebook (training + inference)
├── utils/                    # Helper scripts (preprocessing, plotting)
├── models/                   # Saved model checkpoints (optional)
├── predictions/              # Output CSV for Kaggle submission
└── README.md
```

---

## 📽 Demo

- 🔗 Notebook: [Google Colab](https://colab.research.google.com/drive/1Y4uLZtbjdo9LQsMd7xHgTxVw5_kkuOIx)
- 📊 Sample Output: CSV submission with prediction probabilities

---

## 📌 Future Improvements

- TensorFlow Lite conversion for mobile/edge deployment
- Real-time prediction via web camera or mobile app
- Model quantization for lightweight deployment

---

## 🤝 Contributing

Pull requests are welcome! If you’d like to add improvements or report bugs, please open an issue.

---

## 🙋‍♂️ Author

**Navin Sahu**  
💻 AI Enthusiast | Deep Learning Practitioner  
📧 Email: [navinsahu2109@gmail.com](mailto:navinsahu2109@gmail.com)  
🔗 LinkedIn: [linkedin.com/in/navin-sahu](https://www.linkedin.com/in/navin-sahu/)  

> Passionate about building AI tools that make a real-world impact.

---


## 🌍 Let AI Make a Pawsitive Impact!

```
🐾 From shelters to startups, intelligent dog breed detection is a step toward smarter, kinder technology.
```
