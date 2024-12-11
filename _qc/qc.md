---
title: "Quantum Computing"
permalink: /qc/
collection: qc
layout: default
classes: wide
---

<div class="learning-topnav">
  <a href="/learning/">Back</a>
  <a href="/linalg/">Linear Algebra</a>
</div>


<style>
.learning-content {
  margin-left: 5%;
  margin-right: 5%;
  max-width: 100%;
}
.text-block {
    text-align: justify;
    text-indent: 50px;
    max-width: 100%;
}
</style>

<div class="learning-content">
  <h1>Quantum Computing</h1>

<a name="linear-algebra"></a>
<div class="text-block">
 <p>Linear algebra has been a crucial part of my learning journey, especially as I ventured into quantum computing. I started with <a href="https://archive.org/details/gilbert-strang-introduction-to-linear-algebra-fifth-edition/page/504/mode/2up">Gilbert Strang's Introduction to Linear Algebra</a> to build a strong foundation, but I often found myself exploring much deeper concepts and proofs beyond what the book covered. Throughout this process, <a href="https://math.stackexchange.com/users/223599/sooraj-soman">Mathematics Stack Exchange</a> became an invaluable resource for clarifying doubts, solving challenging problems, and learning through engaging discussions with the community.</p>
 <p>These notes are an attempt to organize and share what I’ve learned over the years. They reflect not only the material from Strang's book but also the extended explorations and insights I’ve gained while tackling questions and problems. Having enrolled in Math 6108 Applied Matrix Theory at Missouri S & T, my notes go well beyond the scope of a 6000-level advanced graduate course.</p>
</div>

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

<h2 id="toc">Table of Contents</h2>

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
  
  <li>
    Book 2: <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=36')">Page Rank Algorithm (Page 36)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=62')">Neumann Series (Page 62)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=88')">Vandermonde Matrix (Page 88)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=168')">Chapter 3 Vector Spaces and Subspaces</a></li>
    </ul>
  </li>


<div id="pdf-viewer-container">
  <iframe id="pdf-viewer"
    src="https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf"
    style="width: 100%; height: 100vh; border: none;">
  </iframe>
</div>


