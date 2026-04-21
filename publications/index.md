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
  <button onclick="filterPubs('other')">Other</button>
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
    <div class="pub-title"><b><a href="https://aclanthology.org/2025.inlg-main.20/" class="paper-link">Statistical Multicriteria Evaluation of LLM-Generated Text</a></b></div>
    <div class="pub-meta">INLG 2025</div>
    <span class="tag">CORE B</span>

    <details><summary>Abstract</summary>
   Assessing the quality of LLM-generated text remains a fundamental challenge in natural language processing. Current evaluation approaches often rely on isolated metrics or simplistic aggregations that fail to capture the nuanced trade-offs between coherence, diversity, fluency, and other relevant indicators of text quality. In this work, we adapt a recently proposed framework for statistical inference based on Generalized Stochastic Dominance (GSD) that addresses three critical limitations in existing benchmarking methodologies: the inadequacy of single-metric evaluation, the incompatibility between cardinal automatic metrics and ordinal human judgments, and the lack of inferential statistical guarantees. The GSD-front approach enables simultaneous evaluation across multiple quality dimensions while respecting their different measurement scales, building upon partial orders of decoding strategies, thus avoiding arbitrary weighting of the involved metrics. By applying this framework to evaluate common decoding strategies against human-generated text, we demonstrate its ability to identify statistically significant performance differences while accounting for potential deviations from the i.i.d. assumption of the sampling design.
     </details>
  </div>
  <img src="/assets/inlg_logo.png">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://link.springer.com/chapter/10.1007/978-3-032-05134-9_13" class="paper-link">Consensus in Motion: A Case of Dynamic Rationality of Sequential Learning in Probability Aggregation</a></b></div>
    <div class="pub-meta">ECSQARU 2025</div>
    <span class="tag">CORE C</span>

    <details><summary>Abstract</summary>
    We propose a framework for probability aggregation based on propositional probability logic. Unlike conventional judgment aggregation, which focuses on static rationality, our model addresses dynamic rationality by ensuring that collective beliefs update consistently with new information. We show that any consensus-compatible and independent aggregation rule on a non-nested agenda is necessarily linear. Furthermore, we provide sufficient conditions for a fair learning process, where individuals initially agree on a specified subset of propositions known as the common ground, and new information is restricted to this shared foundation. This guarantees that updating individual judgments via Bayesian conditioning—whether performed before or after aggregation—yields the same collective belief. A distinctive feature of our framework is its treatment of sequential decision-making, which allows new information to be incorporated progressively through multiple stages while maintaining the established common ground. We illustrate our findings with a running example in a political scenario concerning healthcare and immigration policies.
     </details>
  </div>
  <img src="/assets/ecsqaru.webp">
