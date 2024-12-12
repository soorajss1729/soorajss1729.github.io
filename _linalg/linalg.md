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
ol.toc {
  list-style-type: decimal;
  padding-left: 0;
  margin-left: 0;
}

/* Remove bullets from main ordered list items */
ol.toc > li {
  list-style-type: none;
  position: relative; /* For positioning the toggle button */
  padding-left: 25px; /* Space for the toggle button */
}

/* Add bullets to nested unordered lists (subsections) */
ol.toc > li > ul {
  list-style-type: square; /* Options: disc, circle, square */
  padding-left: 0px;    /* Adjust to control indentation */
  margin-left: 30px;
  
  /* Initially hide the subsections */
  display: none;
}

/* Style for the toggle buttons */
.toggle-button {
  position: absolute;
  left: 0;
  top: 0;
  cursor: pointer;
  font-weight: bold;
  user-select: none;
  width: 20px;
  text-align: center;
}

/* Initial state: plus sign */
.toggle-button::before {
  content: "+";
}

/* Active state: minus sign */
.toggle-button.active::before {
  content: "−";
}

/* Optional: Add hover effects */
.toggle-button:hover {
  color: #007BFF; /* Change color on hover */
}

/* Ensure links are displayed inline and not obscured */
ol.toc a {
  display: inline-block;
  margin-left: 5px; /* Space between toggle button and link */
  text-decoration: none; /* Remove underline if desired */
  color: inherit; /* Inherit color from parent */
}

/* Optional: Change link color on hover */
ol.toc a:hover {
  text-decoration: underline;
  color: #0056b3;
}
</style>

<script>
// Function to load PDF pages as you already have
function loadPdfPage(pdfUrl) {
  document.getElementById('pdf-viewer').src = pdfUrl;
  document.getElementById('pdf-viewer-container').scrollIntoView({ behavior: 'smooth' });
}

// Function to initialize collapsible TOC
function initializeCollapsibleTOC() {
  // Select all main TOC list items that have a nested ul
  const tocItems = document.querySelectorAll('ol.toc > li');

  tocItems.forEach(function(item) {
    const subList = item.querySelector('ul');
    if (subList) {
      // Create a span element to act as the toggle button
      const toggleButton = document.createElement('span');
      toggleButton.classList.add('toggle-button');
      
      // Insert the toggle button at the beginning of the list item
      item.insertBefore(toggleButton, item.firstChild);
      
      // Add click event listener to the toggle button
      toggleButton.addEventListener('click', function(event) {
        event.stopPropagation(); // Prevent event bubbling
        
        // Toggle the display of the subsections
        if (subList.style.display === 'none' || subList.style.display === '') {
          subList.style.display = 'block';
          toggleButton.classList.add('active');
        } else {
          subList.style.display = 'none';
          toggleButton.classList.remove('active');
        }
      });
      
      // Initially hide the subsections
      subList.style.display = 'none';
    }
  });
}

// Initialize the collapsible TOC after the DOM is fully loaded
document.addEventListener('DOMContentLoaded', function() {
  initializeCollapsibleTOC();
});
</script>

<div class="learning-content">
  <h1>Linear Algebra</h1>

<a name="linear-algebra"></a>
<div class="text-block">
 <p>Linear algebra has been a crucial part of my learning journey, especially as I ventured into quantum computing. I started with <a href="https://archive.org/details/gilbert-strang-introduction-to-linear-algebra-fifth-edition/page/504/mode/2up">Gilbert Strang's Introduction to Linear Algebra</a> to build a strong foundation, but I often found myself exploring much deeper concepts and proofs beyond what the book covered. Throughout this process, <a href="https://math.stackexchange.com/users/223599/sooraj-soman">Mathematics Stack Exchange</a> became an invaluable resource for clarifying doubts, solving challenging problems, and learning through engaging discussions with the community.</p>
 <p>These notes are an attempt to organize and share what I’ve learned over the years. They reflect not only the material from Strang's book but also the extended explorations and insights I’ve gained while tackling questions and problems. Having enrolled in Math 6108 Applied Matrix Theory at Missouri S & T, my notes go well beyond the scope of a 6000-level advanced graduate course.</p>
</div>
</div>

<h2 id="toc">Table of Contents</h2>

<ol class="toc">
  <li>
    Book 1: <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=3')">Chapter 1 Introduction to Vectors</a>
    <ul>
      <li>n Dimensional Cube <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=22')">(Page 22)</a>, <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=36')">(Page 36)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=57')">Chapter 2 Solving Linear Equations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=17')">Matrix Multiplication Methods (Page 71)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=76')">Block Matrix (Page 76)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=92')">Gershgorin Circle Theorem (Page 92)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=97')">LU Factorization (Page 97)</a></li>
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
</ol>

<div id="pdf-viewer-container" style="width: 100%; display: flex; justify-content: center;">
  <iframe id="pdf-viewer"
    src="https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf&zoom=110"
    style="width: 210mm; height: 297mm; border: none;">
  </iframe>
</div>
