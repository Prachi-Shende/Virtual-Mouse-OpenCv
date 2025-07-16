#  Virtual Mouse using OpenCV & MediaPipe

A Python-based virtual mouse system that uses hand gestures to control mouse movement and clicks using a webcam. Built with OpenCV, MediaPipe, and AutoPy.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-ComputerVision-success)
![MediaPipe](https://img.shields.io/badge/MediaPipe-HandTracking-blue)

---
Move your index finger to control the cursor. Pinch with index and middle finger to simulate a click.
---

##  Features

- Hand tracking using MediaPipe  
- Real-time cursor movement via finger tracking  
- Mouse clicking by measuring distance between fingers  
- Frame rate monitoring and UI overlay  
- Region-restricted mouse control for better accuracy

---

## Project Structure

AIVirtualMouse/  
├── HandTrackingModule.py — Hand detection and utility functions  
├── VirtualMouse.py — Main control logic using webcam  
├── requirements.txt — Project dependencies  
└── README.md — Project documentation  



---

##  Tech Stack

| Library     | Purpose                              |
|-------------|--------------------------------------|
| OpenCV      | Image processing & camera access     |
| MediaPipe   | Real-time hand tracking              |
| AutoPy      | Controlling mouse pointer/clicks     |
| NumPy       | Efficient numerical operations       |

---

##  Setup Instructions

1. **Clone the repository**  
   `git clone https://github.com/Prachi-Shende/Virtual-Mouse-OpenCv.git`  
   `cd Virtual-Mouse-OpenCv`

2. **Create and activate a virtual environment**  
   `python -m venv .venv`  
   `.\.venv\Scripts\activate`  *(Windows)*

3. **Install dependencies**  
   `pip install -r requirements.txt`

4. **Run the project**  
   `python VirtualMouse.py`

---

##  How It Works

- Uses MediaPipe to detect hand landmarks in real-time.  
- Tracks the tip of the index finger to move the mouse.  
- Detects pinch gesture (index + middle fingers) to simulate mouse clicks.  
- Uses `autopy` to control the actual OS mouse.

---

##  Security Note

Make sure to allow webcam access if you're running this on a secured system.

---

##  Credits

- [OpenCV](https://opencv.org/)  
- [MediaPipe](https://mediapipe.dev/)  
- [AutoPy](https://github.com/autopilot-rs/autopy)

---

##  Feedback

Feel free to raise issues or contribute to improve the project.
