# Edge AI Visualizer

**Edge** is a browser-based tool for understanding how neural networks run on edge devices.  
It focuses on practical aspects of deployment — like inference time, memory usage, and model size — especially for smaller, resource-constrained hardware.

The goal is to make model execution more transparent, especially for students, embedded engineers, and ML developers who care about performance beyond just accuracy.

---

## Features

### Model Upload + Graph Viewer
- Upload ONNX or TensorFlow.js models
- See the model as a visual flow of layers
- Inspect shapes, parameter counts, and operations per layer

### Inference Time Simulation
- Choose from a set of preset edge devices (e.g. Pi 4, Jetson Nano, ESP32)
- Simulate how long each layer might take
- See peak memory usage and total latency

### Optimization Tools
- Try simulated **quantization** (e.g. FP32 → INT8)
- Explore effects of **pruning** low-importance weights
- Compare original vs optimized models side-by-side

### Device Profiles
- Built-in profiles with realistic constraints (memory, compute)
- Option to create your own

---

## Stack

- **Frontend**: React, Vite, Tailwind, D3.js or Three.js
- **Backend logic**: ONNX.js or TensorFlow.js, with some WebAssembly
- **Format support**: ONNX, TF.js
- **Hosting**: GitHub Pages or Vercel

---

## Roadmap (in progress)

- View basic activation maps for conv layers
- Add real inference for small models (using TF.js)
- Compare multiple models for the same task
- Simulate layer compilation for embedded targets

---

## Why This Exists

This project came out of wanting to better understand what happens between a trained model and it actually running on-device — especially on limited hardware.

Most tools focus on training or end deployment. This one sits in the middle: helping you analyze, optimize, and learn what's happening layer by layer.

---

## Local Setup

```bash
npm install
npm run dev



---

### ✅ Instructions to Use It:

1. Create the file:
```bash
code README.md