</div>

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
    <div class="pub-title"><b><a href="https://link.springer.com/chapter/10.1007/978-3-031-65993-5_13" class="paper-link">Semi-supervised Learning Guided by the Generalized Bayes Rule Under Soft Revision</a></b></div>
    <div class="pub-meta">SMPS 2024</div>
   

    <details><summary>Abstract</summary>
      We provide a theoretical and computational investigation of the Gamma-Maximin method with soft revision, which was recently proposed as a robust criterion for pseudo-label selection (PLS) in semi-supervised learning. Opposed to traditional methods for PLS we use credal sets of priors (“generalized Bayes”) to represent the epistemic modeling uncertainty. These latter are then updated by the Gamma-Maximin method with soft revision. We eventually select pseudo-labeled data that are most likely in light of the least favorable distribution from the so updated credal set. We formalize the task of finding optimal pseudo-labeled data w.r.t. the Gamma-Maximin method with soft revision as an optimization problem. A concrete implementation for the class of logistic models then allows us to compare the predictive power of the method with competing approaches. It is observed that the Gamma-Maximin method with soft revision can achieve very promising results, especially when the proportion of labeled data is low.
    </details>
  </div>
  <img src="/assets/smps.webp">
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
    <div class="pub-title"><b><a href="https://link.springer.com/chapter/10.1007/978-3-031-08971-8_59" class="paper-link">Decision Making with State-Dependent Preference Systems</a></b></div>
    <div class="pub-meta">IPMU 2022</div>
    <span class="tag">CORE C</span>

    <details><summary>Abstract</summary>
     In this paper we present some first ideas for decision making with agents whose preference system may depend on an uncertain state of nature. Our main formal framework here are commonly scalable state-dependent decision systems. After giving a formal definition of those systems, we introduce and discuss two criteria for defining optimality of acts, both of which are direct generalizations of classical decision criteria under risk. Further, we show how our criteria can be naturally extended to imprecise probability models. More precisely, we consider convex and finitely generated credal sets. Afterwards, we propose linear pogramming-based algorithms for evaluating our criteria and show how the complexity of these algorithms can be reduced by approximations based on clustering the preference systems under similar states. Finally, we demonstrate our methods in a toy example.
     </details>
  </div>
  <img src="/assets/ipmu.webp">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://link.springer.com/chapter/10.1007/978-3-031-08974-9_2" class="paper-link">Statistical Models for Partial Orders Based on Data Depth and Formal Concept Analysis</a></b></div>
    <div class="pub-meta">IPMU 2022</div>
    <span class="tag">CORE C</span>

    <details><summary>Abstract</summary>
     In this paper, we develop statistical models for partial orders where the partially ordered character cannot be interpreted as stemming from the non-observation of data. After discussing some shortcomings of distance based models in this context, we introduce statistical models for partial orders based on the notion of data depth. Here we use the rich vocabulary of formal concept analysis to utilize the notion of data depth for the case of partial orders data. After giving a concise definition of unimodal distributions and unimodal statistical models of partial orders, we present an algorithm for efficiently sampling from unimodal models as well as from arbitrary models based on data depth.
     </details>
  </div>
  <img src="/assets/ipmu.webp">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://link.springer.com/chapter/10.1007/978-3-319-61581-3_30" class="paper-link">Decision Theory Meets Linear Optimization Beyond Computation</a></b></div>
    <div class="pub-meta">ECSQARU 2017</div>
    <span class="tag">CORE C</span>

    <details><summary>Abstract</summary>
    The paper is concerned with decision making under complex uncertainty. We consider the Hodges and Lehmann-criterion relying on uncertain classical probabilities and Walley’s maximality relying on imprecise probabilities. We present linear programming based approaches for computing optimal acts as well as for determining least favorable prior distributions in finite decision settings. Further, we apply results from duality theory of linear programming in order to provide theoretical insights into certain characteristics of these optimal solutions. Particularly, we characterize conditions under which randomization pays out when defining optimality in terms of the Gamma-Maximin criterion and investigate how these conditions relate to least favorable priors.
     </details>
  </div>
  <img src="/assets/ecsqaru.webp">
</div>

<div class="pub conference">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://proceedings.mlr.press/v62/jansen17a.html" class="paper-link">Concepts for Decision Making under Severe Uncertainty with
Partial Ordinal and Partial Cardinal Preferences</a></b></div>
    <div class="pub-meta">ISIPTA 2017</div>
    
<details><summary>Abstract</summary>
    We introduce three different approaches for decision making under uncertainty, if (I) there is only partial (both cardinal and ordinal) information on an agent’s preferences and (II) the uncertainty about the states of nature is described by a credal set. Particularly, (I) is modeled by a pair of relations, one specifying the partial rank order of the alternatives and the other modeling partial information on the strength of preference. Our first approach relies on criteria that construct complete rankings of the acts based on generalized expectation intervals. Subsequently, we introduce different concepts of global admissibility that construct partial orders by comparing all acts simultaneously. Finally, we define criteria induced by suitable binary relations on the set of acts and, therefore, can be understood as concepts of local admissibility. Whenever suitable, we provide linear programming based algorithms for checking optimality/admissibility of acts.
     </details>
  </div>
  <img src="/assets/pmlr.svg">
