---
title: "Group Theory"
permalink: /grp/
collection: grp
layout: default
classes: wide
---

<div class="learning-topnav">
  <a href="/learning/">Back</a>
  <a href="/linalg/">Linear Algebra</a>
  <a href="/qc#">Quantum Computing</a>
</div>

<style>
.learning-content {
  margin-left: 5%;
  margin-right: 5%;
  max-width: 35cm;
}
.text-block {
    text-align: justify;
    text-indent: 50px;
    max-width: 35cm;
}
#toc-container details {
  margin-bottom: 1em; /* Add spacing between collapsible sections */
}
#toc-container summary {
  font-weight: bold;
  cursor: pointer;
}
/* General styles for TOC */
#toc-container ul {
  margin-left: 10px; /* Indent nested lists */
  padding-left: 10px;   /* Remove any default browser padding */
  list-style-type: square;
}

/* Nested lists inside TOC */
#toc-container ul ul {
  margin-left: 10px; /* Additional indentation for nested lists */
}

/* Mobile-specific adjustments */
@media (max-width: 768px) {
  #toc-container ul {
    margin-left: 2px; /* Reduced indentation on mobile */
  }
  #toc-container ul ul {
    margin-left: 2px; /* Further reduced for nested lists */
  }
}
</style>

<div class="learning-content">
  <h1>Group Theory</h1>

<a name="qc"></a>
<div class="text-block">
 <p>I began studying group theory after enrolling in Math 5105 Modern Algebra I at Missouri S&T, taught by <a href="https://sites.mst.edu/cjlungstrum/">Dr. Clayton Lungstrum</a>. His clear and engaging teaching style made the subject both accessible and inspiring, and I consider him the best instructor I’ve had at this university. While the course provided a strong foundation, much of my deeper understanding came from self-study and working through <a href="https://edisciplinas.usp.br/pluginfile.php/5409004/mod_resource/content/2/John%20B.%20Fraleigh%2C%20Victor%20J.%20Katz%20-%20A%20first%20course%20in%20abstract%20algebra-Addison-Wesley%20%282003%29%20%281%29.pdf">A First Course in Abstract Algebra by John B. Fraleigh (7th Edition)</a>.</p>
 
 <p>My notes include detailed proofs and explanations from the textbook, insights gained from solving problems, and explorations of challenging topics tackled independently. They also feature a dedicated section for problems with solutions and the project report I completed as part of the course.</p>
</div>

<script>
function loadPdfPage(pdfUrl) {
  document.getElementById('pdf-viewer').src = pdfUrl;
  document.getElementById('pdf-viewer-container').scrollIntoView({ behavior: 'smooth' });
}
</script>

<h2 id="toc">Table of Contents</h2>

<div id="toc-container">
  <details>
    <summary>Section 1: Introduction to Groups</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=3')">Introduction</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=7')">Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=22')">Binary Operations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=26')">Properties of Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=39')">Three Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=57')">Subgroups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=64')">Nontrivial Subgroup of $(\mathbb{Z},+)$ is $m\mathbb{Z}$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=68')">Properties of Subgroups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=77')">Cyclic Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-2.pdf#page=3')">Cyclic Groups</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 2: Factor Groups and Homomorphisms</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=1')">Finitely Generated Abelian Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=4')">Homomorphisms</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=10')">Factor Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=16')">Fundamental Homomorphism Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=23')">Converse of Lagrange's Theorem is False</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=27')">Simple Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=29')">Maximal Normal Subgroup</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=30')">Center and Commutator Subgroups</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 3: Group Action on a Set</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=33')">G-Sets</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=35')">Isotropy Subgroups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=40')">Application of G-Sets to Counting</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=42')">Burnside's Formula</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 4: Advanced Group Theory</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=1')">First Isomorphism Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=4')">Join of Subgroups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=6')">Second Isomorphism Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=10')">Third Isomorphism Theorem</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 5: Series of Groups</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=13')">Normal(Subnormal) Series</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=15')">Refinement of a Series</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=16')">Butterfly Lemma</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=17')">Schreier Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=22')">Composition and Principal Series</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=24')">Jordan-Holder Theorem</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 6: Sylow Theorems</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=29')">Introduction</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=33')">Cauchy's Theorem and p-Group</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=37')">Normalizer of a Subgroup</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=41')">First Sylow Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=44')">Sylow p-Subgroup</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=45')">Second Sylow Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=47')">Third Sylow Theorem</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 7: Problem Set</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 9: Coursework Project</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-proj-report.pdf#page=17')">Project Report</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-proj-ppt.pdf#page=22')">My Contribution to the Project Presentation</a></li>
    </ul>
  </details>
</div>





<div id="pdf-viewer-container" style="width: 100%; display: flex; justify-content: center;">
  <iframe id="pdf-viewer"
    src="https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf&zoom=110"
    style="width: 210mm; height: 297mm; border: none;">
  </iframe>
</div>

