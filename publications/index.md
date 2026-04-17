---
layout: default
title: Publications
permalink: /publications/
---

<h1>Publications</h1>

<!-- FILTER BUTTONS -->
<div class="filter-bar">
  <button onclick="filterPubs('all')">All</button>
  <button onclick="filterPubs('journal')">Journals</button>
  <button onclick="filterPubs('conference')">Conferences</button>
  <button onclick="filterPubs('preprint')">Preprints</button>
  <button onclick="filterPubs('thesis')">Theses</button>
</div>

<style>
.filter-bar {
  margin-bottom: 25px;
}

.filter-bar button {
  margin-right: 6px;
  margin-bottom: 6px;
  padding: 6px 10px;
  border: 1px solid #ccc;
  background: #f8f8f8;
  cursor: pointer;
  border-radius: 6px;
}

.pub {
  display: flex;
  justify-content: space-between;
  gap: 18px;
  padding: 16px 0;
  border-bottom: 1px solid #eee;
}

.pub-left {
  flex: 1;
}

.pub-title {
  color: teal;
  font-weight: 600;
}

.pub-meta {
  font-size: 0.9em;
  color: #444;
}

.tag {
  display: inline-block;
  font-size: 0.75em;
  color: purple;
  border: 1px solid #ddd;
  padding: 2px 6px;
  border-radius: 5px;
  margin-left: 6px;
}

.pub img {
  width: 85px;
  height: 85px;
  object-fit: cover;
  border-radius: 8px;
  border: 1px solid #ddd;
}

details {
  margin-top: 6px;
  font-size: 0.9em;
}
</style>

<script>
function filterPubs(type) {
  let pubs = document.getElementsByClassName("pub");

  for (let i = 0; i < pubs.length; i++) {
    if (type === "all") {
      pubs[i].style.display = "flex";
    } else {
      pubs[i].style.display = pubs[i].classList.contains(type) ? "flex" : "none";
    }
  }
}
</script>

<!-- ========================= -->
<!-- JOURNAL PAPERS -->
<!-- ========================= -->

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">Comparing Machine Learning Algorithms by Union-Free Generic Depth</div>
    <div class="pub-meta">International Journal of Approximate Reasoning (2024)</div>
    <span class="tag">SJR Q1/Q2</span>

    <details>
      <summary>Abstract</summary>
      We propose a depth-based framework for comparing machine learning algorithms under uncertainty.
    </details>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">Statistical Comparisons of Classifiers by Generalized Stochastic Dominance</div>
    <div class="pub-meta">Journal of Machine Learning Research (2023)</div>
    <span class="tag">SJR Q1</span>

    <details>
      <summary>Abstract</summary>
      We introduce generalized stochastic dominance as a method for comparing classifiers statistically.
    </details>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3f/JMLR_logo.svg">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">Risk Aversion over Finite Domains</div>
    <div class="pub-meta">Theory and Decision (2022)</div>
    <span class="tag">SJR Q2</span>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<!-- ========================= -->
<!-- CONFERENCE PAPERS -->
<!-- ========================= -->

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">Statistical Multicriteria Benchmarking via the GSD-Front</div>
    <div class="pub-meta">NeurIPS 2024 (Spotlight)</div>
    <span class="tag">CORE A*</span>

    <details>
      <summary>Abstract</summary>
      We introduce a multicriteria benchmarking framework for machine learning evaluation.
    </details>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/96/NeurIPS_logo.svg">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">Reciprocal Learning</div>
    <div class="pub-meta">NeurIPS 2024</div>
    <span class="tag">CORE A*</span>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/96/NeurIPS_logo.svg">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">Robust statistical comparison of random variables</div>
    <div class="pub-meta">UAI 2023</div>
    <span class="tag">CORE A</span>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<!-- ========================= -->
<!-- PREPRINTS -->
<!-- ========================= -->

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title">Beyond Arrow: From Impossibility to Possibilities in Multi-Criteria Benchmarking</div>
    <div class="pub-meta">arXiv (2026)</div>

    <details>
      <summary>Abstract</summary>
      We extend Arrow-type impossibility results into constructive benchmarking frameworks.
    </details>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/8/87/Arxiv_logo_2022.svg">
</div>

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title">A Statistical Case Against Empirical Human–AI Alignment</div>
    <div class="pub-meta">arXiv (2026)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/8/87/Arxiv_logo_2022.svg">
</div>

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title">Empirical Decision Theory</div>
    <div class="pub-meta">arXiv (under review)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/8/87/Arxiv_logo_2022.svg">
</div>

<!-- ========================= -->
<!-- THESES -->
<!-- ========================= -->

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title">Habilitation Thesis</div>
    <div class="pub-meta">LMU Munich (2024)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/1b/Graduation_cap_icon.svg">
</div>

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title">PhD Thesis</div>
    <div class="pub-meta">LMU Munich (2018)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/1b/Graduation_cap_icon.svg">
</div>
