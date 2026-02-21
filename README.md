# Pokemon ML Classification

A collection of self-contained notebooks that apply machine learning and deep learning techniques to Pokémon classification tasks using both structured tabular data and image-based computer vision.

This repository includes:
- A tabular classification model to predict whether a Pokémon is "legendary".
- An image-based neural network model to predict Pokémon types from images.

## Key points
- Uses SMOTE to balance a highly imbalanced target class in the tabular dataset.
- Implements preprocessing pipelines with imputation, scaling and one-hot encoding.
- Compares Decision Tree, Random Forest, AdaBoost and Gradient Boosting classifiers (up to 97% F1-score).
- Trains a convolutional neural network (CNN) for multi-class image classification of Pokémon types.

## Quick start
1. Open and run either notebook:
   - `legendary_pokemon_classifier.ipynb`
   - `pokemon_image_type_classifier.ipynb`
2. The legendary classifier notebook downloads the dataset from Kaggle (dataset: `kingabzpro/pokmon-legendary-data`) using `kagglehub`. If you prefer not to use `kagglehub`, place `pokedex.csv` next to the notebook and update the path in the first cells.
3. Install the minimal dependencies (example):

```bash
pip install pandas numpy scikit-learn imbalanced-learn seaborn matplotlib kagglehub tensorflow
```

(If using PyTorch instead of TensorFlow, install `torch` and related vision packages instead.)

## What you'll see
- Data loading and basic EDA for structured Pokédex data.
- Preprocessing pipeline with imputation, scaling and one-hot encoding.
- SMOTE resampling to balance classes.
- Training and evaluation of ensemble classifiers with metric tables and plots.
- Image preprocessing, CNN model training and evaluation with accuracy and loss tracking.

## Notes
- The notebooks are intended for exploration and demonstration; use cross-validation, hyperparameter tuning and model optimization for production use.

## License
See the `LICENSE` file in this repository.
