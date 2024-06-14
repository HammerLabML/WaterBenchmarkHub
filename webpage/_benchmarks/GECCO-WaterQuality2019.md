---
title: "GECCO Industrial Challenge 2019 Dataset"
id: "gecco-waterquality2019"
permalink: /benchmarks/GECCO-WaterQuality2019.html
collection: benchmarks
layout: benchmark
---

## Description

The GECCO Industrial Challenge 2019 Dataset: A water quality dataset for the "Internet of Things:
Online Event Detection for Drinking Water Quality Control" competition organized by F. Rehbach,
S. Moritz, T. Bartz-Beielstein at the Genetic and Evolutionary Computation Conference 2019,
Prague, Czech Republic.

The data is provided by the "Thüringer Fernwasserversorgung" (Germany) and
constitutes a real-world data set.
In this data set, 6 numeric water quality features are given at a sampling rate of 1 min
over approx. 3 month.
The goal is to predict the presence of an anomaly -- i.e. binary classification.
The data set itself comes in three splits: A train set, a validation set, and a test set.

## How to Use

- **Training data:** `7_gecco2019_train_water_quality.csv`
- **Validation data:** `8_gecco2019_valid_water_qulity.csv`
- **Test data:** `6_gecco2019_test_water_quality.csv`


| Column  | Description                                                                                      |
|---------|--------------------------------------------------------------------------------------------------|
| `Time`  | Time of measurement, given in following format: yyyy-mm-dd HH:MM:SS                              |
| `Tp`    | The temperature of the water, given in °C.                                                       |
| `pH`    | pH value of the water.                                                                           |
| `Cond`  | Electric conductivity of the water, given in S/m.                                                |
| `Turb`  | Turbidity of the water, given in FNU.                                                            |
| `SAC`   | Spectral absorption coefficient, given in 1/m.                                                   |
| `PFM`   | Pulse-Frequency-Modulation, given in Hz.                                                         |
| `EVENT` | Marker if this entry should be considered as a remarkable change resp. event, given in boolean.  |


### Usage in Python

This benchmark is also available in Python in the GECCO water quality collection (key: *GECCO-WaterQuality*)
through the
[```load_gecco2019_water_quality_data()```](https://water-benchmark-hub.readthedocs.io/en/stable/water_benchmark_hub.gecco_waterquality.html#water_benchmark_hub.gecco_waterquality.gecco_water_quality.GeccoWaterQuality.load_gecco2019_water_quality_data)
function:
```python
# Load GECCO water quality benchmark
benchmark = load("GECCO-WaterQuality")

# Load 2019 data set
data = benchmark.load_gecco2019_water_quality_data(return_X_y=True)

# Show number of samples
X_train, y_train = data["train"]
X_val, y_val = data["validation"]
X_test, y_test = data["test"]
print(X_train.shape, X_val.shape, X_test.shape)
```

## Reference

Moritz, S., Rehbach, F., & Bartz-Beielstein, T. (2019). *GECCO Industrial Challenge 2019 Dataset:
A water quality dataset for the 'Internet of Things: Online Event Detection for Drinking Water Quality Control'*
competition at the Genetic and Evolutionary Computation Conference 2019, Prague, Czech Republic.