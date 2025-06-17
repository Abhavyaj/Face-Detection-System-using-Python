# 👁️ Face Detection System using Python & OpenCV

This Python script uses **OpenCV** to perform **real-time face detection** through your computer’s webcam using the **Haar Cascade Classifier**.

It captures live video feed, detects human faces frame-by-frame, and highlights them with bounding rectangles — all in real time.

---

## 📌 Features

- 🧠 Real-time face detection using Haar Cascade Classifier
- 🎥 Webcam integration via OpenCV
- 🖼️ Bounding boxes drawn around detected faces
- 🛑 Exit on single keypress (`a`)
- 🪶 Lightweight and easy to use

---

## 🛠️ Technologies Used

- Python 3.x
- [OpenCV](https://opencv.org/) (`cv2`)
- Haar Cascade Classifier (pre-trained XML file)

---

## 📁 Project Structure

```bash
face-detection-system/
│
├── face_detection.py         # Main Python script
├── haarcascade_frontalface_default.xml   # Haar cascade classifier (use local path)
└── README.md                 # Project documentation
```

---

## 🧾 Requirements
### Install the required package:

- pip install opencv-python

---

## 🚀 How to Run

### Download Haar Cascade Classifier
### Make sure you have the haarcascade_frontalface_default.xml file. It's usually located at:
- <your-python-install-path>/Lib/site-packages/cv2/data/haarcascade_frontalface_default.xml

###📌 NOTE: Update the path in the script to match your local system. Example:
- face_cascade = cv2.CascadeClassifier("C:/Users/HP/AppData/Local/Programs/Python/Python310/Lib/site-packages/cv2/data/haarcascade_frontalface_default.xml")

--- 

## Run the Script
- python Face_Detection_System.py
- Press a to Exit

--- 

## 🖥️ How it Works
- Captures video from your webcam.
- Converts each frame to grayscale.
- Uses detectMultiScale() to find faces.
- Draws rectangles around detected faces.
- Displays the real-time video feed with bounding boxes.

---

## 🧠 Haar Cascade Parameters Used

- faces = face_cascade.detectMultiScale(
    gray, 
    scaleFactor=1.1, 
    minNeighbors=5, 
    minSize=(30, 30)
)
- scaleFactor: Image size reduction scale (default = 1.1)
- minNeighbors: Neighboring rectangles needed to retain detection
- minSize: Minimum object size
- flags: Default behavior if not specified

---

# ⚠️ Note
## 🗂️ IMPORTANT: You must set the correct path to your Haar Cascade XML file in your code. If you’re using a virtual environment or different OS, this path will vary.

---

## 📄 License
This project is licensed under the MIT License. Feel free to use and modify it for personal or commercial use.

---

## 🤝 Contributing
Pull requests are welcome! For significant changes, please open an issue first.
