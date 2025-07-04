# 🐶 Major Assignment 2: Dog Breed Identification

## 🔍 Problem
Classify dog breeds from images using CNNs.  
Dataset: [Kaggle - Dog Breed Identification](https://www.kaggle.com/competitions/dog-breed-identification)

---

## 📌 Model Architecture
- **Base Model:** EfficientNetB0 (pretrained on ImageNet)
- **Custom Layers:**
  - `GlobalAveragePooling2D`
  - `Dense(512, activation='relu')`
  - `Dropout(0.4)`
  - `Dropout(0.3)`
  - `Dense(num_classes, activation='softmax')`

---

## 🔁 Transfer Learning Strategy
- Used pre-trained **EfficientNetB0** for feature extraction
- Added a custom classification head on top
- **Frozen base layers** (can be fine-tuned later)
- Applied `preprocess_input` specific to EfficientNet for proper normalization

---

## 📈 Performance Metrics

| Metric              | Value                 |
|---------------------|-----------------------|
| **Validation Accuracy** | ~85% *(varies with seed)* |
| **Epochs**              | 5                    |
| **Optimizer**           | Adam                 |
| **Loss Function**       | Categorical Crossentropy |


