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
    <div class="pub-title"><b><a href="https://doi.org/10.1016/j.ijar.2024.109166" class="paper-link">Comparing Machine Learning Algorithms by Union-Free Generic Depth</a></b></div>
    <div class="pub-meta">International Journal of Approximate Reasoning (2024)</div>
    <span class="tag">SJR Q1/Q2</span>

    <details><summary>Abstract</summary>
      We propose a framework for descriptively analyzing sets of partial orders based on the concept of depth functions. Despite intensive studies in linear and metric spaces, there is very little discussion on depth functions for non-standard data types such as partial orders. We introduce an adaptation of the well-known simplicial depth to the set of all partial orders, the union-free generic (ufg) depth. Moreover, we utilize our ufg depth for a comparison of machine learning algorithms based on multidimensional performance measures. Concretely, we provide two examples of classifier comparisons on samples of standard benchmark data sets. Our results demonstrate promisingly the wide variety of different analysis approaches based on ufg methods. Furthermore, the examples outline that our approach differs substantially from existing benchmarking approaches, and thus adds a new perspective to the vivid debate on classifier comparison.
    </details>
  </div>
  <img src="/assets/ijar.jpg">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://jmlr.org/papers/v24/22-0902.html" class="paper-link">Statistical Comparisons of Classifiers by Generalized Stochastic Dominance</a></b></div>
    <div class="pub-meta">Journal of Machine Learning Research (2023)</div>
    <span class="tag">SJR Q1</span>

    <details><summary>Abstract</summary>
      Although being a crucial question for the development of machine learning algorithms, there is still no consensus on how to compare classifiers over multiple data sets with respect to several criteria. Every comparison framework is confronted with (at least) three fundamental challenges: the multiplicity of quality criteria, the multiplicity of data sets and the randomness of the selection of data sets. In this paper, we add a fresh view to the vivid debate by adopting recent developments in decision theory. Based on so-called preference systems, our framework ranks classifiers by a generalized concept of stochastic dominance, which powerfully circumvents the cumbersome, and often even self-contradictory, reliance on aggregates. Moreover, we show that generalized stochastic dominance can be operationalized by solving easy-to-handle linear programs and moreover statistically tested employing an adapted two-sample observation-randomization test. This yields indeed a powerful framework for the statistical comparison of classifiers over multiple data sets with respect to multiple quality criteria simultaneously. We illustrate and investigate our framework in a simulation study and with a set of standard benchmark data sets.
    </details>
  </div>
  <img src="/assets/jmlr.jpg">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://doi.org/10.1016/j.ijar.2022.01.016" class="paper-link">Information efficient learning of complexly structured preferences: Elicitation procedures and their application to decision making under uncertainty</a></b></div>
    <div class="pub-meta">International Journal of Approximate Reasoning (2022)</div>
    <span class="tag">SJR Q1/Q2</span>

    <details><summary>Abstract</summary>
      In this paper we propose efficient methods for elicitation of complexly structured preferences and utilize these in problems of decision making under (severe) uncertainty. Based on the general framework introduced in Jansen et al. (2018) [37], we now design elicitation procedures and algorithms that enable decision makers to reveal their underlying preference system (i.e. two relations, one encoding the ordinal, the other the cardinal part of the preferences) while having to answer as few as possible simple ranking questions. Here, two different approaches are followed. The first approach directly utilizes the collected ranking data for obtaining the ordinal part of the preferences, while their cardinal part is constructed implicitly by measuring the decision maker's consideration times. In contrast, the second approach explicitly elicits also the cardinal part of the decision maker's preference system, however, only an approximate version of it. This approximation is obtained by additionally collecting labels of preference strength during the elicitation procedure. For both approaches, we give conditions under which they produce the decision maker's true preference system and investigate how their efficiency can be improved. For the latter purpose, besides data-free approaches, we also discuss ways for statistically guiding the elicitation procedure if data from elicitations of previous decision makers is available. Finally, we demonstrate how the proposed elicitation methods can be utilized in problems of decision under (severe) uncertainty. Precisely, we show that under certain conditions optimal decisions can be found without fully specifying the preference system.
    </details>
  </div>
  <img src="/assets/ijar.jpg">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://link.springer.com/article/10.1007/s11238-021-09847-8" class="paper-link">Risk Aversion over Finite Domains</a></b></div>
    <div class="pub-meta">Theory and Decision (2022)</div>
    <span class="tag">SJR Q2</span>

    <details><summary>Abstract</summary>
     We investigate risk attitudes when the underlying domain of payoffs is finite and the payoffs are, in general, not numerical. In such cases, the traditional notions of absolute risk attitudes, that are designed for convex domains of numerical payoffs, are not applicable. We introduce comparative notions of weak and strong risk attitudes that remain applicable. We examine how they are characterized within the rank-dependent utility model, thus including expected utility as a special case. In particular, we characterize strong comparative risk aversion under rank-dependent utility. This is our main result. From this and other findings, we draw two novel conclusions. First, under expected utility, weak and strong comparative risk aversion are characterized by the same condition over finite domains. By contrast, such is not the case under non-expected utility. Second, under expected utility, weak (respectively: strong) comparative risk aversion is characterized by the same condition when the utility functions have finite range and when they have convex range (alternatively, when the payoffs are numerical and their domain is finite or convex, respectively). By contrast, such is not the case under non-expected utility. Thus, considering comparative risk aversion over finite domains leads to a better understanding of the divide between expected and non-expected utility, more generally, the structural properties of the main models of decision-making under risk.
    </details>
  </div>
  <img src="/assets/11238.webp">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://doi.org/10.1016/j.ijar.2018.04.011" class="paper-link">Concepts for decision making under severe uncertainty with partial ordinal and partial cardinal preferences</a></b></div>
    <div class="pub-meta">International Journal of Approximate Reasoning (2018)</div>
