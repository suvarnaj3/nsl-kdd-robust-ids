# NSL-KDD Robust Binary Intrusion Detection

A robust binary network intrusion detection system (IDS) built using the NSL-KDD dataset.

---

## 🎯 Project Goals & Scope

The primary objective is to build a binary intrusion detection model (Normal vs. Attack) and evaluate its resilience in realistic, adversarial, and non-stationary network environments through four key study areas:

1. **Class Imbalance**: Evaluating and mitigating class imbalance between normal traffic and low-frequency attack classes.
2. **Feature Perturbation Robustness**: Analyzing model degradation under noise, missing features, and adversarial feature modifications.
3. **Simulated Concept Drift**: Modeling shifts in network traffic distributions and emerging attack patterns over time.
4. **Static vs. Adaptive Models**: Comparing traditional static offline models (e.g., scikit-learn, XGBoost) against online, streaming adaptive architectures (e.g., River).

---

## 📁 Repository Structure

```text
nsl-kdd-robust-ids/
│
├── data/
│   ├── raw/              # Original unprocessed NSL-KDD datasets
│   └── processed/        # Cleaned, encoded, and split datasets
│
├── notebooks/            # Exploratory data analysis and experimental notebooks
│
├── src/                  # Reusable Python source modules (preprocessing, models, evaluation)
│
├── models/               # Saved model artifacts and weights
│
├── results/
│   ├── figures/          # Visualizations, confusion matrices, and plots
│   └── metrics/          # Evaluation metrics, benchmarking logs, and summaries
│
├── README.md             # Project documentation
├── requirements.txt      # Project dependencies
└── .gitignore            # Git ignore rules for Python/ML/Jupyter projects
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.9+ recommended

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/nsl-kdd-robust-ids.git
   cd nsl-kdd-robust-ids
   ```

2. Create and activate a virtual environment:
   ```bash
   # Linux/macOS
   python3 -m venv venv
   source venv/bin/activate

   # Windows
   python -m venv venv
   venv\Scripts\activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## 📦 Core Dependencies

- **Data Processing & ML**: `numpy`, `pandas`, `scikit-learn`, `xgboost`, `imbalanced-learn`
- **Online & Adaptive Learning**: `river`
- **Visualization**: `matplotlib`, `seaborn`
- **Serialization & Notebooks**: `joblib`, `jupyter`
