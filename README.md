# Forest Cover Type Classification

A machine learning project to predict forest cover types based on cartographic variables. Using Python and scikit-learn, this project analyzes the UCI Forest CoverType dataset and builds classification models to identify tree species distribution.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Methodology](#methodology)
- [Results](#results)
- [Dependencies](#dependencies)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

---

## 🔍 Project Overview

This project predicts the forest cover type (species of tree in a given area) using environmental and cartographic variables. Accurate classification helps in forest management, ecology research, and conservation planning.

Key goals:

- Explore and preprocess the Forest CoverType dataset.
- Train and evaluate classification algorithms such as Decision Trees, Random Forests, and Gradient Boosting.
- Analyze feature importance and model performance.

---

## 📊 Dataset Description

The **Forest CoverType** dataset is sourced from the UCI Machine Learning Repository. It contains 581,012 samples with 54 attributes:

- **10** quantitative variables (e.g., elevation, slope, horizontal distance to water)
- **4** categorical wilderness areas (one-hot encoded)
- **40** soil type indicators (one-hot encoded)
- **1** target variable: `Cover_Type` (integer 1–7)

The dataset is available in the notebook `Forest_Cover_Type.ipynb`.

---

## 🗂 Project Structure

```
forest-cover-type-classification/
├── Forest_Cover_Type.ipynb   # Jupyter Notebook with analysis and modeling
├── data/                      # (Optional) Raw and processed data files
├── models/                    # Saved trained model files
├── requirements.txt           # Python dependencies
├── README.md                  # Project overview and instructions
└── .gitignore                 # Ignored files & folders
```

---

## 🛠 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/<swapnil bilgoji>/forest-cover-type-classification.git
   cd forest-cover-type-classification
   ```
2. (Optional) Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate    # Windows: venv\Scripts\activate
   ```
3. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

---

## ▶️ Usage

1. Launch the Jupyter Notebook:
   ```bash
   jupyter notebook Forest_Cover_Type.ipynb
   ```
2. Follow the notebook to:
   - Load and explore the data
   - Preprocess features (scaling, encoding)
   - Train classification models
   - Evaluate using accuracy, confusion matrix, and classification report
   - Visualize feature importance and results

---

## 📈 Methodology

1. **Data Exploration**: Inspect distributions, correlations, and missing values.
2. **Preprocessing**:
   - Standardize quantitative variables.
   - Handle categorical variables (one-hot encoding).
   - Split data into training and test sets.
3. **Modeling**:
   - Train models: Decision Tree, Random Forest, Gradient Boosting.
   - Perform cross-validation and hyperparameter tuning.
4. **Evaluation**:
   - Compute accuracy, precision, recall, F1-score.
   - Plot confusion matrices.
   - Analyze feature importance.

---

## 🏆 Results

- **Random Forest** achieved the highest accuracy of **\~0.94** on the test set.
- Top predictive features included **Elevation**, **Horizontal Distance to Roadways**, and **Slope**.
- Gradient Boosting provided competitive performance with slightly slower training time.

---

## 📦 Dependencies

Key libraries listed in `requirements.txt`:

- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn

---

## 🚀 Future Work

- Incorporate additional algorithms (e.g., XGBoost, lightGBM).
- Optimize hyperparameters using GridSearchCV or Bayesian optimization.
- Deploy the best model as a REST API using Flask or FastAPI.
- Build a simple web dashboard for visualizing predictions.

---

## 🤝 Contributing

Contributions are welcome! Please:

1. Fork the repo
2. Create a feature branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m 'Add feature'`)
4. Push to branch (`git push origin feature-name`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

