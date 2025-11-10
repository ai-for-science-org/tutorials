# 🧬 Foundation Models for Science Workshop: Protein Machine Learning Tutorials

November 3-5, 2025 | University of Toronto

Repository of hands-on workshop materials for [**Foundation Models for Science Workshop**](ai-for-science.org). These tutorials cover the complete workflow of working with protein language models, from data preparation to advanced analysis techniques.

---

## 📚 Table of Contents

- [Installation](#-installation)
- [Tutorials Overview](#-tutorials-overview)
  - [Tutorial 1: Data Extraction & Cleaning](#-tutorial-1-data-extraction--cleaning)
  - [Tutorial 2: Model Fine-Tuning](#-tutorial-2-model-fine-tuning)
  - [Tutorial 3: Uncertainty Quantification](#-tutorial-3-uncertainty-quantification)
  - [Tutorial 4: Latent Space Analysis](#-tutorial-4-latent-space-analysis)
- [Getting Started](#-getting-started)
- [Requirements](#-requirements)

---

## 🚀 Installation

### 1. Launch the Docker instance

The required packages are pre-installed in a Docker container. 

You will need to configure your local computer using [the official Docker instructions](https://www.docker.com/get-started/). 

```docker
docker pull ghcr.io/carte-toronto/utoronto-fms-workshop-pytorch:latest
```

The official repository for this Docker is [here](https://github.com/CARTE-Toronto/utoronto-fms-workshop-pytorch).

> ***Important*** A `requirements.txt` file is provided as a courtesy only.  Please use the Docker container. 

### 2. Clone the Repository

```bash
git clone https://github.com/ai-for-science-org/tutorials.git
cd tutorials
```

### 3. Launch Jupyter

```bash
jupyter lab
```

---

## 📖 Tutorials Overview

### 🧬 Tutorial 1: Data Extraction & Cleaning

**📂 Location:** `Tutorial_1_Data_Cleaning/Data_Extraction.ipynb`

**What You'll Learn:**

- Download and extract datasets from ProteinGym
- Clean and standardize tabular data with pandas
- Handle missing values and duplicates
- Normalize DMS (Deep Mutational Scanning) scores for machine learning
- Visualize dataset characteristics

**Key Skills:** Data wrangling, pandas operations, data quality assessment

---

### 🔬 Tutorial 2: Model Fine-Tuning

**📂 Location:** `Tutorial_2_Fine_Tuning/` *(Notebook TBD)*

**What You'll Learn:**

- Load and use pre-trained protein language models (ESM-2)
- Generate protein embeddings for downstream tasks
- Perform zero-shot similarity search
- Fine-tune models with LoRA (Low-Rank Adaptation)
- Predict DMS stability scores using adapted models

**Key Skills:** Transfer learning, model adaptation, embedding generation

---

### 🎯 Tutorial 3: Uncertainty Quantification

**📂 Location:** `Tutorial_3_Uncertainty_Quant/UQ_tutorial.ipynb`

**What You'll Learn:**

- Assess and improve model calibration using temperature scaling
- Implement heteroscedastic models to capture prediction uncertainty
- Use MC dropout to estimate epistemic uncertainty
- Apply conformal prediction for distribution-free uncertainty intervals
- Distinguish between different types of uncertainty in your predictions

**Key Skills:** Confidence estimation, calibration methods, probabilistic prediction

---

### 🧠 Tutorial 4: Latent Space Analysis

**📂 Location:** `Tutorial_4_Latent_Space/Latent_Space_Analysis.ipynb`

**What You'll Learn:**

- Extract and manipulate protein embeddings from pre-trained ESM2 models
- Reduce high-dimensional embeddings to 2D for visualization using UMAP
- Quantify clustering quality using mutual information metrics
- Optimize dimensionality reduction hyperparameters automatically with Optuna
- Analyze how features change across different layers of a transformer model
- Interpret latent space structure in relation to protein function (EC classes)

**Key Skills:** Embedding analysis, dimensionality reduction, hyperparameter optimization, interpretability

---

## 📦 Requirements

### Core Dependencies

- **Python**: 3.8 or higher
- **PyTorch**: For deep learning models
- **Transformers**: HuggingFace library for ESM models
- **Pandas**: Data manipulation
- **NumPy**: Numerical computing
- **Matplotlib/Seaborn**: Visualization

### Specialized Libraries

- **UMAP**: Dimensionality reduction (Tutorial 4)
- **Optuna**: Hyperparameter optimization (Tutorial 4)
- **scikit-learn**: Machine learning utilities
- **tqdm**: Progress bars

### Hardware Recommendations

- **GPU**: Recommended for Tutorial 2 (fine-tuning) and Tutorial 4 (embeddings)
- **RAM**: 16GB minimum, 32GB recommended
- **Storage**: ~10GB for datasets and models

---

## 📝 License

See [LICENSE](LICENSE) file for details.

---

## 🤝 Contributing

This is a private workshop repository. For questions or issues, please contact the workshop organizers.

---

## 📧 Support

For technical support or questions about the tutorials, please reach out to the FOMO4Sci Workshop team.

---

**Happy Learning! 🚀**
