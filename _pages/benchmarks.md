---
permalink: /benchmarks/
title: "Benchmarks"
layout: categories
---

### Model Selection

![image](/assets/diagrams/model_selection_map2.svg)

### Benchmark selection

![image](/assets/diagrams/benchmark_map.svg)


### Benchmark implementation

![image](/assets/diagrams/benchmark_impl.svg)

### CAP Results
1. Model: Qwen3-30B-A3B; \
Dataset: GSM8K; \
Hardware: 4xRTX-A6000-48GB; \
Config: TP=4
<iframe src="/assets/diagrams/Qwen3-30B-A3B_radar.html" width="150%" height="800px" frameborder="0"></iframe>

2. Model: Qwen3-235B-A22B; \
Dataset: GSM8K; \
Hardware: H100-HBM3-80GB; \
Config: BF16-TP=8; FP8-TP=4; AWQ-TP=4;
<iframe src="/assets/diagrams/Qwen3-235B-A22B_radar.html" width="150%" height="800px" frameborder="0"></iframe>