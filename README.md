# Next Word Prediction with LSTM using TensorFlow and Keras.

**<h3>Introduction</h3>**

This project aims to build a next-word prediction model using Long Short-Term Memory (LSTM) neural networks. The model will generate text based on a given input word.

**<h3>Dataset</h3>**

The dataset used for training the model is extracted from the 'tmdb_5000_movies.csv' file. This dataset contains movie titles, which will be used to train the next-word prediction model.


**<h3>Dependencies</h3>**

To run the code in this repository, you will need the following dependencies:

    pandas
    TensorFlow
    Keras
    numpy

**<h3>Instructions for Use</h3>**

• Clone the repository to your local machine.

• Install the required dependencies using pip install -r requirements.txt.

• Load the dataset 'tmdb_5000_movies.csv' into a pandas DataFrame.

• Train the model using the provided code snippet.

• Use the 'make_prediction()' function to generate text based on a given input word.



**<h3>Model Architecture</h3>**

The model architecture consists of the following layers:

1. Embedding layer: Converts input words into dense vectors of fixed size.
2. LSTM layer 1: A Long Short-Term Memory layer with 100 units, returning sequences.
3. LSTM layer 2: A Long Short-Term Memory layer with 100 units.
4. Dense layer 1: A dense layer with 100 units and ReLU activation.
5. Dense layer 2: The output layer with a softmax activation, predicting the probability distribution of the next word.

**<h3>Training Process</h3>**

The model is compiled with the Adam optimizer and categorical cross-entropy loss. It is then trained using the 'X' and 'y' data for 150 epochs.
Text Generation

The 'make_prediction()' function generates new text based on a given starting word. It predicts the next word using the trained LSTM model and repeats the process for the desired number of words.

**<h3>Results</h3>**

Here are some example outputs of the text generation process:

![image](https://github.com/yaaaash/Next-Word-Predictor/assets/87315730/ed28d9b0-e279-4839-9f95-7f50640ac9f1)

![image](https://github.com/yaaaash/Next-Word-Predictor/assets/87315730/062db05d-aab6-4a72-80f4-bdbb34a859fe)


**<h3>Future Improvements</h3>**

• Fine-tune the model architecture and hyperparameters for better performance.

• Explore larger datasets to enhance the model's ability to generate creative text.
