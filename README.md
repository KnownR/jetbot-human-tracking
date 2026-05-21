# 🤖 JetBot Human Tracking System

Real-time autonomous human tracking and following robot built using NVIDIA Jetson Nano, PyTorch, OpenCV, and SSDLite MobileNetV3.

---

## 🚀 Features

- Real-time human detection
- Autonomous human following
- GPU-accelerated inference using CUDA
- Low-latency MJPEG live stream
- Optimized for Jetson Nano
- OpenCV + GStreamer camera pipeline
- Smooth tracking using EMA filtering

---

## 🧠 Model Used

### SSDLite320 MobileNetV3 Large

The project uses:

```python
torchvision.models.detection.ssdlite320_mobilenet_v3_large(pretrained=True)
```

Why this model?

- Lightweight and fast
- Optimized for edge devices
- Good balance between speed and accuracy
- Works efficiently on Jetson Nano

---

## 🛠️ Tech Stack

- Python
- PyTorch
- TorchVision
- OpenCV
- NVIDIA Jetson Nano
- CUDA
- GStreamer
- JetBot SDK

---

## 📷 System Architecture

Camera → OpenCV → MobileNetV3 Detection → Tracking Logic → Robot Movement

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/jetbot-human-tracking.git
cd jetbot-human-tracking
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the notebook:

```bash
jupyter notebook
```

Open:

```text
KIRTAN.ipynb
```

---

## 📡 Live Stream

The MJPEG stream runs on:

```text
http://<jetson-ip>:8080
```

---

## 🎯 Tracking Logic

The robot:

- Detects humans using COCO class labels
- Calculates target center position
- Applies smoothing using EMA
- Rotates left/right based on position error
- Moves forward when aligned

---

## 📂 Project Structure

```text
.
├── KIRTAN.ipynb
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
└── assets/
```

---

## 📈 Future Improvements

- TensorRT optimization
- DeepSORT tracking
- Multi-object tracking
- Face recognition support
- Web dashboard
- ROS2 integration

---

## 🖥️ Hardware Used

- NVIDIA Jetson Nano
- JetBot
- CSI Camera

---

## 📄 License

MIT License

---

## 🙌 Acknowledgements

- NVIDIA Jetson
- PyTorch
- TorchVision
- OpenCV
- JetBot Project
