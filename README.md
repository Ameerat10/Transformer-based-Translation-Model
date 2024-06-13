# Transformer-based-Translation-Model
This project represents Python code for training a Transformer-based neural network model to translate text between Lingala and English languages. The model utilizes the TensorFlow framework and Keras API for implementation. 


## Key Steps

### Dataset Loading and Tokenization
- Load and preprocess the dataset (`verse_pairs.csv`) containing Lingala-English text pairs.
- Tokenize text using TensorFlow's `Tokenizer` for both Lingala and English languages.

### Data Preprocessing
- Pad sequences to a fixed length using `pad_sequences` to ensure uniform sequence length for model training.

### Model Architecture
- Implement a Transformer architecture using Keras layers:
  - Embedding layers with positional encoding.
  - Multi-head self-attention and feed-forward neural network layers.
  - Encoder and decoder layers for processing both input and target sequences.
  - Output layer with softmax activation for predicting the next word in the translated sequence.

### Training and Evaluation
- Split the dataset into training, validation, and test sets using `train_test_split`.
- Define the model's optimizer (Adam) and loss function (sparse categorical cross-entropy).
- Train the model on the Lingala-English text pairs with monitoring of validation loss and accuracy.
- Adjust hyperparameters such as batch size, learning rate, and number of epochs as necessary.

## Dependencies
- TensorFlow
- pandas
- scikit-learn

