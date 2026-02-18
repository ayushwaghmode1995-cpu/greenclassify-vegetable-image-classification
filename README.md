# Greenclassify: Deep Learning-Based Vegetable Image Classification

Greenclassify is a robust machine learning project designed to identify various types of vegetables from images with high accuracy. It leverages state-of-the-art Deep Learning architectures like **Xception** and **ResNet50**, integrated within a **Flask** web application for real-time classification.

## 🚀 Features

- **High Accuracy Classification**: Uses transfer learning with Xception and ResNet50 models.
- **Web Interface**: A clean and intuitive Flask-based web dashboard for uploading and classifying vegetable images.
- **Dataset Analysis**: Integrated scripts to visualize dataset distribution and class counts.
- **Flexible Backend**: Configured to use **Keras 3** with a **PyTorch** backend.
- **Pre-trained Support**: Ready to load and use pre-trained `.keras` or `.h5` models.

## 🛠️ Tech Stack

- **Core**: Python
- **Deep Learning**: Keras 3 (Backend: PyTorch), Torchvision
- **Web Framework**: Flask, Jinja2
- **Image Processing**: OpenCV, PIL (Pillow)
- **Data Analysis**: Matplotlib, NumPy, Pandas

## 📂 Project Structure

```text
Veg-class/
├── app.py                  # Flask web application entry point
├── train_resnet_keras.py   # Script for ResNet50 transfer learning
├── analyze_dataset.py      # Tool for analyzing dataset distribution
├── preprocess_data.py      # Data preprocessing utilities
├── dataset/                # Train/Validation image data
├── static/                 # Web assets (CSS, JS)
├── templates/              # HTML templates (index, prediction)
├── uploads/                # Temporary storage for uploaded images
├── requirements.txt        # Project dependencies
└── class_names.json        # List of supported vegetable classes
```

## 🥦 Supported Classes

The system is trained to recognize 15 different vegetables:
- Bean, Bitter Gourd, Bottle Gourd, Brinjal, Broccoli, Cabbage, Capsicum, Carrot, Cauliflower, Cucumber, Papaya, Potato, Pumpkin, Radish, Tomato.

## ⚙️ Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ayushwaghmode1995-cpu/greenclassify-vegetable-image-classification.git
   cd Veg-class
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Ensure Keras Backend is set (Optional but recommended):**
   The project is pre-configured to use PyTorch. You can verify this by checking the `KERAS_BACKEND` environment variable.

## 🖥️ Usage

### 1. Running the Web App
Start the Flask server:
```bash
python app.py
```
Open your browser and navigate to `http://127.0.0.1:5000`.

### 2. Training the Model
To train a ResNet50 model on your dataset:
```bash
python train_resnet_keras.py
```

### 3. Analyzing the Dataset
To generate a distribution chart of your classes:
```bash
python analyze_dataset.py
```

## 📊 Evaluation
The latest model (Xception v4) achieved a validation accuracy of **99.8%**, demonstrating the efficacy of the transfer learning approach.

---
Developed by **Ayush Waghmode**.
