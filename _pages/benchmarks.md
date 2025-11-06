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

<script type="text/javascript">
function setPicture() {
    var img = document.getElementById("results").src;
    var valueM = Modeldropdown.options[Modeldropdown.selectedIndex].value;
    var valueD = Datasetdropdown.options[Datasetdropdown.selectedIndex].value;
    var valueH = Hardwaredropdown.options[Hardwaredropdown.selectedIndex].value;

    if(Modeldropdown.selectedIndex == 0)
    {
        document.getElementById("results").src = "/assets/diagrams/Qwen3-235B-A22B_radar.html";
    } else {
        document.getElementById("results").src = "/assets/diagrams/Qwen3-30B-A3B_radar.html";
    }
}
</script>


<div class="row">

<label for="Models">Model</label>
<select id="Modeldropdown" onchange="setPicture()">
    <option value="Qwen3-235B-A22B" selected>Qwen3-235B-A22B</option>
    <option value="Qwen3-30B-A3B">Qwen3-30B-A3B</option>
</select>

<select id="Datasetdropdown" onchange="setPicture()">
    <option value="GSM8K" selected>GSM8K</option>
</select>

<select id="Hardwaredropdown" onchange="setPicture()">
    <option value="H100-HBM3-80GB" selected>H100-HBM3-80GB</option>
    <option value="4xRTX-A6000-48GB" selected>4xRTX-A6000-48GB</option>
</select>
</div>


<iframe id="results" src="/assets/diagrams/Qwen3-30B-A3B_radar.html" width="150%" height="800px" frameborder="0"></iframe>

