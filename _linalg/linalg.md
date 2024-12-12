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

/* TOC Styles */
.collapsible-toc {
  list-style-type: none;
  padding-left: 0;
}

.toc-item {
  margin-bottom: 0.5em;
}

.toc-header {
  cursor: pointer;
  display: flex;
  align-items: center;
  outline: none; /* Remove default focus outline */
}

.toc-header a {
  text-decoration: none;
  color: inherit;
}

.toc-sublist {
  list-style-type: square;
  padding-left: 20px;
  display: none; /* Hidden by default */
}

.toc-item.active .toc-sublist {
  display: block;
}

/* Arrow Indicators */
.toc-header::after {
  content: '▼'; /* Down arrow */
  margin-left: auto;
  transition: transform 0.3s;
}

.toc-item.active .toc-header::after {
  transform: rotate(-180deg); /* Up arrow */
}

/* Hover Behavior for Desktop */
@media (min-width: 768px) {
  .toc-header:hover + .toc-sublist {
    display: block;
  }
  
  .toc-header::after {
    display: none; /* Hide arrows on desktop hover */
  }
}

/* Click Behavior for Mobile */
@media (max-width: 767px) {
  .toc-header::after {
    display: inline; /* Show arrows on mobile */
  }
}

/* Indicate clickable headers with focus styles */
.toc-header:focus {
  outline: 2px solid #000;
}

/* Improve arrow visibility */
.toc-header::after {
  font-size: 0.8em;
  color: #555;
}
</style>

<script>
function loadPdfPage(pdfUrl) {
  document.getElementById('pdf-viewer').src = pdfUrl;
  document.getElementById('pdf-viewer-container').scrollIntoView({ behavior: 'smooth' });
}

document.addEventListener('DOMContentLoaded', function() {
  const tocHeaders = document.querySelectorAll('.toc-header');

  tocHeaders.forEach(header => {
    header.addEventListener('click', function(event) {
      if (window.innerWidth < 768) {
        const parentItem = this.parentElement;
        const isActive = parentItem.classList.toggle('active');
        this.setAttribute('aria-expanded', isActive);
        
        // Close other items
        document.querySelectorAll('.toc-item').forEach(item => {
          if (item !== parentItem) {
            item.classList.remove('active');
            item.querySelector('.toc-header').setAttribute('aria-expanded', false);
          }
        });
      }
    });

    // Allow toggling with Enter key
    header.addEventListener('keypress', function(event) {
      if (event.key === 'Enter') {
        header.click();
      }
    });
  });
});
</script>

<h2 id="toc">Table of Contents</h2>

<ol class="collapsible-toc">
  <li class="toc-item">
    <div class="toc-header" tabindex="0" aria-expanded="false">
      Book 1: <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=3')">Chapter 1 Introduction to Vectors</a>
    </div>
    <ul class="toc-sublist">
      <li>n Dimensional Cube <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=22')">(Page 22)</a>, <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=36')">(Page 36)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=57')">Chapter 2 Solving Linear Equations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=17')">Matrix Multiplication Methods (Page 71)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=76')">Block Matrix (Page 76)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=92')">Gershgorin Circle Theorem (Page 92)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=97')">LU Factorization (Page 97)</a></li>
    </ul>
  </li>
  
  <li class="toc-item">
    <div class="toc-header" tabindex="0" aria-expanded="false">
      Book 2: <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a>
    </div>
    <ul class="toc-sublist">
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=36')">Page Rank Algorithm (Page 36)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=62')">Neumann Series (Page 62)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=88')">Vandermonde Matrix (Page 88)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=168')">Chapter 3 Vector Spaces and Subspaces</a></li>
    </ul>
  </li>

  <!-- Add more toc-item blocks for additional books -->
</ol>

<div id="pdf-viewer-container" style="width: 100%; display: flex; justify-content: center;">
  <iframe id="pdf-viewer"
    src="https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf&zoom=110"
    style="width: 210mm; height: 297mm; border: none;">
  </iframe>
</div>
