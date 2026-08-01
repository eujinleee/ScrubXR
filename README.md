# ScrubXR

**Winner of the Most Impactful Project Award**
**2026 Cornell Health AI Hackathon**

ScrubXR is an augmented reality system that automatically detects, counts, and tracks surgical instruments in real time using computer vision. Built with Unity, YOLOv11, and Meta Quest Pro, the system helps reduce manual surgical counts, improve operating room efficiency, and prevent retained surgical items.

---

## Overview

Manual surgical instrument counting is still performed multiple times during every operation and remains susceptible to human error. ScrubXR leverages augmented reality and computer vision to automatically detect and count surgical instruments, providing real-time tracking through an XR headset.

---

## Presentation

📄 **Project Presentation:** [ScrubXR.pdf](ScrubXR.pdf)

> Includes the project motivation, technical approach, architecture, business case, and live demonstration presented at the 2026 Cornell Health AI Hackathon.

---

## My Contributions

Responsible for the Unity application, including:

- Designed and developed the AR interface
- Integrated YOLO object detection into Unity
- Built the real-time surgical instrument counting system
- Developed the live visualization and tracking interface
- Connected the computer vision pipeline with the Meta Quest Pro experience

---

## Team

- Eujin Lee
- Sally Scofield
- Molly Matri
- Rahul Ramarao
- Pradhi Pakkerakari

---

## Features

- 🥽 Real-time AR interface using Meta Quest Pro
- 🔍 YOLOv11-based surgical instrument detection
- 🔢 Automatic surgical instrument counting
- ⚡ Live tracking during procedures
- 📊 Automatic logging of detected instruments

---

## Tech Stack

- Unity
- C#
- Python
- YOLOv11
- Meta Quest Pro

---

## Surgical Instruments

| Instrument | Training Images |
|------------|----------------:|
| Scalpel | 550 |
| Straight Dissection Clamp | 460 |
| Straight Mayo Scissor | 450 |
| Curved Mayo Scissor | 550 |

---

## Installation

```bash
pip install -r requirements.txt
```

---

## Training

```bash
python setup_dataset.py
python train.py
```

Best weights are saved to:

```text
runs/detect/scrubtech_v1/weights/best.pt
```

---

## Inference

```bash
python count_instruments.py --source data/
```

Additional options are documented in `count_instruments.py`.

---

## Repository Structure

```text
ScrubXR/
├── data/
├── Labels/
├── dataset/
├── runs/
├── dataset.yaml
├── setup_dataset.py
├── train.py
├── count_instruments.py
└── requirements.txt
```