<span class="tag">SJR Q1/Q2</span>

    <details><summary>Abstract</summary>
      We introduce three different approaches for decision making under uncertainty if (I) there is only partial (both cardinally and ordinally scaled) information on an agent's preferences and (II) the uncertainty about the states of nature is described by a credal set (or some other imprecise probabilistic model). Particularly, situation (I) is modeled by a pair of binary relations, one specifying the partial rank order of the alternatives and the other modeling partial information on the strength of preference. Our first approach relies on decision criteria constructing complete rankings of the available acts that are based on generalized expectation intervals. Subsequently, we introduce different concepts of global admissibility that construct partial orders between the available acts by comparing them all simultaneously. Finally, we define criteria induced by suitable binary relations on the set of acts and, therefore, can be understood as concepts of local admissibility. For certain criteria, we provide linear programming based algorithms for checking optimality/admissibility of acts. Additionally, the paper includes a discussion of a prototypical situation by means of a toy example.
    </details>
    
  </div>
  <img src="/assets/ijar.jpg">
</div>

<div class="pub journal">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://doi.org/10.1016/j.mathsocsci.2018.09.001" class="paper-link">A probabilistic evaluation framework for preference aggregation reflecting group homogeneity</a></b></div>
    <div class="pub-meta">Mathematical Social Sciences (2018)</div>
   <span class="tag">SJR Q2</span>

    <details><summary>Abstract</summary>
      Groups differ in the homogeneity of their members’ preferences. Reflecting this, we propose a probabilistic criterion for evaluating and comparing the adequateness of preference aggregation procedures that takes into account information on the considered group’s homogeneity structure. Further, we discuss two approaches for approximating our criterion if information is only imperfectly given and show how to estimate these approximations from data. As a preparation, we elaborate some general minimal requirements for measuring homogeneity and discuss a specific proposal for a homogeneity measure. Finally, we investigate our framework by comparing aggregation rules in a simulation study.
        </details>
    
  </div>
  <img src="/assets/mss.jpg">
</div>

