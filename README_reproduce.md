# Previsão de potência solar PV – up202511105

## Ficheiros
- `forecast_solar.ipynb` – notebook com todo o código (dados -> features -> modelos -> validação -> submissão)
- `up202511105_forecast.csv` – previsões submetidas (4 296 linhas)
- `model_matrix.csv` – matriz de modelos (validação cruzada em blocos mensais, leads 1-24)
- `requirements_used.txt` – versões das bibliotecas

## Como reproduzir
1. Colocar na mesma pasta: `Solar_dataset_train.csv`, `Solar_dataset_test.csv`, `submission_template.csv`, `check_submission.py`.
2. Abrir o notebook (Python 3, Colab ou local) e executar **Restart and run all**.
3. O notebook escreve `up202511105_forecast.csv` e corre o `check_submission.py` (deve imprimir "Submission is VALID").

Sementes: SEED = 42. Modelo final: M7-PP com FS_ENS (treino com leads 1-24).
Só se usa informação disponível à emissão de cada run; nenhum modelo, scaler ou seleção de variáveis usa dados de teste.
