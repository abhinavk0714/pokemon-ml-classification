# legendary-pokemon-classifier

A short, self-contained notebook that trains classifiers to predict whether a Pokémon is "legendary" using a Kaggle Pokédex dataset.

Key points
- Uses SMOTE to balance the (highly imbalanced) target class.
- Compares Decision Tree, Random Forest, AdaBoost and Gradient Boosting classifiers.
- Evaluates precision, recall and F1; RandomForest and GradientBoosting perform best in the notebook.

Quick start
1. Open and run the notebook `legendary_pokemon_classifier.ipynb`.
2. The notebook downloads the dataset from Kaggle (dataset: `kingabzpro/pokmon-legendary-data`) using `kagglehub`. If you prefer not to use `kagglehub`, place `pokedex.csv` next to the notebook and update the path in the first cells.
3. Install the minimal dependencies (example):

```bash
pip install pandas numpy scikit-learn imbalanced-learn seaborn matplotlib kagglehub
```

What you'll see
- Data loading and basic EDA.
- Preprocessing pipeline with imputation, scaling and one-hot encoding.
- SMOTE resampling to balance classes.
- Training and evaluation of multiple classifiers with metric tables and plots.

Notes
- The notebook is intended for exploration and demonstration; use cross-validation and hyperparameter tuning for production use.

License
See the `LICENSE` file in this repository.