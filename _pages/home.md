---
layout: splash
permalink: /
hidden: true
title: Tracking Evolving AI and Systems
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/alina-grubnyak-ZiQkhI7417A-unsplash.jpg
excerpt:  Uniting Models, Algorithms, and System Innovators with Top-Down Evolutionary Benchmarks.

feature_row:
  - image_path: /assets/images/michael-dziedzic-aQYgUYwnCsM-unsplash.jpg
    alt: "Hardware"
    title: "Hardware Landscape"
    excerpt: "Explore the landscape of hardware."
    url: "/hardware/"
    btn_class: "btn--primary"
    btn_label: "Explore Hardware"
  - image_path: /assets/images/open-clip-art-j9BIoxEpWKM-unsplash.jpg
    alt: "ML Models"
    title: "ML Models"
    excerpt: "Discover ML models."
    url: "/models/"
    btn_class: "btn--primary"
    btn_label: "Explore ML Models"
  - image_path: /assets/images/chris-liverani-dBI_My696Rk-unsplash.jpg
    alt: "Benchmarks"
    title: "Benchmarks"
    excerpt: "Investigate our benchmarks"
    url: "/benchmarks/"
    btn_class: "btn--primary"
    btn_label: "Explore Results"

--- 

{% include feature_row %}    


<div style="text-align: left; display: grid; grid-template-columns: 1fr 0.1fr 1fr;">
  <div>
  <h1>Our Goal</h1>
  We aim to create a suite of next-generation benchmarks that track the fast-evolving landscape of AI, and measure the complex trade-offs across costs, accuracy, and performance on a range of state-of-the-art hardware.
  </div>
  <div>
  </div>
  <div>
  <h1>Our Approach</h1>
  Our approach is informed by two selection maps (one for models and the other for systems), with a broad team with extensive expertise in AI research and practice – a combination that allows for rapid evolution of the benchmarks.
  </div>
</div>


## CAP Results

<script type="text/javascript">
function setPicture() {
    var img = document.getElementById("results1").src;
    var valueM = Modeldropdown.options[Modeldropdown.selectedIndex].value;
    var valueD = Datasetdropdown.options[Datasetdropdown.selectedIndex].value;
    var valueH = Hardwaredropdown.options[Hardwaredropdown.selectedIndex].value;

    if(Modeldropdown.selectedIndex == 0)
    {
        document.getElementById("results1").src = "/assets/diagrams/Qwen3-235B-A22B_radar.html";
    } else {
        document.getElementById("results1").src = "/assets/diagrams/Qwen3-30B-A3B_radar.html";
    }
}
</script>


<div class="row">

<select id="Modeldropdown" onchange="setPicture()">
    <option value="Qwen3-235B-A22B" selected>Qwen3-235B-A22B</option>
    <option value="Qwen3-30B-A3B">Qwen3-30B-A3B</option>
</select>

<select id="Datasetdropdown" onchange="setPicture()">
    <option value="GSM8K" selected>GSM8K</option>
</select>

<select id="Hardwaredropdown" onchange="setPicture()">
    <option value="H100-HBM3-80GB" selected>H100-HBM3-80GB</option>
    <option value="4xRTX-A6000-48GB">4xRTX-A6000-48GB</option>
</select>
</div>

<div>
<iframe id="results1" src="/assets/diagrams/Qwen3-235B-A22B_radar.html" width="150%" height="800px" frameborder="0"></iframe>
</div>