</div>

<!-- ===================================================== -->
<!-- ================= PREPRINTS ========================= -->
<!-- ===================================================== -->

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://arxiv.org/abs/2512.05677" class="paper-link">Empirical Decision Theory</a></b></div>
    <div class="pub-meta">arXiv (2026)</div>

  <details><summary>Abstract</summary>
    Analyzing decision problems under uncertainty commonly relies on idealizing assumptions about the describability of the world, with the most prominent examples being the closed world and the small world assumption. Most assumptions are operationalized by introducing states of the world, conditional on which the decision situation can be analyzed without any remaining uncertainty. Conversely, most classical decision-theoretic approaches are not applicable if the states of the world are inaccessible. We propose a decision model that retains the appeal and simplicity of the original theory, but completely overcomes the need to specify the states of the world explicitly. The main idea of our approach is to address decision problems in a radically empirical way: instead of specifying states and consequences prior to the decision analysis, we only assume a protocol of observed act--consequence pairs as model primitives. We show how optimality in such empirical decision problems can be addressed by using protocol-based empirical choice functions and discuss three approaches for deriving inferential guarantees: (I) consistent statistical estimation of choice sets, (II) consistent statistical testing of choice functions with robustness guarantees, and (III) direct inference for empirical choice functions using credal sets. We illustrate our theory with a proof-of-concept application comparing different prompting strategies in generative AI models.
     </details>
  </div>
  <img src="/assets/arxiv.jpg">
</div>

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://arxiv.org/abs/2602.07593" class="paper-link">Beyond Arrow: From Impossibility to Possibilities in Multi-Criteria Benchmarking</a></b></div>
    <div class="pub-meta">arXiv (2026)</div>
  
  <details><summary>Abstract</summary>
  Modern benchmarks such as HELM MMLU account for multiple metrics like accuracy, robustness and efficiency. When trying to turn these metrics into a single ranking, natural aggregation procedures can become incoherent or unstable to changes in the model set. We formalize this aggregation as a social choice problem where each metric induces a preference ranking over models on each dataset, and a benchmark operator aggregates these votes across metrics. While prior work has focused on Arrow's impossibility result, we argue that the impossibility often originates from pathological examples and identify sufficient conditions under which these disappear, and meaningful multi-criteria benchmarking becomes possible. In particular, we deal with three restrictions on the combinations of rankings and prove that on single-peaked, group-separable and distance-restricted preferences, the benchmark operator allows for the construction of well-behaved rankings of the involved models. Empirically, we investigate several modern benchmark suites like HELM MMLU and verify which structural conditions are fulfilled on which benchmark problems.
     </details>
  </div>
  <img src="/assets/arxiv.jpg">
</div>

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://arxiv.org/abs/2502.14581" class="paper-link">A Statistical Case Against Empirical Human–AI Alignment</a></b></div>
    <div class="pub-meta">arXiv (2025)</div>

    <details><summary>Abstract</summary>
    Empirical human-AI alignment aims to make AI systems act in line with observed human behavior. While noble in its goals, we argue that empirical alignment can inadvertently introduce statistical biases that warrant caution. This position paper thus advocates against naive empirical alignment, offering prescriptive alignment and a posteriori empirical alignment as alternatives. We substantiate our principled argument by tangible examples like human-centric decoding of language models.
     </details>
  </div>
 <img src="/assets/arxiv.jpg">
