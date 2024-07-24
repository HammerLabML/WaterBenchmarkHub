---
title: "KY5"
id: "network-ky5"
permalink: /benchmarks/network-KY5.html
collection: benchmarks
layout: benchmark
---


## Description

The KY 5 system is based on a real-world system in KY and was originally used by Jolly et al. in 2014 as part of a
classification study. The system has a total demand of 2.28 MGD, four reservoirs, two tanks, nine pumps, and 52.3 miles
of pipe. It is classified as distribution sparse-grid by Hwang & Lansey (2017) and looped by Hoagland et al. (2015).

It was published 2016 by University of Kentucky Libraries.

The network consists of 402 nodes (junctions), 496 pipes, 3 tanks, 9 pumps and 4 reservoirs.

<img src="../static/benchmarks/network-ky5/ky5_plot.png"/>

## How to Use

The KY5 network is provided as an .inp file and can be loaded into EPANET or any other software package
supporting .inp files.

### Usage in Python

The KY5 network is also available in Python through the key "*Network-KY5*":
```python
network = load("Network-KY5")
ky5_inp = network.load()
```

Detailed information about the provided functionality can be found in the documentation of
[`load()`](https://water-benchmark-hub.readthedocs.io/en/stable/water_benchmark_hub.networks.html#water_benchmark_hub.networks.networks.KY5.load).


## Reference

Hoagland, Steven, "05 KY 5" (2016). Kentucky Dataset. 7.
https://uknowledge.uky.edu/wdst/7

Jolly, M. D., Lothes, A. D., Bryson, L. S., & Ormsbee, L. (2014). Research Database of Water Distribution System Models.
Journal of Water Resources Planning and Management, 410-416. 10.1061/(ASCE)WR.1943-5452.0000352