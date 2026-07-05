# 🔬 Learning Computer Vision

A hands-on, from-scratch journey through Computer Vision using **PyTorch**. Every notebook in this repo was written independently as part of a self-directed learning path — no copy-pasting solutions, just building intuition one layer at a time.

---

## 🧭 What This Repo Is

This is a progressive curriculum that starts with "what is a pixel?" and builds up to semantic segmentation with U-Net. Each chapter introduces one core concept, reinforces it with code, and leaves behind a working notebook you can re-run and extend.

The guiding principle: **understand it well enough to rebuild it from memory.**

---

## 📓 Chapters

| # | Notebook | Topic | Key Concepts |
|---|----------|-------|--------------|
| **1** | `Ch1_What an image actually is.ipynb` | Image Fundamentals | PIL, NumPy arrays, PyTorch tensors, RGB channels, `uint8` vs `float32`, `ToTensor`, `transforms.Normalize` |
| **1P** | `Ch1_Practise.ipynb` | Hands-on Practice | Masks, batch dimensions, tensor manipulation drills |
| **2** | `Ch2_Convolutions.ipynb` | Convolution Operations | `Conv2d` mechanics, kernel weights, stride, feature maps |
| **3** | `Ch3_Stacking_Convolution.ipynb` | Encoder Architecture | Stacking conv stages, `MaxPool2d`, spatial-to-semantic compression (WHERE → WHAT) |
| **4** | `Ch4_CNN_Classifier.ipynb` | End-to-End CNN | Full MNIST classifier — training loop, loss, optimizer, evaluation |
| **6** | `Ch6_UNet.ipynb` | Semantic Segmentation | U-Net via `segmentation_models_pytorch`, ResNet34 backbone, mask prediction |
| **7** | `Ch7_DataLoader.ipynb` | Custom Data Loading | Building a `DataLoader` with `cv2`, BGR→RGB conversion, batch iteration |
| **7.1** | `Ch7.1_The_Dataset_Class.ipynb` | Custom Dataset | Implementing PyTorch's `Dataset` interface for real-world data |

### Supporting Notebooks

| Notebook | Purpose |
|----------|---------|
| `Python_class.ipynb` | Python OOP refresher — classes, `__init__`, `__len__`, `__getitem__` |
| `Revision.ipynb` | Spaced review — re-deriving key concepts from memory |
| `Practise.ipynb` | Miscellaneous coding drills and experiments |

---

## 🛠 Tech Stack

- **Python 3**
- **PyTorch** — `Conv2d`, `MaxPool2d`, `DataLoader`, `Dataset`, `nn.Module`
- **torchvision** — transforms, datasets
- **segmentation_models_pytorch** — pretrained U-Net architectures
- **OpenCV (cv2)** — image I/O, color space conversion
- **PIL / Pillow** — image loading and manipulation
- **NumPy** — array operations
- **Matplotlib** — visualization

---

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/AsimNayakawadi/Learning_Computer_Vision.git
cd Learning_Computer_Vision

# Install dependencies
pip install torch torchvision segmentation-models-pytorch opencv-python pillow numpy matplotlib

# Open any notebook
jupyter notebook
```

Start with **Ch1** and work forward — each chapter builds on the previous one.

---

## 🗺 Roadmap

- [x] Image fundamentals (pixels, tensors, normalization)
- [x] Convolution mechanics and pooling
- [x] Encoder architecture (stacking conv stages)
- [x] CNN classifier (MNIST end-to-end)
- [x] Semantic segmentation with U-Net
- [x] Custom DataLoader and Dataset
- [ ] Conv2d kernel visualization
- [ ] U-Net from-scratch implementation
- [ ] Transfer learning and fine-tuning
- [ ] Object detection
- [ ] Real-world project: Plant disease classifier
- [ ] Real-world project: Safety helmet detector

---

## 📐 Learning Approach

This repo follows a **build-to-understand** philosophy:

1. **Concept first** — intuitive explanation before any code
2. **Write it yourself** — every line written independently, then reviewed
3. **Break it on purpose** — deliberate experiments to test understanding
4. **Re-derive from memory** — spaced re-implementation at increasing intervals

No chapter is marked "done" until it can be rebuilt without reference material.

---

## 📄 License

This project is open for learning purposes. Feel free to use it as a reference for your own CV journey.

---

<p align="center">
  <i>Built one convolution at a time.</i>
</p>
