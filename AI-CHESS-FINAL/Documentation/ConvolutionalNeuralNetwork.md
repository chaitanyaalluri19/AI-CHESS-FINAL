### ConvolutionalNeuralNetwork - This class is used to create, train, save, load, and predict the results of convolutional neural networks.
 - The model has two branches, one for the board and one for the turn.
 - The board branch is a convolutional neural network that takes  the board as a tensor and outputs a tensor.
 - A turn branch is a fully connected neural network that takes turns as a tensor and outputs a tensor.
 – The two branches are then merged and passed through a  fully connected set of layers.
 The output layer is a fully connected layer with three nodes, one for each possible outcome.
 The model was compiled using the Adam optimizer, categorical cross entropy loss, and accuracy metrics.
 - The model is trained for 128 epochs with  batch size  64 and  validation split  0.3
 #### Properties - input_board: Board branch input layer  - input_turn: Turn branch input layer  - Model: Neural network model  #### Method - 'train(path) ': Train the model using the dataset on the specified path.
 - 'predict(fen=None,board_tensor=None,turn_tensor=None)': Predict the outcome of the given board and turn.
 - 'save(path)': Save the model to the specified path.
 - 'load(path)': Loads the model from the specified path.
 - 'preprocess_data(path)': Preprocess the data set at the specified path.



#### Example 
```python
# Create the model
model = ConvolutionalNeuralNetwork()

# Train the model
model.train("Resources/training_dataset.json")

# Predict the result
model.predict("rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - 0 1")

# Output = [0. 1. 0.] (draw)
```

