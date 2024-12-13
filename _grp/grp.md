---
title: "Group Theory"
permalink: /grp/
collection: qrp
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
</style>

<div class="learning-content">
  <h1>Group Theory</h1>

<a name="linear-algebra"></a>
<div class="text-block">
 <p>I began studying group theory after enrolling in Math 5105 Modern Algebra I at Missouri S&T, taught by Dr. Clayton Lungstrum. His clear and engaging teaching style made the subject both accessible and inspiring, and I consider him the best instructor I’ve had at this university. While the course provided a strong foundation, much of my deeper understanding came from self-study and working through <a href="https://edisciplinas.usp.br/pluginfile.php/5409004/mod_resource/content/2/John%20B.%20Fraleigh%2C%20Victor%20J.%20Katz%20-%20A%20first%20course%20in%20abstract%20algebra-Addison-Wesley%20%282003%29%20%281%29.pdf">A First Course in Abstract Algebra by John B. Fraleigh (7th Edition)</a>.</p>
 <p>My notes include detailed proofs and explanations from the textbook, insights gained from solving problems, and explorations of challenging topics tackled independently. They also feature a dedicated section for problems with solutions and the project report I completed as part of the course.</p>
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