</div>

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://doi.org/10.5282/ubm/epub.40450" class="paper-link">A simple descriptive method for multidimensional item response theory based on stochastic dominance</a></b></div>
    <div class="pub-meta">Department of Statistics: Technical Reports, No.210 (2017)</div>

    <details><summary>Abstract</summary>
    In this paper we develop a descriptive concept of a (partially) ordinal joint scaling of items and persons in the context of (dichotomous) item response analysis. The developed method has to be understood as a purely descriptive method describing relations among the data observed in a given item response data set, it is not intended to directly measure some presumed underlying latent traits. We establish a hierarchy of pairs of item difficulty and person ability orderings that empirically support each other. The ordering principles we use for the construction are essentially related to the concept of first order stochastic dominance. Our method is able to avoid a paradoxical result of multidimensional item response theory models described in \cite{hooker2009paradoxical}. We introduce our concepts in the language of formal concept analysis. This is due to the fact that our method has some similarities with formal concept analysis and knowledge space theory: Both our methods as well as descriptive techniques used in knowledge space theory (concretely, item tree analysis) could be seen as two different stochastic generalizations of formal implications from formal concept analysis.
     </details>
  </div>
 <img src="/assets/simple.jpg">
</div>

<div class="pub preprint">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://doi.org/10.5282/ubm/epub.40416" class="paper-link">Detecting stochastic dominance for poset-valued random variables as an example of linear programming on closure systems</a></b></div>
    <div class="pub-meta">Department of Statistics: Technical Reports, No.209 (2017)</div>

    <details><summary>Abstract</summary>
    In this paper we develop a linear programming method for detecting stochastic dominance for random variables with values in a partially ordered set (poset) based on the upset-characterization of stochastic dominance. The proposed detection-procedure is based on a descriptively interpretable statistic, namely the maximal probability-difference of an upset. We show how our method is related to the general task of maximizing a linear function on a closure system. Since closure systems are describable via their valid formal implications, we can use here ingredients of formal concept analysis. We also address the question of inference via resampling and via conservative bounds given by the application of Vapnik-Chervonenkis theory, which also allows for an adequate pruning of the envisaged closure system that allows for the regularization of the test statistic (by paying a price of less conceptual rigor). We illustrate the developed methods by applying them to a variety of data examples, concretely to multivariate inequality analysis, item impact and differential item functioning in item response theory and to the analysis of distributional differences in spatial statistics. The power of regularization is illustrated with a data example in the context of cognitive diagnosis models.
     </details>
  </div>
 <img src="/assets/detecting.jpg">
</div>

<!-- ===================================================== -->
<!-- ================= BOOK CHAPTERS ===================== -->
<!-- ===================================================== -->

<div class="pub book">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://link.springer.com/chapter/10.1007/978-3-031-15436-2_13" class="paper-link">Quantifying Degrees of E-admissibility in Decision Making with Imprecise Probabilities</a></b></div>
    <div class="pub-meta">Reflections on the Foundations of Probability and Statistics:
Essays in Honor of Teddy Seidenfeld, Theory and Decision Library A (2022)</div>
    
    <details><summary>Abstract</summary>
    This paper is concerned with decision making using imprecise probabilities and looks at extensions and aspects of the criterion of E-admissibility, as introduced by Levi and extensively studied and advocated by Teddy Seidenfeld. In the first part, we introduce a decision criterion that allows for explicitly modeling how far maximal decisions in Walley’s sense are accepted to deviate from E-admissibility. We also provide an efficient and simple algorithm based on linear programming theory for this criterion. In the second part of the paper, we propose two measures for quantifying what we call the extent of E-admissibility of an E-admissible act, i.e. the size of the set of measures for which the corresponding act maximizes expected utility. The first measure is the maximal diameter of this set, while the second one relates to the maximal barycentric cube that can be inscribed into it. Also here, for both measures, we give linear programming algorithms capable to deal with them. Finally, we discuss some ideas in the context of ordinal decision theory. The paper concludes with a stylized application example illustrating all introduced concepts.
     </details>
  </div>
  <img src="/assets/festschrift.webp">
</div>

