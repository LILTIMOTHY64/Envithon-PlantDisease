# 🌱 Envithon Plant Disease Detection

## 📌 Overview
Envithon Plant Disease Detection is a machine learning–powered project designed to **detect plant diseases from leaf images**. It combines a **deep learning model (YOLOv8 + TensorFlow/Keras)** with a simple **Flask-based web frontend** to provide real-time plant disease predictions.

---

## 📂 Project Structure
```
Envithon-PlantDisease-main/
│── yolov8n.pt                  # Pre-trained YOLOv8 model
│
├── Backend/
│   ├── Model/                  # Saved TensorFlow/Keras model
│   │   ├── fingerprint.pb
│   │   ├── keras_metadata.pb
│   │   ├── saved_model.pb
│   │   └── variables/
│   ├── Output/                 # Sample output predictions
│   └── Training Code/          # Jupyter notebook + training PDF
│
├── Frontend/
│   ├── app.py                   # Flask server
│   ├── connect.py               # Helper for model integration
│   ├── static/                  # CSS, JS, and images
│   └── templates/               # HTML templates
│
└── README.md
```

---

## 🚀 Features
- Upload an image of a plant leaf through the web app.  
- Model predicts if the plant is **healthy** or **diseased**.  
- Uses **YOLOv8 for object detection** and a **CNN (Keras/TensorFlow)** for classification.  
- Frontend built with **Flask, HTML, CSS, and JavaScript**.  

---

## ⚙️ Installation & Setup
1. Clone the repository or extract the zip:
   ```bash
   git clone https://github.com/LILTIMOTHY64/Envithon-PlantDisease.git
   cd Envithon-PlantDisease-main
   ```

2. Create a virtual environment & install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate   # (Linux/Mac)
   venv\Scripts\activate      # (Windows)

   pip install -r requirements.txt
   ```

   > If `requirements.txt` is missing, manually install:
   ```bash
   pip install flask tensorflow torch ultralytics opencv-python numpy
   ```

3. Run the Flask app:
   ```bash
   cd Frontend
   python app.py
   ```

4. Open your browser at:
   ```
   http://127.0.0.1:5000/
   ```

---

## 📊 Training
Training code and explanation are available in:
- `Backend/Training Code/Plant_Disease_Training.ipynb`  
- `Backend/Training Code/Plant_Disease_Model_Building.pdf`  

---

## 📸 Sample Output
Sample prediction images are available in:
```
Backend/Output/
```

---

## 🛠 Tech Stack
- **Backend:** TensorFlow, Keras, PyTorch (YOLOv8), OpenCV  
- **Frontend:** Flask, HTML, CSS, JavaScript  
- **Language:** Python 3.x  

---

## 🙌 Contributors
This project was developed for **Envithon** as a demonstration of how **AI can help farmers identify plant diseases** efficiently.
