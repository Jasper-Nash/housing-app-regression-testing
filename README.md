# Housing Price Regression App

A Streamlit app that predicts a house's sale price from a few of its features,
using a linear regression model saved with `pickle`.

## How it works

The model (`lr_model.pkl`) is a scikit-learn pipeline that one-hot encodes the
categorical features and fits a linear regression. The app loads the pickled
model, collects inputs from the user, and shows the predicted sale price.

**Inputs:**
- Above-ground living area (`Gr_Liv_Area`)
- Total lot area (`Lot_Area`)
- Overall quality (`Overall_Qual`)
- Sale condition (`Sale_Condition`)

## Files

| File | Purpose |
|---|---|
| `app.py` | The Streamlit app |
| `lr_model.pkl` | The trained regression model |
| `requirements.txt` | Package versions needed to run the app |

## Run it locally

Requires Python 3.13 or earlier (scikit-learn 1.6.1 doesn't support 3.14).

```
pip install -r requirements.txt
streamlit run app.py
```
