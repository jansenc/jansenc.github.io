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
</div>

<style>
.filter-bar {
  margin-bottom: 20px;
}

.filter-bar button {
  margin-right: 8px;
  padding: 6px 10px;
  border: 1px solid #ccc;
  background: #f8f8f8;
  cursor: pointer;
  border-radius: 6px;
}

.pub {
  display: flex;
  justify-content: space-between;
  gap: 15px;
  padding: 15px 0;
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
  font-size: 0.85em;
  color: #666;
}

.pub-tags {
  font-size: 0.75em;
  color: purple;
}

.pub img {
  width: 90px;
  height: 90px;
  object-fit: cover;
  border-radius: 8px;
  border: 1px solid #ddd;
}

details {
  margin-top: 6px;
  font-size: 0.9em;
}

.hidden {
  display: none;
}
</style>

<!-- PUBLICATION LIST -->

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">Statistical Multicriteria Benchmarking via the GSD-Front</div>
    <div class="pub-meta">NeurIPS 2024 (Spotlight)</div>
    <div class="pub-tags">CORE A*</div>

    <details>
      <summary>Abstract</summary>
      Method for comparing machine learning algorithms via statistical multicriteria evaluation...
    </details>
  </div>
  <img src="https://via.placeholder.com/90" alt="paper image">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">Statistical Comparisons of Classifiers by Generalized Stochastic Dominance</div>
    <div class="pub-meta">JMLR 2023</div>

    <details>
      <summary>Abstract</summary>
      We introduce a framework for comparing classifiers using stochastic dominance...
    </details>
  </div>
  <img src="https://via.placeholder.com/90" alt="paper image">
</div>

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title">Beyond Arrow: From Impossibility to Possibilities in Multi-Criteria Benchmarking</div>
    <div class="pub-meta">Preprint (2026)</div>

    <details>
      <summary>Abstract</summary>
      This work generalizes Arrow-type impossibility results into constructive benchmarking settings...
    </details>
  </div>
  <img src="https://via.placeholder.com/90" alt="paper image">
</div>

<!-- JS FILTER -->
<script>
function filterPubs(type) {
  let pubs = document.getElementsByClassName("pub");

  for (let i = 0; i < pubs.length; i++) {
    if (type === "all") {
      pubs[i].style.display = "flex";
    } else {
      if (pubs[i].classList.contains(type)) {
        pubs[i].style.display = "flex";
      } else {
        pubs[i].style.display = "none";
      }
    }
  }
}
</script>
