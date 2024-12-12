---
title: ""
permalink: /stac/
layout: default
collection: stac
entries_layout: grid
classes: wide
---

<div class="learning-topnav">
  <a href="lin-stac">Mathematics Stack Exchange</a>
  <a href="/qc-stac">Quantum Computing Stack Exchange</a>
</div>

<style>
.qc-stac {
  margin-left: 5%;
  margin-right: 5%;
  text-align: justify;
  text-indent: 50px;
  max-width: 100%;
}
.mat-stac {
  margin-left: 5%;
  margin-right: 5%;
  text-align: justify;
  text-indent: 50px;
  max-width: 100%;
}
.text-block {
  margin-left: 5%;
  margin-right: 5%;
  text-align: justify;
  text-indent: 50px;
  max-width: 100%;
}
</style>

<style>
/* Add vertical spacing below the Table of Contents */
ul {
  margin-bottom: 1.5em; /* Adjust this value for more or less vertical space */
}
/* Remove default numbering and padding from the main ordered list */
ol {
  list-style-type: decimal;
  padding-left: 0;
  margin-left: 0;
}

/* Remove bullets from main ordered list items */
ol > li {
  list-style-type: none;
}

/* Add bullets to nested unordered lists (subsections) */
ol > li > ul {
  list-style-type: square; /* Options: disc, circle, square */
  padding-left: 0px;    /* Adjust to control indentation */
  margin-left: 30px;
}
</style>

<script>
function loadPdfPage(pdfUrl) {
  document.getElementById('pdf-viewer').src = pdfUrl;
  document.getElementById('pdf-viewer-container').scrollIntoView({ behavior: 'smooth' });
}
</script>

<h2 id="toc">Mathematics Stack Exchange</h2>

<ol>
  <li>
    Book 1: <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=3')">Postulates of Quantum Mechanics</a>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=46')">Distinguishing Quantum States</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=56')">Projective Measurement</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=73')">POVM Measurement</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=93')">General Measurement=Projective+Unitary</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=106')">Superdense Coding</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=121')">Tensor Product</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=165')">Multipartite System</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=182')">Schmidt Decomposition</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=191')">Quantum Measurement Revisited</a></li>
    </ul>
  </li>
## Mathematics Stack Exchange
</a>
<div class="text-block">
<a name="mat-stac"></a>
1. <a href="https://math.stackexchange.com/questions/4614700/prove-fy-%E2%88%92-fx-leq-fy-%E2%88%92-x-if-y-%E2%88%92-x-%E2%89%A4-1-2-given-fx-x-log-2-x">$f(y) - f(x) \leq f(|y - x|)$ if $|y - x| \leq \frac{1}{2}$ given $f(x) = -x \log_2 x$</a>, Analyzed the behavior of the inequality and proved a bound with detailed steps and reasoning.
  
  [ $f(y) - f(x) \leq f(|y - x|)$ if $|y - x| \leq \frac{1}{2}$ given $f(x) = -x \log_2 x$
][1]: Analyzed the behavior of the inequality and proved a bound with detailed steps and reasoning.

3. [Understanding Filippov’s Inductive Proof for Jordan Canonical Form][2]: Provided a detailed explanation and visual aid for the proof after extended discussions.

4. [Understanding the Expression $\text{tr}(\rho(X \otimes I)) = \sum_{a,b,a',b'} \rho_{ab,a'b'} X_{a,a'} \delta_{b,b'}$][3]: Initiated and contributed to a detailed discussion on the trace properties of tensor products.

5. [The median minimizes the sum of absolute deviations (the $\ell_1$ norm)][4]: Provided a detailed explanation of a standard proof with an original example.

  [1]: https://math.stackexchange.com/questions/4614700/prove-fy-%E2%88%92-fx-leq-fy-%E2%88%92-x-if-y-%E2%88%92-x-%E2%89%A4-1-2-given-fx-x-log-2-x
  [2]: https://math.stackexchange.com/questions/3909381/filippovs-inductive-proof-for-jordan-canonical-form/3911296#3911296
  [3]: https://math.stackexchange.com/questions/4250990/understanding-the-expression-tr-big-rhox-otimes-i-big-sum-a-b-a-b-rho
  [4]: https://math.stackexchange.com/questions/113270/the-median-minimizes-the-sum-of-absolute-deviations-the-ell-1-norm/2364943#2364943



## Quantum Computing Stack Exchange

<a name="qc-stac"></a>
 1. [Derivation of Efficiency of Phase Estimation Algorithm][1]: Explored and engaged deeply with the derivation of efficiency bounds for the phase estimation algorithm.
 2. [Why does the $\chi$ matrix have $d^4-d^2$ independent parameters?][2]: Initiated and actively contributed to an in-depth discussion related to the $\chi$ matrix in quantum process tomography.


  [1]: https://quantumcomputing.stackexchange.com/questions/22032/derivation-of-efficiency-of-phase-estimation-algorithm
  [2]: https://quantumcomputing.stackexchange.com/questions/28924/why-does-the-chi-matrix-have-d4-d2-independent-parameters

