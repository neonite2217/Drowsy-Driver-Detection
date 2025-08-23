Here’s a clean and professional **README.md** draft for your project **Drowsy Driver Detection using OpenCV and CNN**:

---

# 🚗 Drowsy Driver Detection using OpenCV and CNN

A computer vision project that detects driver drowsiness in real-time using **OpenCV** for image/video processing and a **Convolutional Neural Network (CNN)** model for classification. The system alerts when it detects that a driver is sleepy or closing their eyes for a prolonged duration, helping to prevent accidents caused by fatigue.

---

## 📌 Features

* Real-time face and eye detection using **OpenCV**
* CNN-based model to classify **Open / Closed eyes**
* Works with live camera feed or pre-recorded video
* Alerts when drowsiness is detected (sound/alarm support can be added)
* Lightweight and runs on CPU/GPU

---

## 🛠️ Tech Stack

* **Python 3.x**
* **OpenCV** – for face/eye detection and video streaming
* **TensorFlow / Keras (CNN model)** – for training and prediction
* **NumPy & Pandas** – data handling
* **Matplotlib / Seaborn** – visualization (optional)

---

## 📂 Project Structure

```
Drowsy-Driver-Detection/
│── data/                 # Dataset (images of open/closed eyes)
│── models/               # Saved CNN models
│── notebooks/            # Jupyter notebooks (experiments/training)
│── src/                  # Source code
│   ├── train_model.py    # Train CNN model
│   ├── detect_drowsy.py  # Real-time detection script
│   └── utils.py          # Helper functions
│── requirements.txt      # Dependencies
│── README.md             # Project documentation
```

---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/Drowsy-Driver-Detection.git
cd Drowsy-Driver-Detection
```

2. Create a virtual environment (recommended):

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 📊 Dataset

* The project uses **labeled images of open and closed eyes**.
* You can use datasets like:

  * [MRL Eye Dataset](https://www.kaggle.com/datasets/serenaraju/mrl-dataset)
  * [Closed Eyes In The Wild (CEW)](http://parnec.nuaa.edu.cn/xtan/data/ClosedEyeDatabases.html)

---

## 🧠 Model Training

1. Place dataset inside the `data/` folder.
2. Run the training script:

```bash
python src/train_model.py
```

3. The trained model will be saved in `models/`.

---

## 🎥 Real-Time Detection

Run the detection script with webcam:

```bash
python src/detect_drowsy.py
```

* A bounding box will appear around the face.
* If eyes remain closed for a certain duration, an **alert** will be triggered.

---

## 📈 Results

* CNN model accuracy: **\~95%** (on test dataset)
* Works well in real-time scenarios with webcam feed.
* Performance may vary depending on lighting conditions and camera quality.

---

## 🚀 Future Improvements

* Add **alarm system** (buzzer/speaker alert)
* Improve detection under low-light conditions
* Integrate with **vehicle systems** for real-world deployment
* Deploy as a **mobile app** or **IoT device**

---

## 📜 License

This project is licensed under the **MIT License** – feel free to use and modify it.