<!-- ===================================================== -->
<!-- ================= THESES ============================= -->
<!-- ===================================================== -->

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://arxiv.org/abs/2501.10195" class="paper-link">Contributions to the Decision Theoretic Foundations of Machine Learning and Robust Statistics under Weakly Structured Information</a></b></div>
    <div class="pub-meta">Habilitation thesis, Department of Statistics, LMU Munich (2025)</div>

      <details><summary>Abstract</summary>
    This habilitation thesis is cumulative and, therefore, is collecting and connecting research that I (together with several co-authors) have conducted over the last few years. Thus, the absolute core of the work is formed by the ten publications listed on page 5 under the name Contributions 1 to 10. The references to the complete versions of these articles are also found in this list, making them as easily accessible as possible for readers wishing to dive deep into the different research projects. The chapters following this thesis, namely Parts A to C and the concluding remarks, serve to place the articles in a larger scientific context, to (briefly) explain their respective content on a less formal level, and to highlight some interesting perspectives for future research in their respective contexts. Naturally, therefore, the following presentation has neither the level of detail nor the formal rigor that can (hopefully) be found in the papers. The purpose of the following text is to provide the reader an easy and high-level access to this interesting and important research field as a whole, thereby, advertising it to a broader audience.
     </details>
  </div>
  <img src="/assets/lmu.jpg">
</div>

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://doi.org/10.5282/edoc.22653" class="paper-link">Some contributions to decision making in complex information settings with imprecise probabilities and incomplete preferences: theoretical and algorithmic results</a></b></div>
    <div class="pub-meta">Doctoral dissertation, Department of Statistics, LMU Munich (2018)</div>

      <details><summary>Abstract</summary>
    A significant amount of the challenges arising in the modern sciences can be reformulated as
some suitable problem belonging to the theory of Decision Under Uncertainty. This includes
parameter estimation and hypothesis testing in Statistics, modeling an agent’s preferences and
choice behavior in Philosophy and Economics or the formalization of game theoretic problems.
The basic model of this theory is equally simple and expressive: A decision maker (or agent)
can choose an alternative (or act) X from a set G of different available options. However, the
consequence that choosing X ∈ G yields depends on which potential state of the world from a set
S turns out to be the true one. Formally, the objects of choice are represented by random elements
X :S →A, where A is a set of consequences for which, usually, some additional order structure
is available. For this very general setup, several concepts for obtaining an optimal alternative X∗
from G have been proposed. However, almost all of these concepts (more or less directly) rely
on the following assumptions: (I) the ability of the agent to characterize her beliefs about the
states of the world from S by some classical probability measure π and (II) the availability of a
cardinal utility function that adequately characterizes the agent’s preferences. Additionally, by
(III) restricting the model to single agents, also the case where decisions have to be formed by
inhomogeneous groups is excluded in the classical framework.
The present cumulative PhD project models decision problems in settings with (potentially) very
weakly structured, or incomplete, information available, i.e. in settings where one or more of the
classical assumptions (I), (II) and (III) are violated. Moreover, we propose criteria for optimal
decision making that are applicable in such weakly structured situations. Here, we lay a special
focus on obtaining new theoretical insights into the properties of these optimal decisions and on
providing algorithms capable of finding optimal decisions in these complex situations.
Contribution 1 deals with decision problems where only assumption (I) is violated. We pro
pose algorithms for computing optimal acts with respect to criteria based on uncertain classical
probabilities as well as on imprecise probabilities. Further, we give conditions under which ran
domization in decision making pays out and characterize these in terms of least favorable priors.
Contribution 2 again deals with violations of assumption (I). We introduce a new decision
criterion and provide a simple algorithm for evaluating it. Further, we propose two measures for
quantifying the extent of E-Admissibility and give linear programming algorithms for computing
these. Finally, we discuss some ideas in the context of ordinal decision theory.
Contribution 3 investigates simultaneous violations of (I) and (II). We consider acts taking
values in so-called preference systems and propose three approaches for constructing decision
criteria: i) generalized expectation intervals, ii) global admissibility, and iii) local admissibility.
Whenever suitable, we provide linear programming based algorithms for checking optimality.
Contribution 4 deals with violations of (III). We propose a criterion for evaluating the ade
quateness of preference aggregation procedures reflecting the group’s homogeneity. We show how
to approximate our criterion if information is only imperfectly given and how to estimate these
approximations from data. Finally, we compare common aggregation rules in a simulation study.
Contribution 5 develops a linear programming method for detecting stochastic dominance for
random variables with values in a partially ordered set. We study the dual program and discuss
its properties. Subsequently, we address the question of inference by utilizing resampling methods
as well as conservative bounds that are given by the application of Vapnik-Chervonenkis theory.

     </details>
  </div>
  <img src="/assets/lmu.jpg">
