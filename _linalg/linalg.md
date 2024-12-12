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
ul.toc-sublist {
  margin-bottom: 1.5em; /* Adjust this value for more or less vertical space */
}

/* Remove default numbering and padding from the main ordered list */
ol.collapsible-toc {
  list-style-type: none;
  padding-left: 0;
  margin-left: 0;
}

/* TOC Styles */
.collapsible-toc .toc-item {
  margin-bottom: 0.5em;
}

.collapsible-toc .toc-header {
  display: flex;
  align-items: center;
  cursor: pointer;
}

/* Style the toggle button */
.toggle-button {
  background: none;
  border: none;
  cursor: pointer;
  margin-right: 0.5em;
  font-size: 1em;
  transition: transform 0.3s;
  /* Increase tappable area on mobile */
  padding: 0.2em;
  line-height: 1;
}

.toggle-button::before {
  content: '▼'; /* Down arrow */
  display: inline-block;
  transition: transform 0.3s;
  font-size: 0.8em;
  color: #555;
}

/* Rotate the arrow when expanded */
.toc-item.expanded .toggle-button::before {
  transform: rotate(-180deg); /* Up arrow */
}

/* Style the nested sublists */
.collapsible-toc .toc-sublist {
  list-style-type: square; /* Options: disc, circle, square */
  padding-left: 1.5em;
  display: none; /* Hidden by default */
}

/* Show sublist when expanded */
.toc-item.expanded .toc-sublist {
  display: block;
}

/* Hover Behavior for Desktop */
@media (min-width: 768px) {
  .toc-header:hover + .toc-sublist {
    display: block;
  }
  
  .toggle-button {
    display: none; /* Hide toggle buttons on desktop */
  }
}

/* Click Behavior for Mobile */
@media (max-width: 767px) {
  .toggle-button {
    display: inline; /* Show toggle buttons on mobile */
  }
}

/* Indicate clickable headers with focus styles */
.collapsible-toc .toc-header:focus {
  outline: 2px solid #000;
}

/* Improve arrow visibility */
.toggle-button::before {
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
  const toggleButtons = document.querySelectorAll('.toggle-button');

  toggleButtons.forEach(button => {
    button.addEventListener('click', function(event) {
      event.stopPropagation(); // Prevent the click from triggering parent elements
      const tocItem = this.closest('.toc-item');
      const isExpanded = tocItem.classList.toggle('expanded');
      this.setAttribute('aria-expanded', isExpanded);
      
      // Optionally, close other expanded items
      /*
      if (isExpanded) {
        document.querySelectorAll('.toc-item').forEach(item => {
          if (item !== tocItem) {
            item.classList.remove('expanded');
            const btn = item.querySelector('.toggle-button');
            if (btn) btn.setAttribute('aria-expanded', false);
          }
        });
      }
      */
    });

    // Allow toggling with Enter and Space keys for accessibility
    button.addEventListener('keydown', function(event) {
      if (event.key === 'Enter' || event.key === ' ') {
        event.preventDefault();
        this.click();
      }
    });
  });
});
</script>

<div class="learning-content">
  <h1>Linear Algebra</h1>

  <a name="linear-algebra"></a>
  <div class="text-block">
    <p>Linear algebra has been a crucial part of my learning journey, especially as I ventured into quantum computing. I started with <a href="https://archive.org/details/gilbert-strang-introduction-to-linear-algebra-fifth-edition/page/504/mode/2up">Gilbert Strang's Introduction to Linear Algebra</a> to build a strong foundation, but I often found myself exploring much deeper concepts and proofs beyond what the book covered. Throughout this process, <a href="https://math.stackexchange.com/users/223599/sooraj-soman">Mathematics Stack Exchange</a> became an invaluable resource for clarifying doubts, solving challenging problems, and learning through engaging discussions with the community.</p>
    <p>These notes are an attempt to organize and share what I’ve learned over the years. They reflect not only the material from Strang's book but also the extended explorations and insights I’ve gained while tackling questions and problems. Having enrolled in Math 6108 Applied Matrix Theory at Missouri S & T, my notes go well beyond the scope of a 6000-level advanced graduate course.</p>
  </div>

  <h2 id="toc">Table of Contents</h2>

  <ol class="collapsible-toc">
    <li class="toc-item">
      <div class="toc-header">
        <button class="toggle-button" aria-expanded="false" aria-label="Expand Book 1">▼</button>
        <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=3')">
          Book 1: Chapter 1 Introduction to Vectors
        </a>
      </div>
      <ul class="toc-sublist">
        <li>
          n Dimensional Cube 
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=22')">
            (Page 22)
          </a>, 
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=36')">
            (Page 36)
          </a>
        </li>
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=57')">
            Chapter 2 Solving Linear Equations
          </a>
        </li>
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=17')">
            Matrix Multiplication Methods (Page 71)
          </a>
        </li>
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=76')">
            Block Matrix (Page 76)
          </a>
        </li>
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=92')">
            Gershgorin Circle Theorem (Page 92)
          </a>
        </li>
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=97')">
            LU Factorization (Page 97)
          </a>
        </li>
      </ul>
    </li>
    
    <li class="toc-item">
      <div class="toc-header">
        <button class="toggle-button" aria-expanded="false" aria-label="Expand Book 2">▼</button>
        <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">
          Book 2: Markov Matrix (Page 17)
        </a>
      </div>
      <ul class="toc-sublist">
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">
            Perron Frobenius Theorem (Page 22)
          </a>
        </li>
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=36')">
            Page Rank Algorithm (Page 36)
          </a>
        </li>
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=62')">
            Neumann Series (Page 62)
          </a>
        </li>
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=88')">
            Vandermonde Matrix (Page 88)
          </a>
        </li>
        <li>
          <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=168')">
            Chapter 3 Vector Spaces and Subspaces
          </a>
        </li>
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
</div>
