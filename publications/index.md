---
layout: default
title: Publications
permalink: /publications/
---

<h1>Publications</h1>

<!-- ================= FILTERS ================= -->
<div class="filter-bar">
  <button onclick="filterPubs('all')">All</button>
  <button onclick="filterPubs('journal')">Journals</button>
  <button onclick="filterPubs('conference')">Conferences</button>
  <button onclick="filterPubs('preprint')">Preprints</button>
  <button onclick="filterPubs('book')">Book Chapters</button>
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
  padding: 18px 0;
  border-bottom: 1px solid #eee;
}

.pub-left {
  flex: 1;
}

.pub-title {
  font-weight: 600;
  color: teal;
  font-size: 1.05em;
}

.pub-meta {
  font-size: 0.9em;
  color: #555;
}

.tag {
  display: inline-block;
  font-size: 0.75em;
  color: purple;
  border: 1px solid #ddd;
  padding: 2px 6px;
  border-radius: 5px;
  margin-top: 4px;
  margin-right: 5px;
}

.pub img {
  width: 85px;
  height: 85px;
  object-fit: contain;
  border-radius: 8px;
  border: 1px solid #eee;
  background: white;
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

<!-- ===================================================== -->
<!-- ===================== JOURNALS ======================= -->
<!-- ===================================================== -->

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">Comparing Machine Learning Algorithms by Union-Free Generic Depth</div>
    <div class="pub-meta">International Journal of Approximate Reasoning (2024)</div>
    <span class="tag">SJR Q1/Q2</span>

    <details><summary>Abstract</summary>
      We propose a framework for descriptively analyzing sets of partial orders based on the concept of depth functions. Despite intensive studies in linear and metric spaces, there is very little discussion on depth functions for non-standard data types such as partial orders. We introduce an adaptation of the well-known simplicial depth to the set of all partial orders, the union-free generic (ufg) depth. Moreover, we utilize our ufg depth for a comparison of machine learning algorithms based on multidimensional performance measures. Concretely, we provide two examples of classifier comparisons on samples of standard benchmark data sets. Our results demonstrate promisingly the wide variety of different analysis approaches based on ufg methods. Furthermore, the examples outline that our approach differs substantially from existing benchmarking approaches, and thus adds a new perspective to the vivid debate on classifier comparison.
    </details>
  </div>
  <img src="src="/assets/ijar.jpg">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">Statistical Comparisons of Classifiers by Generalized Stochastic Dominance</div>
    <div class="pub-meta">Journal of Machine Learning Research (2023)</div>
    <span class="tag">SJR Q1</span>

    <details><summary>Abstract</summary>
      Generalized stochastic dominance framework for classifier comparison.
    </details>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3f/JMLR_logo.svg">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">Information Efficient Learning of Complexly Structured Preferences</div>
    <div class="pub-meta">International Journal of Approximate Reasoning (2022)</div>
    <span class="tag">SJR Q1/Q2</span>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">Risk Aversion over Finite Domains</div>
    <div class="pub-meta">Theory and Decision (2022)</div>
    <span class="tag">SJR Q2</span>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">Concepts for Decision Making under Severe Uncertainty</div>
    <div class="pub-meta">International Journal of Approximate Reasoning (2018)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">A Probabilistic Evaluation Framework for Preference Aggregation</div>
    <div class="pub-meta">Mathematical Social Sciences (2018)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<!-- ===================================================== -->
<!-- ================= CONFERENCES ======================= -->
<!-- ===================================================== -->

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">Statistical Multicriteria Benchmarking via the GSD-Front</div>
    <div class="pub-meta">NeurIPS 2024 (Spotlight)</div>
    <span class="tag">CORE A*</span>

    <details><summary>Abstract</summary>
      Multicriteria benchmarking framework for ML evaluation.
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
    <div class="pub-title">Robust Statistical Comparison of Random Variables</div>
    <div class="pub-meta">UAI 2023</div>
    <span class="tag">CORE A</span>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">Depth Functions for Partial Orders</div>
    <div class="pub-meta">ISIPTA 2023</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">Robust Selection of Pseudo-Labeled Data</div>
    <div class="pub-meta">ISIPTA 2023</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">Multi-target Decision Making under Severe Uncertainty</div>
    <div class="pub-meta">MDAI 2023</div>
    <span class="tag">CORE B</span>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">Decision Theory Meets Linear Optimization</div>
    <div class="pub-meta">ECSQARU 2017</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<!-- ===================================================== -->
<!-- ================= PREPRINTS ========================= -->
<!-- ===================================================== -->

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title">Empirical Decision Theory</div>
    <div class="pub-meta">arXiv (2026)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/8/87/Arxiv_logo_2022.svg">
</div>

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title">Beyond Arrow: From Impossibility to Possibilities in Multi-Criteria Benchmarking</div>
    <div class="pub-meta">arXiv (2026)</div>
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

<!-- ===================================================== -->
<!-- ================= BOOK CHAPTERS ===================== -->
<!-- ===================================================== -->

<div class="pub book">
  <div class="pub-left">
    <div class="pub-title">Quantifying Degrees of E-admissibility</div>
    <div class="pub-meta">Theory and Decision Library A (2022)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Research_icon.png">
</div>

<!-- ===================================================== -->
<!-- ================= THESES ============================= -->
<!-- ===================================================== -->

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title">Habilitation Thesis (2024)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/1b/Graduation_cap_icon.svg">
</div>

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title">PhD Thesis (2018)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/1b/Graduation_cap_icon.svg">
</div>

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title">Master Thesis (2015)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/1b/Graduation_cap_icon.svg">
</div>

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title">Bachelor Thesis (2013)</div>
  </div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/1b/Graduation_cap_icon.svg">
</div>
