# 🖱️ Virtual Mouse using Hand Gestures

A computer vision-based virtual mouse system built with Python that allows users to control the mouse cursor and perform click actions using only hand gestures — no hardware mouse required.

## 🚀 Demo

![Demo video][(link-to-my-demo-video)](https://drive.google.com/file/d/1uEJ1q1Demsetf0OBAUvx74XNE2DG7f1q/view?usp=sharing)

## 📌 Features

- 🖐️ Real-time hand tracking using **MediaPipe**
- 🎯 Move mouse cursor using your **index finger**
- 👆 Simulate **mouse clicks** when **thumb and index finger** touch
- 🔄 Mirror webcam view for natural interaction
- ⚡ Smooth performance across different screen resolutions

## 🧠 How It Works

- The webcam captures frames in real time.
- **MediaPipe Hands** identifies 21 hand landmarks.
- The **index finger tip (ID 8)** controls the cursor's x-y position on the screen.
- If the **index finger** and **thumb (ID 4)** come close (less than a threshold), a mouse click is triggered using `pyautogui`.

## 🛠️ Technologies Used

- Python 3.x
- OpenCV
- MediaPipe
- PyAutoGUI

