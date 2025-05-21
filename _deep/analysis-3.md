---
title: "Semi-Quantum Random Number Generation"
permalink: /deep/analysis-3/
layout: default
classes: wide
footer_fixed: false
---

<!-- Top Navigation Bar (Empty but maintaining design consistency) -->
<div class="learning-topnav">
  <a>&#8203;</a>
  <a>&#8203;</a>  
  <a>&#8203;</a>  
</div>

<!-- Main Content Style -->
<!-- Main Content Style (Updated) -->
<style>
/* Text blocks: no longer indent every first line */
.text-block {
    margin-left: 2%;
    margin-right: 2%;
    text-align: justify;
    margin-bottom: 1rem;
}

/* Only paragraphs get the 50px indent */
.text-block p {
    text-indent: 50px;
    margin-bottom: 1rem;
}

/* Main Title Style */
.text-block {
    margin-left: 2%;
    margin-right: 2%;
    text-align: justify;
    text-indent: 50px;
    margin-bottom: 1rem; /* Add space below */
}
h1 {
    all: unset; /* Reset all styles */
    display: block; /* Ensure it behaves like a block element */
    border-bottom: 0.5px solid #f5f5f5; /* Lighten the underline further */
    padding-bottom: 0.5rem; /* Add space between text and underline */
    font-size: 1.5rem; /* Adjust font size */
    font-weight: bold; /* Ensure it's bold */
    text-align: left; /* Align text to the left */
    margin-left: 2%; /* Align with text block */
    margin-bottom: 1rem; /* Add space below */
}

/* Subheading Styles (Aligned Same as Main Title) */
h2, h3, h4, h5, h6 {
    display: block;
    font-size: 1.3rem;
    font-weight: bold;
    text-align: left;
    margin-left: 0%;
    margin-right: 2%;
    margin-top: 0;           /* remove default top margin */
    margin-bottom: 0.8rem;   /* controlled bottom margin */
    text-indent: 0;
    border-bottom: 0.5px solid #f5f5f5;
}

/* Compact List Styling */
.text-block ol {
    margin-left: 0;
    padding-left: 1.2rem;
    line-height: 1.5;
    margin-bottom: 0.5rem;
}

.text-block ol li {
    margin-bottom: 0.3rem;
    line-height: 1.4;
    font-size: 1rem;
}

/* Sub-lists */
.text-block ul {
    margin-top: 0.2rem;
    margin-bottom: 0.2rem;
    padding-left: 1rem;
    list-style-type: disc;
}

.text-block ul li {
    margin-bottom: 0.2rem;
    font-size: 0.95rem;
    line-height: 1.3;
    text-indent: 0;
}

/* TOC Container Styling */
#toc-container {
    margin-left: 2%;
    margin-right: 2%;
    margin-bottom: 0.5rem;   /* reduced gap below TOC */
}

#toc-container ul {
    list-style-type: square;
    padding-left: 20px;
}

#toc-container li {
    margin-bottom: 0.4rem;
    font-size: 1rem;
}

#toc-container a {
    text-decoration: none;
    color: #2f7f93;
    font-weight: 500;
    transition: color 0.3s;
}

#toc-container a:hover {
    color: #1a5e73;
    text-decoration: underline;
}
.subtitle {
  margin-left: 2%;
  margin-right: 2%;
  font-size: 0.9rem;
  color: #555;
  margin-bottom: 1.5rem;
}
.subtitle a {
  color: #2f7f93;
  text-decoration: none;
}
.subtitle a:hover {
  text-decoration: underline;
}
#further-reading {
  margin-bottom: 3rem;
}
.text-block p.no-indent {
  text-indent: 0;
}
</style>



<!-- Main Heading -->
<h1>
  Semi-Quantum Random Number Generation
  <a href="https://arxiv.org/abs/2210.16427"
     target="_blank" rel="noopener"
     title="Guskind & Krawec, IEEE QCE 2023 / arXiv:2210.16427"
     style="font-size:0.6em; margin-left:0.5em; vertical-align:middle; color:#2f7f93; text-decoration:none;">
    📄
  </a>
</h1>

