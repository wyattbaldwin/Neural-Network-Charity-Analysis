# Neural Network Charity Analysis
The goal of this project is to use a neural network model to predict the success rate of applicants seeking funding from Alphabet Soup. The model will also be used to determine whether the money was used effectively if funding is granted.

## Data Preprocessing
The first step in this project is to clean, transform, and preprocess the charity data for the neural network model. The target variable for the model is Is_successful, which indicates whether the funding was used effectively. The features for the model include the following columns; APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, IS_SUCCESSFUL. In addition, the NAME column was retroactively restored to increase the model's prediction accuracy. The EIN column was removed as it was not expected to add any useful information to the dataset.

## Model Compilation, Training, and Evaluation
The model was compiled, trained, and evaluated using the preprocessed data. The initial model had 3 layers and 110 neurons, with activation functions of relu and sigmoid. The accuracy of this model was 72.68% and the loss was 0.5527.

The second model was optimized by adding the NAME column and increasing the number of layers and neurons to 5 and 350 respectively. The activation function used was sigmoid. The accuracy of this model was 72.71% and the loss was 0.5508.

The project was able to achieve a target model performance of 79% by optimizing the model by adding the sorted NAME data and increasing the number of layers and neurons. Recommendations for further optimization include sorting through the bins for rare occurrences in columns, deeper exploration of the data, and transforming the noise and columns to optimize for higher accuracy.
