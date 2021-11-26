# stockmarket-predictor

Many economists and investors have found it impossible to predict asset values. In reality, stock market forecast analysis has piqued the attention of investors. Many investors are interested in understanding the stock market's potential situation in order to make a good and profitable bet. Traders, buyers, and analysts benefit from good and accurate stock market forecast programs because they have supportive knowledge such as the stock market's potential trajectory. In this project, we showed how to forecast stock market indices using a Long Short- Term Memory (LSTM) method. Our system is divided into many stages, as follows:-

***Stage 1: Raw Data:***\
In this stage, the Apple company stock price dataset is collected from Tiingo
(https://www.tiingo.com) and this dataset is used for the prediction of future stock prices.

***Stage 2: Data Preprocessing:***\
The pre-processing stage involves:\
a) Data discretization: Part of data reduction but with particular importance, especially for numerical data\
b) Data transformation: Normalization.\
c) Data cleaning: Fill in missing values.\
We have used MinMaxScaler for data preprocessing.\
After the dataset is transformed into a clean dataset, the dataset is divided into training and
testing sets so as to evaluate. Here, the training values are taken as the more recent values. Testing data is kept as 35 percent of the total dataset.

***Stage 3: Feature Extraction:***\
Only the functions that will be fed to the neural network are chosen in this layer. Date, open, big, medium, near, and volume will be the features we choose.

***Stage 4: Training Neural Network:***\
In this stage, the data is fed to the neural network and trained for prediction assigning random biases and weights. Our LSTM model is composed of a sequential input layer followed by 3 LSTM layers and a dense output layer with a linear activation function.

***Stage 5: Output Generation:***\
The output value provided by the LSTM's output layer is compared to the target value in this layer. The error, or discrepancy between the objective and the received output value, is reduced using a backpropagation algorithm that changes the network's weights and biases. The Root Mean Square Error (RMSE) is used to evaluate the system's performance
