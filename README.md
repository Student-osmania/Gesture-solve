# ✋ GestureSolve: AI-Powered Gesture-Based Drawing and Math Solver

![Banner](D:\\projects\\Guestures calculator\\MathGestures.png)

**GestureSolve** is an interactive AI-powered web application that lets users draw using hand gestures captured via webcam and automatically interprets mathematical diagrams or equations using Google Gemini AI to solve them intelligently.

---

## 🚀 Features

- ✋ **Gesture-Based Drawing** using real-time hand tracking with OpenCV and cvzone
- 🧠 **AI-Powered Recognition** of hand-drawn figures, mathematical problems, and shapes
- 📐 **Smart Inference & Calculation**, like solving triangle side lengths or evaluating expressions
- 🖼️ Real-time webcam feed display with visual canvas overlay
- ⚡ Lightweight and fast using `Streamlit` and `Gemini 1.5 Flash`
- 🔁 Intuitive finger gestures for:
  - Drawing (`Index Finger`)
  - Clearing Canvas (`Thumb Up`)
  - Sending to AI (`Four Fingers Up`)

---

## 🛠️ Tech Stack

| Component       | Technology           |
|----------------|----------------------|
| Language        | Python               |
| GUI Framework   | Streamlit            |
| Hand Detection  | cvzone + OpenCV      |
| Image Handling  | PIL                  |
| AI Model        | Google Gemini 1.5    |
| Math Reasoning  | Gemini AI Inference  |
| Gesture Drawing | HandTrackingModule   |

---

## ✨ How It Works

1. **Hand Detection**: Uses `cvzone.HandTrackingModule` to detect hand landmarks.
2. **Gesture Control**:
   - Raise **only Index Finger** → Draw on the canvas.
   - Raise **only Thumb** → Clear the canvas.
   - Raise **4 Fingers** → Send canvas to Gemini AI for interpretation.
3. **AI Processing**: Sends the canvas as an image to Gemini with a prompt to analyze and solve the math-related content.
4. **Result Display**: The result is shown in real time beside the webcam feed.

---

## 🎮 Controls Summary

| Gesture             | Action                   |
|---------------------|--------------------------|
| ☝️ Index Finger Up    | Draw on canvas           |
| 👍 Thumb Up           | Clear canvas             |
| ✋ Four Fingers Up    | Send to AI for solving   |

---

## 📸 Sample Use Cases

- ✏️ Draw a **triangle** with two sides, and the AI calculates the missing side using geometry.
- ✏️ Sketch a **mathematical symbol** or **expression** like an integral or equation.
- ✏️ Sketch **simple shapes** (e.g., square, rectangle, circle) and the AI returns properties like area, perimeter, or side lengths.

---

## 📦 Installation & Setup

### 🔧 Prerequisites
- Python 3.8+
- Webcam
- Google Gemini API Key

### 📥 Install Dependencies
```bash
pip install opencv-python cvzone numpy streamlit google-generativeai Pillow
```
### 🔑 Configure Gemini API Key
```bash
genai.configure(api_key="YOUR_API_KEY_HERE")
```
### 📁 Project Structure 
GestureSolve/
│
├── MathGestures.png              # App banner/logo
├── your_script_name.py          # Main application script
└── README.md                    # Project overview and instructions

