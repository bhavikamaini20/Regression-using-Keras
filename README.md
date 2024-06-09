# Regression-using-Keras
basic understanding of regression using Keras

# Concrete Strength Prediction

This repository contains code for predicting the compressive strength of concrete using a neural network model. The project utilizes a dataset of various components used in concrete and their corresponding compressive strengths.

## Dataset

The dataset used in this project is obtained from [CognitiveClass](https://s3-api.us-geo.objectstorage.softlayer.net/cf-courses-data/CognitiveClass/DL0101EN/labs/data/concrete_data.csv). It consists of the following columns:

- `Cement`: Quantity of cement in kg per cubic meter (component 1)
- `Blast Furnace Slag`: Quantity of blast furnace slag in kg per cubic meter (component 2)
- `Fly Ash`: Quantity of fly ash in kg per cubic meter (component 3)
- `Water`: Quantity of water in kg per cubic meter (component 4)
- `Superplasticizer`: Quantity of superplasticizer in kg per cubic meter (component 5)
- `Coarse Aggregate`: Quantity of coarse aggregate in kg per cubic meter (component 6)
- `Fine Aggregate`: Quantity of fine aggregate in kg per cubic meter (component 7)
- `Age`: Age of concrete in days
- `Strength`: Concrete compressive strength in MPa

## Requirements

To run the code, you will need the following libraries:

- pandas
- numpy
- keras
- tensorflow

You can install these dependencies using pip:

```sh
pip install pandas numpy keras tensorflow
```

## Getting Started

1. Clone this repository:

```sh
git clone https://github.com/yourusername/concrete-strength-prediction.git
cd concrete-strength-prediction
```

2. Open and run the Jupyter notebook:

```sh
jupyter notebook Concrete_Strength_Prediction.ipynb
```

## Code Overview

1. **Data Loading and Preprocessing**:
   - The dataset is loaded using pandas.
   - The data is normalized by subtracting the mean and dividing by the standard deviation of each feature.

2. **Neural Network Model**:
   - A neural network model is defined using Keras.
   - The model consists of three dense layers with ReLU activation.
   - The model is compiled with the Adam optimizer and mean squared error loss function.

3. **Model Training**:
   - The model is trained on the normalized data with a validation split of 30%.
   - Training runs for 100 epochs.

## Results

The model is trained to predict the compressive strength of concrete based on the given features. The training and validation losses are tracked and displayed.

## Conclusion

This project demonstrates how to build and train a neural network model to predict concrete strength using a given dataset of concrete components. The model can be further optimized and tuned for better performance.

## License
This project is licensed under the MIT License.

## Acknowledgments

- The dataset used in this project is provided by [CognitiveClass](https://s3-api.us-geo.objectstorage.softlayer.net/cf-courses-data/CognitiveClass/DL0101EN/labs/data/concrete_data.csv).

## Contact

For any inquiries or questions, please contact [Bhavika Maini](bhavika.maini04@gmail.com).
