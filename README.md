
# 🤚 Hand Gesture-Based Volume Control using Python 

This project implements a **gesture-controlled volume system** using hand landmark detection. It leverages the **MediaPipe** framework and **OpenCV** for real-time hand tracking, and **PyAutoGUI** to simulate system volume control based on intuitive gestures like raising or lowering the index finger.

<hr>

## 📌 Abstract

The goal of this project is to implement a system that uses human hand gestures to control the computer's volume. By tracking hand landmarks captured through a webcam and recognizing specific gesture patterns, it enables volume adjustment without relying on physical input devices like buttons or keyboards. Real-time detection is achieved using the **MediaPipe** and **OpenCV** libraries in Python, while **PyAutoGUI** simulates the corresponding key presses (`volumeup`, `volumedown`). This interface enhances accessibility and offers a modern, touchless way to interact with digital devices.

---



## 🚀 Features

- Real-time hand tracking and gesture detection
- Volume up/down based on index finger and thumb position
- No keyboard or physical input required
- User-friendly and accessible design
- Easily extendable for other applications (media control, smart devices, etc.)

---

## 🧠 How It Works

### Algorithm Steps

1. Capture real-time video using webcam.
2. Use MediaPipe to detect hand landmarks.
3. Identify position of `INDEX_FINGER_TIP` and `THUMB_TIP`.
4. If:
   - ✋ Index higher than thumb → Volume Up 🔊
   - 🤚 Index lower than thumb → Volume Down 🔉
5. Simulate key press using `pyautogui`.
6. Display the annotated frame on screen.
7. Press `q` to quit program.

---

## 🧾 Project Structure

