# 🚀 FNO & PINO Implementation

This repository contains implementations of **Fourier Neural Operator (FNO)** and **Physics-Informed Neural Operator (PINO)** models for learning and simulating physical systems.

---

## 📌 Overview

Neural Operators are a powerful class of models designed to learn mappings between function spaces. This project focuses on:

* **FNO (Fourier Neural Operator)** → Data-driven learning of PDE solutions
* **PINO (Physics-Informed Neural Operator)** → Combines data + physical constraints (PDE loss)

The goal is to efficiently approximate complex physical phenomena such as wave propagation, fluid dynamics, or MHD systems.

---

## ⚙️ Features

* ✅ Implementation of FNO architecture
* ✅ PINO with physics-based loss functions
* ✅ Training and evaluation pipelines
* ✅ Support for `.npy` datasets
* ✅ Visualization and rollout plots
* ✅ Modular and extendable codebase

---

## 📂 Project Structure

## 📂 Project Structure

```
FNO_PINO/
│
├── inference_FNO/          # FNO inference scripts and outputs
├── inference_PINO/         # PINO inference scripts and outputs
├── inference_comparison/   # Comparison between FNO and PINO
│
├── models/                 # Model architectures (FNO, PINO)
│
├── data_old.py             # Data loading / preprocessing (legacy)
├── main4.ipynb             # ⭐ Main notebook (primary entry point)
├── run.py                  # Script version (optional execution)
│
└── README.md
```

---

## 🚀 How to Run

### Run main notebook (recommended)

```
jupyter notebook main4.ipynb
```


---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/walmartbatman4/FNO_PINO.git
cd FNO_PINO
```

---

### 2. Create virtual environment (recommended)

```bash
python -m venv env
source env/bin/activate      # Linux / Mac
env\Scripts\activate         # Windows
```

---

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

### 4. Run the project

```bash
python main4.ipynb
```

---

## 📊 Data

* Input and output data are stored in `.npy` format
* Ensure correct shapes before training (important for FNO/PINO)

---

## 🧠 Models

### 🔹 FNO

* Uses Fourier transforms for global convolution
* Efficient for learning spatial patterns

### 🔹 PINO

* Adds **physics-based loss (PDE constraints)**
* Improves generalization and physical consistency

---

## 📈 Results

* Model predictions vs ground truth
* Error analysis and rollout performance
* Energy and physical consistency plots

---

## ⚠️ Notes

* Large datasets (`.npy`, model weights) should NOT be pushed to GitHub
* Use `.gitignore` for:

  ```
  *.npy
  *.pt
  *.pth
  env/
  __pycache__/
  ```

---

## 🔧 Future Work

* Improve PINO loss formulation
* Add support for more PDE systems
* Optimize training performance (GPU / CUDA)
* Extend to 3D simulations

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a new branch
3. Make changes
4. Submit a pull request

---

---

## 💡 Acknowledgements

* Neural Operator research community
* Open-source scientific ML tools

---

## 👤 Author

**Alfien Jessurun P**
**Ulaganathan KB**

---

⭐ If you found this useful, consider starring the repo!
