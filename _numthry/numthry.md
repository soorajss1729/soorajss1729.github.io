---
title: "Number Theory"
permalink: /numthry/
collection: numthry
layout: default
classes: wide
---

<div class="learning-topnav">
  <a href="/learning/">Back</a>
  <a href="/linalg/">Linear Algebra</a>
  <a href="/qc#">Quantum Computing</a>
  <a href="/grp/">Group Theory</a>
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
  <h1>Number Theory</h1>

<a name="numthry"></a>
<div class="text-block">
 <p>I explored foundational topics in **Number Theory** while studying quantum algorithms and modular arithmetic, particularly in *Nielsen and Chuang's Quantum Computing and Quantum Information*. Initially, my focus was on understanding the appendix in the book, but I later extended my studies through additional resources. I look forward to diving deeper into advanced number theory and exploring its interplay with **cryptography** and **quantum algorithms**.</p>
 
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
</div>


<div id="pdf-viewer-container" style="width: 100%; display: flex; justify-content: center;">
  <iframe id="pdf-viewer"
    src="{% if page.permalink == '/grp/' %}
            https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf&zoom=110
         {% elsif page.permalink == '/linalg/' %}
            https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf&zoom=110
         {% elsif page.permalink == '/qc/' %}
            https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf&zoom=110
         {% else %}
            https://soorajss1729.github.io/pdfjs/viewer.html?file=default.pdf&zoom=110
         {% endif %}"
    style="width: 210mm; height: 297mm; border: none;">
  </iframe>
</div>

