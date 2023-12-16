# Music Recommender Decision Tree Model

## Overview

This repository contains a decision tree model for recommending music based on the user's gender and age. The decision tree has been trained to provide personalized music recommendations, taking into account both demographic factors.

## Decision Tree Visualization

![Decision Tree](decision_tree.png)

![image](https://github.com/mohamedmouhibnaffeti/music-recommender/assets/107668257/b37939e6-827b-4d33-9934-35713b52574a)


## How It Works

The decision tree model uses the user's gender and age as input features to navigate through the tree and make recommendations. The nodes of the tree represent decision points, and the leaves contain the recommended music genres or specific songs.

## Getting Started

To use the music recommender model in your own project, follow these steps:

1. **Download the Model File:**
   - Download the pre-trained decision tree model file named `music-recommender.joblib` from the repository.

2. **Integrate the Model:**
   - Load the decision tree model in your Python environment using a library like scikit-learn:
     ```python
     import joblib

     # Load the model
     model = joblib.load('music-recommender.joblib')
     ```

3. **Make Predictions:**
   - Use the model to make music recommendations based on user input:
     ```python
     # Example input: gender and age
     user_data = [42, 0]

     # Make a prediction
     recommendation = model.predict([user_data])
     print(f"Recommended music: {recommendation}")
     ```

## Model Details

- **Features:**
  - Gender: 'male' or 'female' represented as 1 and 0
  - Age: Integer representing the user's age

- **Output:**
  - The model outputs recommended music genres.

## Contributing

If you have suggestions, bug reports, or want to contribute to the development of this music recommender model, feel free to open an issue or submit a pull request.

Enjoy recommending music with the decision tree model! 🎶
