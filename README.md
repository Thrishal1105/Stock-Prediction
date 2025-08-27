## Stock Trend Prediction (Streamlit)

A simple Streamlit app that downloads historical stock data with `yfinance`, visualizes moving averages, and loads a pre-trained model (`keras_model.h5`) to plot predicted vs original prices.

### Features
- Data range: 2012–2023 (configurable via `start` and `end` in `app.py`)
- Summary table of open, high, low, close, volume
- Visualization: price, 100MA, 200MA
- Loads `keras_model.h5` and displays predictions vs original

### Quickstart (Windows PowerShell)
```powershell
./run_app.ps1
```
This script will create a virtual environment, install dependencies from `requirements.txt`, and run the app.

If you prefer manual steps:
```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
py -m pip install --upgrade pip
py -m pip install -r requirements.txt
streamlit run app.py
```

### Dependencies
See `requirements.txt`. Key libraries: `streamlit`, `yfinance`, `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `keras`, `tensorflow`.

### Model File
- Place your trained model as `keras_model.h5` in the project root (already referenced by `app.py`).

### Screenshot
The app’s predictions chart (provided by you) is embedded below. Save your image to `assets/predictions.png` to display it here.

![Predictions vs Original](assets/predictions.png)


### Notes
- If you get import warnings in your IDE, ensure it uses the same interpreter as the virtual environment created by the script.
- If `keras` import issues occur, use `tensorflow.keras` in `app.py` or ensure both `tensorflow` and `keras` are installed.


