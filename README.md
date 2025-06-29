# Stock-Market-Prediction-Using-LSTM
Stock Market Prediction Using LSTM
This project implements a deep learning-based model to predict stock market trends using Long Short-Term Memory (LSTM) networks. It utilizes historical stock price data and sentiment analysis (simulated) to forecast next-day closing prices and visualize the trend, helping in short-term intraday trading decisions.

Features
LSTM-based time series prediction

Dual-layer LSTM architecture for improved accuracy

Interactive Streamlit web app for real-time prediction

Visualizations of stock prices (real vs predicted)

Simulated sentiment analysis integration

CSV file upload support for custom prediction

Clean and modular codebase

🗂️ Project Structure
bash
Copy
Edit
.
├── dataset/                # Sample dataset and historical stock data
├── saved_model/           # Saved LSTM model
├── sentiment/             # Simulated sentiment analysis logic
├── utils/                 # Data preprocessing utilities
├── main_app.py            # Streamlit application
├── lstm_model.py          # LSTM model architecture
├── prediction.py          # Model prediction logic
├── train_model.py         # Model training script
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation

🛠️ Installation
Create a virtual environment:

bash
Copy
Edit
python -m venv venv
# On Windows
venv\Scripts\activate
# On Mac/Linux
source venv/bin/activate
Install required dependencies:

bash
Copy
Edit
pip install -r requirements.txt

 Usage
Train the model (optional if already trained):

bash
Copy
Edit
python train_model.py
Run the Streamlit app:

bash
Copy
Edit
streamlit run main_app.py
On the UI:

Select stock ticker

Choose date range

Upload your own CSV (optional)

View predicted vs actual graphs and sentiment outputs

 Configuration
The application supports customization:

Modify train_model.py for different tickers or date ranges

Replace or add sentiment logic in sentiment/ folder

Customize model parameters in lstm_model.py

 Example Output
 Model Prediction Graphs
 Real vs Predicted Price
 Sentiment Analysis Result: Positive / Negative / Neutral

 Requirements
Python 3.7+

TensorFlow / Keras

Streamlit

Pandas, NumPy, Matplotlib

yfinance (Yahoo Finance API)

 License
This project is licensed under the MIT License.