<!-- ===================================================== -->
<!-- ================= CONFERENCES ======================= -->
<!-- ===================================================== -->

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://proceedings.neurips.cc/paper_files/paper/2024/hash/b1f140eeee243db24e9e006481b91cf1-Abstract-Conference.html" class="paper-link">Statistical Multicriteria Benchmarking via the GSD-Front</a></b></div>
    <div class="pub-meta">NeurIPS 2024 (Spotlight)</div>
    <span class="tag">CORE A*</span>

    <details><summary>Abstract</summary>
      Given the vast number of classifiers that have been (and continue to be) proposed, reliable methods for comparing them are becoming increasingly important. The desire for reliability is broken down into three main aspects: (1) Comparisons should allow for different quality metrics simultaneously. (2) Comparisons should take into account the statistical uncertainty induced by the choice of benchmark suite. (3) The robustness of the comparisons under small deviations in the underlying assumptions should be verifiable. To address (1), we propose to compare classifiers using a generalized stochastic dominance ordering (GSD) and present the GSD-front as an information-efficient alternative to the classical Pareto-front. For (2), we propose a consistent statistical estimator for the GSD-front and construct a statistical test for whether a (potentially new) classifier lies in the GSD-front of a set of state-of-the-art classifiers. For (3), we relax our proposed test using techniques from robust statistics and imprecise probabilities. We illustrate our concepts on the benchmark suite PMLB and on the platform OpenML.
    </details>
  </div>
  <img src="/assets/nips.svg">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://proceedings.neurips.cc/paper_files/paper/2024/hash/0337b41b4e8b2eb5d7ab161ffd42cf3b-Abstract-Conference.html" class="paper-link">Reciprocal Learning</a></b></div>
    <div class="pub-meta">NeurIPS 2024</div>
    <span class="tag">CORE A*</span>

    <details><summary>Abstract</summary>
      We demonstrate that numerous machine learning algorithms are specific instances of one single paradigm: reciprocal learning. These instances range from active learning over multi-armed bandits to self-training. We show that all these algorithms not only learn parameters from data but also vice versa: They iteratively alter training data in a way that depends on the current model fit. We introduce reciprocal learning as a generalization of these algorithms using the language of decision theory. This allows us to study under what conditions they converge. The key is to guarantee that reciprocal learning contracts such that the Banach fixed-point theorem applies. In this way, we find that reciprocal learning converges at linear rates to an approximately optimal model under some assumptions on the loss function, if their predictions are probabilistic and the sample adaption is both non-greedy and either randomized or regularized. We interpret these findings and provide corollaries that relate them to active learning, self-training, and bandits.
    </details>
  </div>
  <img src="/assets/nips.svg">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://proceedings.mlr.press/v216/jansen23a.html" class="paper-link">Robust Statistical Comparison of Random Variables with Locally Varying Scale of Measurement</a></b></div>
    <div class="pub-meta">UAI 2023</div>
    <span class="tag">CORE A</span>

    <details><summary>Abstract</summary>
     Spaces with locally varying scale of measurement, like multidimensional structures with differently scaled dimensions, are pretty common in statistics and machine learning. Nevertheless, it is still understood as an open question how to exploit the entire information encoded in them properly. We address this problem by considering an order based on (sets of) expectations of random variables mapping into such non-standard spaces. This order contains stochastic dominance and expectation order as extreme cases when no, or respectively perfect, cardinal structure is given. We derive a (regularized) statistical test for our proposed generalized stochastic dominance (GSD) order, operationalize it by linear optimization, and robustify it by imprecise probability models. Our findings are illustrated with data from multidimensional poverty measurement, finance, and medicine.
    </details>
  </div>
  <img src="/assets/uai2023.png">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://proceedings.mlr.press/v215/blocher23a.html" class="paper-link">Depth functions for partial orders with a descriptive analysis of machine learning algorithms</a></b></div>
    <div class="pub-meta">ISIPTA 2023</div>

    <details><summary>Abstract</summary>
      We propose a framework for descriptively analyzing sets of partial orders based on the concept of depth functions. Despite intensive studies of depth functions in linear and metric spaces, there is very little discussion on depth functions for non-standard data types such as partial orders. We introduce an adaptation of the well-known simplicial depth to the set of all partial orders, the union-free generic (ufg) depth. Moreover, we utilize our ufg depth for a comparison of machine learning algorithms based on multidimensional performance measures. Concretely, we analyze the distribution of different classifier performances over a sample of standard benchmark data sets. Our results promisingly demonstrate that our approach differs substantially from existing benchmarking approaches and, therefore, adds a new perspective to the vivid debate on the comparison of classifiers.
    </details>
  </div>
  <img src="/assets/pmlr.svg">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://proceedings.mlr.press/v215/rodemann23a.html" class="paper-link">In all likelihoods: robust selection of pseudo-labeled data</a></b></div>
    <div class="pub-meta">ISIPTA 2023</div>

    <details><summary>Abstract</summary>
      Self-training is a simple yet effective method within semi-supervised learning. Self-training’s rationale is to iteratively enhance training data by adding pseudo-labeled data. Its generalization performance heavily depends on the selection of these pseudo-labeled data (PLS). In this paper, we render PLS more robust towards the involved modeling assumptions. To this end, we treat PLS as a decision problem, which allows us to introduce a generalized utility function. The idea is to select pseudo-labeled data that maximize a multi-objective utility function. We demonstrate that the latter can be constructed to account for different sources of uncertainty and explore three examples: model selection, accumulation of errors and covariate shift. In the absence of second-order information on such uncertainties, we furthermore consider the generic approach of the generalized Bayesian α