<div class="text-block">
This page presents a detailed study of the protocol described in the paper <a href="https://arxiv.org/pdf/2210.16427" style="text-decoration: none;">Semi-Quantum Random Number Generation</a> by Guskind and Krawec. The focus is on clarifying the theoretical structure of the protocol, particularly the entanglement-based security proof and the derivation of the secure bit generation rate. The content has been fully reformatted and typeset to improve readability, with mathematical steps and reasoning presented in a structured and accessible way. While no simulations or code implementations are included, the goal is to trace the logic of the protocol with precision and depth.
</div>

<div class="content-container">
  <!-- Table of Contents -->
  <div id="toc-container">
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=sqrng_analysis.pdf#page=1')">SQRNG Protocol</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=sqrng_analysis.pdf#page=3')">Purified SQRNG Protocol</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=sqrng_analysis.pdf#page=4')">e-QRNG Protocol</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=sqrng_analysis.pdf#page=6')">Theorem 1: Mapping SQRNG Attacks to e-QNRG</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=sqrng_analysis.pdf#page=8')">Theorem 1: Proof</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=sqrng_analysis.pdf#page=17')">Secure Bit Rate Analysis</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=sqrng_paper.pdf#page=1')">Original Paper</a></li>
    </ul>
  </div>
  



  <!-- PDF Viewer -->
  <div class="pdf-viewer">
    <iframe src="https://soorajss1729.github.io/pdfjs/viewer.html?file=sqrng_analysis.pdf" width="100%" height="1000px" style="border: none;"></iframe>
  </div>
</div>

<style>
/* General styling */
a {
    text-decoration: none; /* Remove underline for all hyperlinks */
}
  
body {
    padding-bottom: 50px; /* Adds 50px of vertical space at the bottom of the page */
}

.learning-content {
  margin-left: 5%;
  margin-right: 5%;
}

.text-block {
    text-align: justify;
    text-indent: 50px;
}

/* Flexbox container for TOC and PDF viewer */
.content-container {
    display: flex;
    flex-wrap: nowrap;
    gap: 0px;
    margin-left: 2%;
    margin-right: 2%;
    height: 1000px; /* Set a height for the container */
}

/* TOC styling */
#toc-container {
    flex: 1 1 30%; /* TOC takes up 30% of the width */
    max-width: 400px;
    overflow-y: auto; /* Enable vertical scrolling */
    border-right: 0px solid #ddd; /* Optional right border for separation */
    padding-right: 10px; /* Space for scroll bar */
    height: 100%; /* Match the container height */
}

#toc-container details {
  margin-bottom: 1em; /* Add spacing between collapsible sections */
}

#toc-container summary {
  font-weight: bold;
  cursor: pointer;
}

#toc-container ul {
  list-style-type: square;
  padding-left: 20px;
}

/* PDF Viewer styling */
.pdf-viewer {
    flex: 1 1 55%; /* PDF viewer takes up 70% of the width */
    border: 0px solid #ddd;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    padding-left:5%;
    padding-right:5%;    
}


/* Mobile adjustments */
@media (max-width: 768px) {
  .content-container {
    flex-direction: column; /* Stack TOC and viewer vertically */
    height: auto; /* Allow the container height to adjust naturally */
    margin-bottom: 50px; /* Prevent overlap with footer */
  }
  #toc-container {
    max-width: 100%;
    height: auto; /* Adjust height naturally */
  }
  .pdf-viewer {
    max-width: 100%;
    height: calc(100vh - 50px); /* Take up remaining space above footer */
    margin-top: 1rem; /* Add spacing between TOC and PDF viewer */
    flex-grow: 1; /* Ensure it stretches to fill available space */
  }
  footer {
    position: relative;
    bottom: 0;
  }
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function () {
  window.loadPdfPage = function(url) {
    const pdfViewer = document.querySelector('.pdf-viewer iframe');
    if (pdfViewer) {
      pdfViewer.src = url;
      if (window.innerWidth <= 768) {
        setTimeout(() => {
          const pdfSection = document.querySelector('.pdf-viewer');
          if (pdfSection) {
            pdfSection.scrollIntoView({ behavior: 'smooth' });
          }
        }, 300);
      }
    } else {
      console.error("PDF viewer iframe not found.");
    }
  }
});
</script>


