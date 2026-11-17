# Solar-Power-Forecasting
# Beatriz Lima - up202511105

## Files
- `forecast_solar.ipynb` – notebook with all the code (data -> features -> models -> validation -> submition)
- `forecast_solar.py` - python code version of `forecast_solar.ipynb`
- `up202511105_forecast.csv` – Submitted forecast (4296 lines)
- `model_matrix.csv` – matriz de modelos (validação cruzada em blocos mensais, leads 1-24)
- `requirements_used.md` – library versions

## How to reproduce
1. Put all the files in the same folder: `Solar_dataset_train.csv`, `Solar_dataset_test.csv`, `submission_template.csv`, `check_submission.py`.
2. Open the notebook and execute **Restart and run all**.
3. The notebook writes  `up202511105_forecast.csv` and runs `check_submission.py` (must print "Submission is VALID").

Seed: SEED = 42. Final model: M7-PP with FS_ENS (train with leads 1-24).
The models only use information available in each run; any model, scaler ou variable selection uses test data.