-cut updating rule for credal sets. We spotlight the application of three of our robust extensions on both simulated and three real-world data sets. In a benchmarking study, we compare these extensions to traditional PLS methods. Results suggest that robustness with regard to model choice can lead to substantial accuracy gains.
    </details>
  </div>
  <img src="/assets/pmlr.svg">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://link.springer.com/chapter/10.1007/978-3-031-33498-6_2" class="paper-link">Multi-target Decision Making Under Conditions of Severe Uncertainty</a></b></div>
    <div class="pub-meta">MDAI 2023</div>
    <span class="tag">CORE B</span>

    <details><summary>Abstract</summary>
     The quality of consequences in a decision making problem under (severe) uncertainty must often be compared among different targets (goals, objectives) simultaneously. In addition, the evaluations of a consequence’s performance under the various targets often differ in their scale of measurement, classically being either purely ordinal or perfectly cardinal. In this paper, we transfer recent developments from abstract decision theory with incomplete preferential and probabilistic information to this multi-target setting and show how – by exploiting the (potentially) partial cardinal and partial probabilistic information – more informative orders for comparing decisions can be given than the Pareto order. We discuss some interesting properties of the proposed orders between decision options and show how they can be concretely computed by linear optimization. We conclude the paper by demonstrating our framework in an artificial (but quite real-world) example in the context of comparing algorithms under different performance measures.
     </details>
  </div>
  <img src="/assets/mdai.webp">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><a href="https://link.springer.com/chapter/10.1007/978-3-319-61581-3_30" class="paper-link">Decision Theory Meets Linear Optimization Beyond Computation</a></b></div>
    <div class="pub-meta">ECSQARU 2017</div>
    <span class="tag">CORE C</span>

    <details><summary>Abstract</summary>
    The paper is concerned with decision making under complex uncertainty. We consider the Hodges and Lehmann-criterion relying on uncertain classical probabilities and Walley’s maximality relying on imprecise probabilities. We present linear programming based approaches for computing optimal acts as well as for determining least favorable prior distributions in finite decision settings. Further, we apply results from duality theory of linear programming in order to provide theoretical insights into certain characteristics of these optimal solutions. Particularly, we characterize conditions under which randomization pays out when defining optimality in terms of the Gamma-Maximin criterion and investigate how these conditions relate to least favorable priors.
     </details>
  </div>
  <img src="/assets/ecsqaru.webp">
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
