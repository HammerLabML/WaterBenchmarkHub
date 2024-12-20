---
title: "KYV21"
id: "network-kyv21"
permalink: /benchmarks/network-KYV21.html
collection: benchmarks
layout: benchmark
---


## Description

The KY V21 system is based on a real-world system in KY and was originally used by Hernandez & Ormsbee in 2020 as part
of a classification study. The system has a total demand of 0.88 MGD, one reservoir, 11 tanks, 16 pump, and 293 miles of
pipe. It is classified as distribution hybrid by Hwang & Lansey (2017) and looped by Hoagland et al. (2015).

It was published 2021 by University of Kentucky Libraries.

The network consists of 1014 nodes (junctions), 1078 pipes, 204 valves, 11 tanks, 21 pumps and 1 reservoir.

<img src="../static/benchmarks/network-kyv21/kyv21_plot.png" width="100%"/>

## How to Use

The KYV21 network is provided as an .inp file and can be loaded into EPANET or any other software package
supporting .inp files.

### Usage in Python

The KYV21 network is also available in Python through the key "*Network-KYV21*":
```python
network = load("Network-KYV21")
kyv21_inp = network.load()
```

Detailed information about the provided functionality can be found in the documentation of
[`load()`](https://waterbenchmarkhub.readthedocs.io/en/latest/water_benchmark_hub.networks.html#water_benchmark_hub.networks.networks.KYV21.load).


## Reference

Hernandez Hernandez, Erika, "06 KY V21" (2021). Kentucky Valved Dataset. 6.
[<i class="bi bi-link"></i>](https://uknowledge.uky.edu/wdst_ky_valved/6)

Hernandez Hernandez, Erika, and Ormsbee, Lindell. "*Segment-Based Assessment of Consequences of Failure on Water
Distribution Systems.*" Journal of Water Resources Planning and Management 147.4 (2021): 04021009.
10.1061/(ASCE)WR.1943-5452.0001340
[<i class="bi bi-link"></i>](https://doi.org/10.1061/(ASCE)WR.1943-5452.0001340)
