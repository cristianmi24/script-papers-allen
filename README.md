# Anonymized supplement

Four self-contained Colab notebooks; each writes the scripts it needs (`%%writefile`) and then runs them. Run in order:

1. `01_descarga_datos.ipynb` – Allen Visual Behavior download (training sessions, running speed, pupil of the same mice). Python 3.10 + allensdk, pynwb==2.5.0, hdmf==3.9.0 (cell A builds it).
2. `02_simulaciones.ipynb` – recovery, volatility, prior sensitivity, sample size, oracle gap, power analysis (no real data).
3. `03_analisis_real.ipynb` – 27 mice: DMA/TD/PH, choice kernel, episodic, HMM, value+CK, latency test.
4. `04_arousal_y_figuras.ipynb` – running speed and pupil tests (with post hoc slow controls) and figures.

`sessions_used.csv` / `sessions_pupil.csv`: Allen behavior-session IDs analyzed (behavior / imaging). `resultados/`: JSON/CSV results reported in the paper. Seeds are fixed in the scripts. Requirements for 2-4: numpy, scipy, pandas, numba, matplotlib.
