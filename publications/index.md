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
  font-size: 0.85em;
  color: #666;
}

.pub-tags {
  font-size: 0.75em;
  color: purple;
  margin-top: 3px;
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

.hidden {
  display: none;
}
</style>

<!-- ===================== -->
<!-- TEMPLATE BLOCK -->
<!-- ===================== -->

<!-- JOURNAL PAPER -->
<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title">TITLE HERE</div>
    <div class="pub-meta">AUTHORS (YEAR), JOURNAL NAME</div>
    <div class="pub-tags">SJR / CATEGORY TAGS</div>

    <details>
      <summary>Abstract</summary>
      ABSTRACT TEXT HERE
    </details>
  </div>
  <img src="https://via.placeholder.com/85" alt="paper image">
</div>

<!-- CONFERENCE PAPER -->
<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title">TITLE HERE</div>
    <div class="pub-meta">AUTHORS (YEAR), CONFERENCE</div>
    <div class="pub-tags">CORE RANK</div>

    <details>
      <summary>Abstract</summary>
      ABSTRACT TEXT HERE
    </details>
  </div>
  <img src="https://via.placeholder.com/85" alt="paper image">
</div>

<!-- PREPRINT -->
<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title">TITLE HERE</div>
    <div class="pub-meta">AUTHORS (YEAR), PREPRINT</div>

    <details>
      <summary>Abstract</summary>
      ABSTRACT TEXT HERE
    </details>
  </div>
  <img src="https://via.placeholder.com/85" alt="paper image">
</div>

<!-- BOOK CHAPTER -->
<div class="pub book">
  <div class="pub-left">
    <div class="pub-title">TITLE HERE</div>
    <div class="pub-meta">BOOK TITLE / EDITORS / YEAR</div>

    <details>
      <summary>Abstract</summary>
      ABSTRACT OR DESCRIPTION HERE
    </details>
  </div>
  <img src="https://via.placeholder.com/85" alt="book cover">
</div>

<!-- THESIS -->
<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title">TITLE HERE</div>
    <div class="pub-meta">TYPE OF THESIS (PhD / MSc / BSc), UNIVERSITY, YEAR</div>

    <details>
      <summary>Abstract</summary>
      ABSTRACT OR SUMMARY HERE
    </details>
  </div>
  <img src="https://via.placeholder.com/85" alt="thesis image">
</div>

<!-- FILTER SCRIPT -->
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
