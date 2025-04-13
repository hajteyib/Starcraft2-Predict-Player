
# StarCraft II Player Identification via Behavioral Trace Analysis

This project aims to identify players in StarCraft II using machine learning techniques applied to behavioral data extracted from game replays. This work was conducted as part of a learning challenge to predict which player is playing a game based on their unique in-game behavior.

## 🧠 Objective

The goal is to develop a model capable of predicting the identity of a player based on the sequence of actions they performed during a match. These actions are extracted from replays and include hotkey usage, selection patterns, camera movements, and more.

## 🗃️ Data Description

The dataset includes:

- **TRAIN / TEST**: Raw action logs with events like hotkeys and selections.
- **TRAIN_LONG / TEST_LONG**: Enriched logs with more detailed events (camera, unit commands, etc.).
- **SAMPLE_SUBMISSION**: A sample format for submitting predictions.

Each row corresponds to a player's behavioral trace during one game, with actions and events timestamped or categorized.

## 🧪 Approach

This project explores multiple modeling approaches and feature extraction strategies across several notebooks. The core steps include:

- **Data parsing**: Transforming raw action sequences into usable features.
- **Feature engineering**: Extracting statistics from action types, frequency, timings, etc.
- **Model experimentation**: Comparing various classifiers (Random Forest, XGBoost, etc.).
- **Evaluation**: Validating performance on the training data and generating predictions for submission.

All experiments are organized in the `code/` folder.

## 📁 Repository Structure

```
.
├── code/                   # Notebooks with experiments
├── data/                   # Contains training and test CSVs
├── results/                # (optional) Submission or model outputs
├── README.md               # Project overview (this file)
└── .gitignore              # Ignore unnecessary files
```

## 🚀 Future Work

- Improve feature engineering based on player behavior sequences
- Integrate sequence models (e.g. RNNs or Transformers)
- Optimize model ensemble for better leaderboard performance
