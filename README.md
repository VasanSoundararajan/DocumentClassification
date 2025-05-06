# Document Classification from Images using CNN

This project implements a Convolutional Neural Network (CNN) to classify different types of documents from their image representations using TensorFlow and Keras.

---

## 📁 Dataset Structure

Ensure your dataset follows this folder structure:

```

document-classification-dataset/
├── resume/
├── email/
└── scientific_publications/

````

Each subfolder should contain sample images of that document type.

---

## 🚀 Features

- Real-time document classification using image input
- CNN-based architecture built from scratch
- Automatic class balancing via `class_weight`
- Early stopping and best model checkpointing
- Inference support for single-image prediction

---

## 📊 Model Performance

- **Validation Loss:** `0.6031`
- **Validation Accuracy:** `72.73%`

> Trained over 25 epochs using a balanced dataset split (80% train / 20% validation).

---

## 🧪 Requirements

Install the dependencies:

```bash
pip install tensorflow numpy scikit-learn
````

---

## 🧠 Model Training

To train the CNN model, run:

```bash
python train_model.py
```

Ensure your dataset is correctly placed inside `document-classification-dataset/`.

---

## 📷 Inference

To classify a single image:

```python
from classify import classify_document

classify_document("path/to/image.jpg")
```

Output example:

```
Predicted Document Type: resume
Confidence: 92.45%
```

---

## 📂 Files

| File             | Description                                |
| ---------------- | ------------------------------------------ |
| `train_model.py` | Code to train the CNN model                |
| `classify.py`    | Contains `classify_document()` for testing |
| `best_model.h5`  | Saved best model (based on val\_accuracy)  |
| `README.md`      | Project overview and setup guide           |

---

## ✅ To-Do

* [ ] Improve results using pre-trained CNNs (e.g., MobileNetV2)
* [ ] Add batch prediction support
* [ ] Integrate drag-and-drop GUI with Tkinter

---

## 📜 License
[MIT License](LICENSE)

---
## Reference
Google COLAB
```
https://colab.research.google.com/drive/1AZJeOWgwWPn0nvrCrS8TDqxOc8wYH_4N?usp=sharing
```
---
## 🤝 Contributing

Pull requests, issues, and feature ideas are welcome!

```

Would you like this saved to a file or split into `train_model.py` and `classify.py` as suggested earlier?
```
