# Stock Price Prediction
The project is a stock price prediction using LSTM (Long Short-Term Memory) in Python. It involves training a deep learning model to predict future stock prices based on historical price data.

Here's a brief explanation of the project:

1. Data Preparation: The project starts by loading the stock price data from a CSV file (replace with the actual data source). The 'Close' price column is extracted and scaled using MinMaxScaler to normalize the data.

2. Train-Test Split: The data is split into training and test sets, with 80% of the data used for training the model.

3. Sequence Creation: Sequences of input-output pairs are created from the training and test data. These sequences are used to train the LSTM model. The length of the input sequences is defined (e.g., 10), and the function 'create_sequences' generates the input-output pairs.

4. LSTM Model: The LSTM model is constructed using the Sequential API from TensorFlow Keras. It consists of an LSTM layer with 64 units and a dense output layer. The model is compiled with an optimizer (adam) and a loss function (mean squared error).

5. Model Training: The model is trained using the training data. The training process involves multiple epochs (e.g., 10) and a batch size (e.g., 16).

6. Prediction: The trained model is used to make predictions on the test data. The predictions are then inverse-transformed to obtain the actual stock price values.

7. Visualization: The actual and predicted stock prices are plotted using Matplotlib for visual comparison.

