# Sem5_Computer_Vision_Project

**Real-Time Object Detection & Analysis Using PyTorch**

This repository contains multiple Jupyter notebooks designed for real-time object detection, model creation, and experimentation using PyTorch. The primary objective is to analyze input from a webcam, detect objects in real-time, and optimize model performance for quick, repeatable inference without needing to reprocess every time.

📁 Repository Structure
.
├── output1.ipynb                        # Initial object detection and model creation
├── output2.ipynb                        # Enhanced version with live webcam analysis
├── output2_additional.ipynb            # Experimenting with training improvements
├── output2_different_approach.ipynb    # Alternate architecture/technique approach

🚀 Features

- Real-time object detection using PyTorch 
- Automatic model saving to .pt for reusability
- Optimized to prevent re-running heavy training multiple times
- Live webcam window with prediction overlay
- Multiple training strategies and architectural variants explored

🛠️ Installation

Clone this repository:
```bash
git clone https://github.com/yourusername/realtime-object-detection.git
cd realtime-object-detection
```
Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```
Install the required dependencies:
```bash
pip install -r requirements.txt
```
If requirements.txt is not present, install manually:
```bash
pip install torch torchvision opencv-python matplotlib numpy
```
📷 How to Run
Each notebook provides a different take or refinement. The most recommended one for full demo:
Launch Jupyter:
```bash
jupyter notebook
```

Open output2.ipynb.
- Run all cells:
- A window should appear using your webcam.
- Objects will be detected in real-time.
- Model will be saved as a .pt file to avoid retraining in future runs.

📓 Notebook Overview
Notebook	Description
- output1.ipynb	Baseline version for real-time detection and model saving.
- output2.ipynb	Final refined version with interactive webcam and persistent .pt model.
- output2_additional.ipynb	Added improvements in training process and accuracy analysis.
- output2_different_approach.ipynb	A variant approach using a different model or training pipeline.

✅ Output
- Saved model as .pt file
- Detected objects shown in webcam window
- Live confidence and label annotations
- Optionally logs training progress and results

📌 Notes
- Make sure your webcam is connected and not in use by another app.
- If cv2.VideoCapture() fails, try changing the index (e.g., cv2.VideoCapture(1)).
- Some notebooks skip training if .pt model exists — delete it to retrain.

📝 License

This project is open-source and available under the MIT License.
