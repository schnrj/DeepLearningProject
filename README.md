# Fourier Neural Operator

In this project, we introduce a powerful new class of neural networks — the **Fourier Neural Operator (FNO)** — designed to efficiently learn operators arising from partial differential equations (PDEs).

By parameterizing the integral kernel **directly in Fourier space**, we develop an expressive and scalable architecture that outperforms existing methods in both **accuracy** and **speed**.

Our model has been extensively tested on:
- **Burgers' Equation**
- **Darcy Flow**
- **Navier-Stokes Equation** (including turbulent regimes)

---

## 🚀 Highlights

- **Efficient Kernel Learning**: Directly learning in Fourier space drastically reduces computational complexity.
- **Fast and Scalable**: Achieves up to **three orders of magnitude faster** inference compared to traditional PDE solvers.
- **State-of-the-art Performance**: Outperforms existing neural network-based methods on a wide range of benchmarks.
- **Simple and Modular Code**: All scripts are standalone, clean, and easy to adapt for different applications.

---

## 📚 Requirements

- [PyTorch](https://pytorch.org/)

Install the required library using:

```bash
pip install torch
```

---

## 📁 Project Structure

Each script in this repository is **independent** and **directly runnable**.

- `main.py` — Training loop and evaluation scripts.
- `utilities.py` — Dataset generation, loading, and preprocessing utilities.
- `models/` — Model architecture files.
- `data/` — Datasets for different PDE problems.

---

## 📦 Datasets

We provide datasets for the Burgers equation and Darcy flow.  
Data generation scripts are available in `utilities.py`.

- [PDE Datasets](https://drive.google.com/file/d/1uwMjkt1ANeHfqDhuOHZxeYaHpGmSwSUP/view?usp=sharing)

Download and place them inside the `data/` directory.

---

## 🧠 Pretrained Models

Evaluate the pre-trained models easily using the provided scripts like `_eval.py` or `_super_resolution.py`.

- [Pretrained Models](https://drive.google.com/file/d/1K0rlZ-iFW7q5Bjmap0CVgdUvQi-eohiO/view?usp=sharing)

---

## ⚙️ How to Run

Train the model:
```bash
python main.py
```

Evaluate the model:
```bash
python eval.py
```

Super-resolution tasks:
```bash
python super_resolution.py
```

---

## 📈 Results

| Problem               | FNO Performance | Traditional Solvers |
|------------------------|-----------------|---------------------|
| Burgers' Equation      | 3x faster        | Slower              |
| Darcy Flow             | 100x faster      | Much slower         |
| Navier-Stokes Equation | State-of-the-art | Poor generalization |

---

## ✨ Conclusion

The Fourier Neural Operator provides an efficient, scalable, and highly accurate method for learning PDE mappings.  
By working in Fourier space, we achieve faster training, better generalization, and superior performance over classical methods and traditional neural networks.

---

## 📩 Contact

For any questions or collaborations, feel free to reach out!

