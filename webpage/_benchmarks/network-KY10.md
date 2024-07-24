---
title: "KY10"
id: "network-ky10"
permalink: /benchmarks/network-KY10.html
collection: benchmarks
layout: benchmark
---


## Description

The KY 10 system is based on a real-world system in KY and was originally used by Jolly et al. in 2014 as part of a
classification study. The system has a total demand of 2.26 MGD, two reservoirs, 13 tanks, 13 pumps, and 256 miles of
pipe. It is classified as distribution hybrid by Hwang & Lansey (2017) and gridded by Hoagland et al. (2015).

It was published 2016 by University of Kentucky Libraries.

The network consists of 884 nodes (junctions), 1043 pipes, 13 tanks, 13 pumps and 2 reservoirs.

<img src="../static/benchmarks/network-ky10/ky10_plot.png"/>

## How to Use

The KY10 network is provided as an .inp file and can be loaded into EPANET or any other software package
supporting .inp files.

### Usage in Python

The KY10 network is also available in Python through the key "*Network-KY10*":
```python
network = load("Network-KY10")
ky10_inp = network.load()
```

Detailed information about the provided functionality can be found in the documentation of
[`load()`](https://water-benchmark-hub.readthedocs.io/en/stable/water_benchmark_hub.networks.html#water_benchmark_hub.networks.networks.KY10.load).


## Reference

Hoagland, Steven, "10 KY 10" (2016). Kentucky Dataset. 12.
https://uknowledge.uky.edu/wdst/12

Jolly, M. D., Lothes, A. D., Bryson, L. S., & Ormsbee, L. (2014). Research Database of Water Distribution System Models.
Journal of Water Resources Planning and Management, 410-416. 10.1061/(ASCE)WR.1943-5452.0000352