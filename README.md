# Algorithmic Trading Model Readme

## Overview
This project contains Python code for an algorithmic trading model that utilizes historical OHLCV (Open, High, Low, Close, Volume) data to generate trading signals. The model is based on a Random Forest Classifier and incorporates technical analysis indicators such as Moving Averages and Relative Strength Index (RSI) to make buy, sell, or hold decisions.

## Files
- **RandomForest.py:** The main Python script containing the algorithmic trading model. It includes functions for reading historical data, creating features, calculating RSI, labeling data based on trading signals, and training the machine learning model.

## Usage
1. **Upload Data:** Run the script, and it will prompt you to upload a CSV file containing historical OHLCV data. The file should include columns for 'datetime', 'open', 'high', 'low', 'close', and 'volume'.

2. **Feature Engineering:** The script will create additional features such as moving averages (ma5, ma20) and the Relative Strength Index (RSI) to enhance the model's predictive capabilities.

3. **Labeling Data:** Trading signals (Buy: 1, Sell: -1, Hold: 0) are generated based on a simple strategy using moving averages.

4. **Model Training:** The features and labels are used to train a Random Forest Classifier. The model's accuracy and a classification report are printed to evaluate its performance.

## Dependencies
- pandas
- numpy
- scikit-learn
- google.colab (for data upload in Google Colab)

Install the dependencies using:
```bash
pip install pandas numpy scikit-learn
```

## Running the Script
Execute the script by running the following command:
```bash
python RandomForest.py
```

## Contributing
Feel free to contribute to this project by opening issues or pull requests. Any feedback or improvements are highly appreciated.


Happy coding 🚀
