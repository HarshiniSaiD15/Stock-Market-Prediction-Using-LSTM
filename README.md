
Stock Market Prediction Using LSTM
This project implements a deep learning model using Long Short-Term Memory (LSTM) networks to forecast stock prices. It provides an interactive interface for intraday stock prediction, combining technical stock data and simulated sentiment logic for better decision-making.
Features
•	LSTM-based sequence modeling for stock prediction
•	Dual-layer architecture for enhanced learning
•	Real vs Predicted graph output
•	Simulated sentiment analysis
•	Streamlit web app for real-time interaction
•	CSV upload and date range support

Project Structure
.
├── dataset/                         # Historical stock data (CSV files)
├── saved_model/                     # Pre-trained LSTM model
├── main_app.py                      # Streamlit app for daily stock prediction
├── intradaytraining_lstm.py         # Streamlit app for intraday prediction
├── Stock Market Prediction Keras.ipynb  # Jupyter Notebook for model training
├── requirements.txt                 # Project dependencies
└── README.md                        # Project documentation
Installation
1.	Create a virtual environment:
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate
2.	Install dependencies:
pip install -r requirements.txt
Usage
Step 1 : Train the model:
Open and run the Jupyter notebook:
 Stock Market Prediction Keras.ipynb
This notebook:
•	Downloads & preprocesses historical stock data
•	Trains a dual-layer LSTM model
•	Saves the trained model in saved_model/
	Note: You only need to train once. Skip this step if the model is already saved.
       Step 2: Run the Streamlit Applications
A.	General Stock Prediction App:
streamlit run main_app.py
B.	Intraday Trend Prediction App:
streamlit run intradaytraining_lstm.py
Both apps allow you to:
	Select stock ticker and date range
		Upload custom CSV files
		Visualize actual vs predicted closing prices
	View sentiment analysis output (positive/negative/neutral)
Requirements
•	Python 3.7+
•	TensorFlow / Keras
•	Streamlit
•	pandas, numpy, matplotlib
•	yfinance
Configuration
The system can be configured through user inputs and source code changes. Key configurable components include:
•	Stock Ticker Selection: Choose different stocks using the dropdown in the Streamlit app.
•	Date Range Selection: Define custom date ranges for fetching and visualizing stock data.
•	CSV File Upload: Upload your own stock dataset for prediction.
•	Model Architecture Parameters: Modify the number of LSTM layers, units, and dropout rates in lstm_model.py.
•	Training Settings: Change batch size, epochs, or learning rate in the training notebook (Stock Market Prediction Keras.ipynb).
•	Sentiment Logic: Customize or replace the simulated sentiment analysis in the sentiment/ directory.
•	Visualization Styles: Update plot designs and layout in main_app.py or intradaytraining_lstm.py.
License
MIT License












