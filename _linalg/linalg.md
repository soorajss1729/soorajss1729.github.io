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

/* Dropdown Styling */
.dropdown {
  position: relative;
  display: block;
  margin-bottom: 15px;
}

.dropdown span {
  cursor: pointer;
  font-weight: bold;
  padding: 5px 0;
  color: inherit; /* Retains original link color */
  text-decoration: underline; /* Matches the hyperlink style */
}

/* Subsections (hidden by default) */
.dropdown-content {
  display: none;
  margin-left: 15px;
}

.dropdown-content ul {
  list-style-type: square; /* Keep the bullet points */
  padding-left: 0;
}

.dropdown-content ul li {
  margin: 5px 0;
}

.dropdown-content ul li a {
  text-decoration: underline; /* Matches link styling */
  color: inherit; /* Use the same color as other links */
}

/* Show content on hover (PC) */
@media (min-width: 768px) {
  .dropdown:hover .dropdown-content {
    display: block;
  }
}

/* Show content on click (Mobile and PC) */
.dropdown.open .dropdown-content {
  display: block;
}
</style>

<script>
/* Function to toggle dropdown visibility */
function toggleDropdown(element) {
  const parent = element.parentElement;

  // Close other dropdowns
  document.querySelectorAll('.dropdown.open').forEach(dropdown => {
    if (dropdown !== parent) dropdown.classList.remove('open');
  });

  // Toggle the clicked dropdown
  parent.classList.toggle("open");
}
</script>

<div class="learning-content">
  <h1>Linear Algebra</h1>

  <div class="text-block">
    <p>Linear algebra has been a crucial part of my learning journey, especially as I ventured into quantum computing. I started with <a href="https://archive.org/details/gilbert-strang-introduction-to-linear-algebra-fifth-edition/page/504/mode/2up">Gilbert Strang's Introduction to Linear Algebra</a> to build a strong foundation, but I often found myself exploring much deeper concepts and proofs beyond what the book covered. Throughout this process, <a href="https://math.stackexchange.com/users/223599/sooraj-soman">Mathematics Stack Exchange</a> became an invaluable resource for clarifying doubts, solving challenging problems, and learning through engaging discussions with the community.</p>
    <p>These notes are an attempt to organize and share what I’ve learned over the years. They reflect not only the material from Strang's book but also the extended explorations and insights I’ve gained while tackling questions and problems. Having enrolled in Math 6108 Applied Matrix Theory at Missouri S & T, my notes go well beyond the scope of a 6000-level advanced graduate course.</p>
  </div>

  <h2 id="toc">Table of Contents</h2>

  <!-- Book 1 Dropdown -->
  <div class="dropdown">
    <span onclick="toggleDropdown(this)">Book 1: Chapter 1 Introduction to Vectors</span>
    <div class="dropdown-content">
      <ul>
        <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=22')">n Dimensional Cube (Page 22)</a></li>
        <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=36')">Matrix Multiplication Methods (Page 36)</a></li>
        <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=76')">Block Matrix (Page 76)</a></li>
      </ul>
    </div>
  </div>

  <!-- Book 2 Dropdown -->
  <div class="dropdown">
    <span onclick="toggleDropdown(this)">Book 2: Markov Matrices</span>
    <div class="dropdown-content">
      <ul>
        <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
        <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=36')">Page Rank Algorithm (Page 36)</a></li>
        <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=88')">Vandermonde Matrix (Page 88)</a></li>
      </ul>
    </div>
  </div>
</div>