</div>

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://doi.org/10.5282/ubm/epub.25591" class="paper-link">Decision making under partial information using precise and imprecise probabilistic models</a></b></div>
    <div class="pub-meta">MSc dissertation, Department of Statistics, LMU Munich (2015)</div>

      <details><summary>Abstract</summary>
    In this work we recall and discuss optimality criteria for decision making under
uncertainty with respect to different assumptions concerning the structure of
the information available. First, an overview of the basic concepts of classi
cal decision theory is given. Here, particular emphasis is placed on explaining
classical decision criteria (i.e. criteria for the case that the uncertainty can
be characterized by using classical probabilistic models) from literature and
discussing the assumptions underlying them (specifically Bernoulli-, Maximin
and Hodges & Lehmann-criterion are discussed). Afterwards, in order to es
tablish the mathematical basis necessary, a brief introduction to the theory of
linear optimization is provided. Thereby, particular interest lies in recalling
theoretical results concerning the resolvability of linear optimization problems.
Subsequently, we demonstrate how linear optimization theory can be used to
construct algorithms for determining optimal decisions (with respect to the
classical criteria) in finite decision problems. Examples of concrete decision
problems are given. Next, we give some (theoretical and practical) examples
that support the idea of introducing imprecise probabilistic models to decision
theory. Accordingly, two common generalizations of classical probability the
ory are explained: Credal sets and interval probability. Connections of the
two concepts are shown up. Finally, we recall criteria for optimal decision
making, if the uncertainty is characterized by a credal set or an interval proba
bility respectively (specifically interval dominance, E-admissibility, maximality,
Γ-Maximin-criterion, Γ-Maximax-criterion and a criterion combining the two
latter). Again, for all criteria discussed, we illustrate and explain algorithms
for determining optimal decisions.
     </details>
  </div>
  <img src="/assets/lmu.jpg">
</div>

<div class="pub thesis">
  <div class="pub-left">
    <div class="pub-title"><b>Boole'sche Algebren und der Stone'sche Darstellungssatz</b></div>
    <div class="pub-meta">BSc dissertation, Department of Mathematics, LMU Munich (2013)</div>
  </div>
  <img src="/assets/lmu.jpg">
</div>


<!-- ===================================================== -->
<!-- ================= OTHER ============================= -->
<!-- ===================================================== -->

<div class="pub other">
  <div class="pub-left">
    <div class="pub-title"><b><a href="https://riviste.unimi.it/index.php/thereasoner/issue/view/2363" class="paper-link">What’s hot in Mathematical Philosophy?</a></b></div>
    <div class="pub-meta">The Reasoner (2025)</div>

      <details><summary>Abstract</summary>
    An impreciseprobabilitymodel P is called two-monotone  if  it  satisfies  the inequality P(A)+P(B)≤P(A∩B)+P(A∪B) for arbitrary events A and B.  Amuch   quoted   phrase   from Peter  Walley, the luminous figure   in   imprecise   probabilities,   is  that  he  doesn’t “...know   any   rationality   argument   for   two-monotonicity, beyond its computational convenience”. And obviously: Usinga  model P that  is  two-monotone  is  computationally  very convenient,  since  for  instance  lower  and  upper  expectations of  arbitrary  (bounded)  gambles  can  be  computed  by  closedformulas. So,  more  interestingly:   What  about  the  second part of the statement, the “beyond” part?
     </details>
  </div>
  <img src="/assets/lmu.jpg">
</div>
