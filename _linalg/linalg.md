---
title: "Linear Algebra"
permalink: /linalg/
layout: default
classes: wide
---

<div class="learning-topnav">
  <a href="/learning/">Back</a>
  <a href="/qc#">Quantum Computing</a>  
  <a href="/qc#">Special Functions</a>
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

/* Dropdown styling */
.dropdown {
  position: relative;
  display: block;
  margin-bottom: 15px;
}

.dropdown span {
  cursor: pointer;
  font-weight: bold;
  padding: 10px;
  background-color: #f0f0f0;
  border: 1px solid #ccc;
  border-radius: 5px;
  display: block;
}

.dropdown-content {
  display: none;
  position: relative;
  background-color: #ffffff;
  padding: 10px;
  z-index: 1;
  border: 1px solid #ddd;
  border-radius: 5px;
}

/* Hover for larger screens */
@media (min-width: 768px) {
  .dropdown:hover .dropdown-content {
    display: block;
  }
}

/* Toggle for click */
.dropdown.open .dropdown-content {
  display: block;
}

.dropdown-content ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.dropdown-content ul li {
  padding: 5px 0;
}

.dropdown-content ul li a {
  text-decoration: none;
  color: #333;
}

.dropdown-content ul li a:hover {
  text-decoration: underline;
}
</style>

<script>
function toggleDropdown(element) {
  const parent = element.parentElement;

  // Close other dropdowns
  document.querySelectorAll('.dropdown.open').forEach(dropdown => {
    if (dropdown !== parent) dropdown.classList.remove('open');
  });

  // Toggle current dropdown
  parent.classList.toggle("open");
}
</script>

<div class="learning-content">
  <h1>Linear Algebra</h1>

<a name="linear-algebra"></a>
<div class="text-block">
 <p>Linear algebra has been a crucial part of my learning journey, especially as I ventured into quantum computing. I started with <a href="https://archive.org/details/gilbert-strang-introduction-to-linear-algebra-fifth-edition/page/504/mode/2up">Gilbert Strang's Introduction to Linear Algebra</a> to build a strong foundation, but I often found myself exploring much deeper concepts and proofs beyond what the book covered. Throughout this process, <a href="https://math.stackexchange.com/users/223599/sooraj-soman">Mathematics Stack Exchange</a> became an invaluable resource for clarifying doubts, solving challenging problems, and learning through engaging discussions with the community.</p>
 <p>These notes are an attempt to organize and share what I’ve learned over the years. They reflect not only the material from Strang's book but also the extended explorations and insights I’ve gained while tackling questions and problems. Having enrolled in Math 6108 Applied Matrix Theory at Missouri S & T, my notes go well beyond the scope of a 6000-level advanced graduate course.</p>
</div>

<h2 id="toc">Table of Contents</h2>

<div class="dropdown">
  <span onclick="toggleDropdown(this)">Book 1: Linear Algebra</span>
  <div class="dropdown-content">
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=3')">Chapter 1: Introduction to Vectors</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=22')">n Dimensional Cube (Page 22)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=36')">Matrix Multiplication Methods (Page 36)</a></li>
    </ul>
  </div>
</div>

<div class="dropdown">
  <span onclick="toggleDropdown(this)">Book 2: Markov Matrices</span>
  <div class="dropdown-content">
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Chapter 1: Markov Processes</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=36')">Page Rank Algorithm (Page 36)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=62')">Neumann Series (Page 62)</a></li>
    </ul>
  </div>
</div>

<div id="pdf-viewer-container" style="width: 100%; display: flex; justify-content: center;">
  <iframe id="pdf-viewer"
    src="https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf&zoom=110"
    style="width: 210mm; height: 297mm; border: none;">
  </iframe>
</div>
