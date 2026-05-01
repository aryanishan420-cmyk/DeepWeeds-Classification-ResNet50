# 🌿 DeepWeeds Classification with ResNet50

> Automated weed species identification using deep learning and transfer learning on the DeepWeeds benchmark dataset.

---

## 📌 Overview

Weed management is one of the most labour-intensive and costly challenges in modern agriculture. Manual identification of weed species is slow, inconsistent, and impossible to scale across large farms. This project addresses that problem by building a **deep learning image classification pipeline** capable of automatically identifying weed species from field photographs.

The model is trained on the **DeepWeeds dataset** — a real-world benchmark containing over 17,000 labelled images of **9 weed species** native to Australia, collected across various sugarcane growing regions.

---

## 🧠 How It Works

The project uses **ResNet50** (Residual Network with 50 layers) with **transfer learning**:

1. **Pretrained weights** from ImageNet are loaded to give the model a strong visual foundation.
2. The **top classification layers are replaced** and fine-tuned on the DeepWeeds dataset.
3. The model learns to distinguish between 9 weed classes and a non-weed (negative) class.

This approach achieves strong accuracy while requiring significantly less training data and compute than training from scratch.

---

## 🛠️ Tech Stack

| Tool / Library | Purpose |
|---|---|
| Python | Core programming language |
| TensorFlow / Keras | Deep learning framework |
| ResNet50 | Pretrained CNN backbone (transfer learning) |
| NumPy | Numerical computations |
| Matplotlib | Plotting training metrics and results |
| Jupyter Notebook | Experimentation and development |

---

## 🗂️ Project Structure

```
DeepWeeds-Classification-ResNet50/
│
├── notebooks/          # Jupyter notebooks for training & evaluation
├── src/                # Source scripts (preprocessing, model, utils)
├── results/            # Output metrics, plots, and saved models
├── output accuracy.png # Training accuracy visualization
└── README.md
```

---

## 🌾 Dataset

**DeepWeeds** is an open-source dataset developed by the University of Queensland.

- **9 weed species** + 1 negative (non-weed) class
- **17,509 images** collected in the field across Queensland, Australia
- Images taken in diverse lighting and growth conditions

> Dataset source: [DeepWeeds on GitHub](https://github.com/AlexOlsen/DeepWeeds)

---

## 📈 Results

Training and validation accuracy curves are available in `output accuracy.png` and the `results/` directory.

The ResNet50 transfer learning approach achieves competitive classification accuracy across all 9 weed species, significantly outperforming training from scratch.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/aryanishan420-cmyk/DeepWeeds-Classification-ResNet50.git
cd DeepWeeds-Classification-ResNet50
```

### 2. Install dependencies

```bash
pip install tensorflow numpy matplotlib jupyter
```

### 3. Download the DeepWeeds dataset

Follow instructions at [https://github.com/AlexOlsen/DeepWeeds](https://github.com/AlexOlsen/DeepWeeds) to download and place the dataset in the appropriate directory.

### 4. Run the notebook

```bash
jupyter notebook notebooks/
```

---

## 🔗 Links

- 📂 **GitHub Repository:** [DeepWeeds-Classification-ResNet50](https://github.com/aryanishan420-cmyk/DeepWeeds-Classification-ResNet50)
- 📊 **DeepWeeds Dataset:** [AlexOlsen/DeepWeeds](https://github.com/AlexOlsen/DeepWeeds)

---

## 👤 Author

**Aryan Ishan**
- GitHub: [@aryanishan420-cmyk](https://github.com/aryanishan420-cmyk)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
