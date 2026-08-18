# Zepto Rider Acceptance Predictor — Streamlit App

## Setup
```
pip install -r requirements.txt
```

## Run
```
streamlit run streamlit_app.py
```

Make sure `rider_acceptance_model.pkl` sits in the same folder as `streamlit_app.py`
(already included here).

## Notes
- Trained with scikit-learn 1.6.1 — the pinned version in requirements.txt avoids
  the pickle-compatibility warning/break you'd get on newer sklearn releases.
- Page 1: interactive prediction form matching your notebook's exact 23-feature schema.
- Page 2: synthetic sample order table (50 rows) run through the model, with
  predicted acceptance + probability columns, plus CSV download.
