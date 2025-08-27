## Stock Trend Prediction (Streamlit)

A simple Streamlit app that downloads historical stock data with `yfinance`, visualizes moving averages, and loads a pre-trained model (`keras_model.h5`) to plot predicted vs original prices.

### Features
- Data range: 2012–2023 (configurable via `start` and `end` in `app.py`)
- Summary table of open, high, low, close, volume
- Visualization: price, 100MA, 200MA
- Loads `keras_model.h5` and displays predictions vs original

![image alt](https://github.com/Thrishal1105/Stock-Prediction/blob/1fd6189d7ab00bacde199f0015814f9cbb612f6a/Screenshot%202025-08-27%20145358.png)



### Dependencies
See `requirements.txt`. Key libraries: `streamlit`, `yfinance`, `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `keras`, `tensorflow`.

### Model File
- Place your trained model as `keras_model.h5` in the project root (already referenced by `app.py`).




### Notes
- If you get import warnings in your IDE, ensure it uses the same interpreter as the virtual environment created by the script.
- If `keras` import issues occur, use `tensorflow.keras` in `app.py` or ensure both `tensorflow` and `keras` are installed.


