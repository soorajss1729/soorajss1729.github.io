---
title: "Linear Algebra"
permalink: /linalg/
layout: default
classes: wide
---

<div class="learning-topnav">
  <a href="/learning/">Back</a>
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
  <h1>Linear Algebra</h1>

<a name="linear-algebra"></a>
<div class="text-block">
 <p>Linear algebra has been a crucial part of my learning journey, especially as I ventured into quantum computing. I started with <a href="https://archive.org/details/gilbert-strang-introduction-to-linear-algebra-fifth-edition/page/504/mode/2up">Gilbert Strang's Introduction to Linear Algebra</a> to build a strong foundation, but I often found myself exploring much deeper concepts and proofs beyond what the book covered. Throughout this process, <a href="https://math.stackexchange.com/users/223599/sooraj-soman">Mathematics Stack Exchange</a> became an invaluable resource for clarifying doubts, solving challenging problems, and learning through engaging discussions with the community.</p>
 <p>These notes are an attempt to organize and share what I’ve learned over the years. They reflect not only the material from Strang's book but also the extended explorations and insights I’ve gained while tackling questions and problems. Having enrolled in Math 6108 Applied Matrix Theory at Missouri S & T, my notes go well beyond the scope of a 6000-level advanced graduate course.</p>
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
    <summary>Book 1: Introduction to Vectors</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=3')">Chapter 1: Introduction to Vectors</a></li>
      <li>
        n Dimensional Cube
        <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=22')">(Page 22)</a>,
        <a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=36')">(Page 36)</a>
      </li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=57')">Chapter 2: Solving Linear Equations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=71')">Matrix Multiplication Methods (Page 71)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=76')">Block Matrix (Page 76)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=92')">Gershgorin Circle Theorem (Page 92)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf#page=97')">LU Factorization (Page 97)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 2: Markov Process</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=36')">Page Rank Algorithm (Page 36)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=62')">Neumann Series (Page 62)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=88')">Vandermonde Matrix (Page 88)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=168')">Chapter 3: Vector Spaces and Subspaces</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 3: Subspaces Continue</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 4: Advanced Topics</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la4.pdf#page=3')">N(A)=N(rref(A))</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la4.pdf#page=5')">Fundamental Theorem: Part 1</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la4.pdf#page=15')">Rank 2=Rank 1+Rank 1</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la4.pdf#page=62')">Rank($A^TA$)=Rank(A)=Rank($A^T$)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la4.pdf#page=105')">$W_1\cap W_2$ and $W_1+W_2$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la4.pdf#page=108')">$dim(W_1\cap W_2)=dim(W_1)+dim(W_2)-dim(W_1\cap W_2)$ </a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la4.pdf#page=113')">$W_1\oplus W_2$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la4.pdf#page=118')">$W_1+W_2=span(W_1\cap W_2)$ and $W_1+W_2$</a></li>

    </ul>
  </details>

  <details>
    <summary>Book 5: Advanced Topics</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la5.pdf#page=39')">Chapter 4: Orthogonality</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la5.pdf#page=48')">Fundamental Theorem: Part 2</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la5.pdf#page=57')">Projection</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la5.pdf#page=90')">Projection on Subspace</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la5.pdf#page=102')">Least Square Approximation</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 6: Chapter 4 Continue</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la6.pdf#page=3')">Chapter 4 Continue...</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la6.pdf#page=6')">Householder Reflection</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la6.pdf#page=11')">Projection using Orthogonal Bases</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la6.pdf#page=16')">Gram Schmidt Process</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la6.pdf#page=29')">QR Decomposition: Givens Rotations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la6.pdf#page=32')">QR Decomposition: Householder Reflections</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la6.pdf#page=54')">Fredholm's Alternative</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 7: Chapter 6 Eigenvalues and Eigenvectors</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 8: Advanced Topics</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 9: Advanced Topics</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 10: Advanced Topics</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 11: Advanced Topics</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 12: Fourier Series, Transform and Delta Function</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 13: Legendre and Hermite Polynomials</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 14: Laguerre and Bessel Functions</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 15: Complex Vectors - Cryptography</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 16: Encryption - Probability</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 17: Advanced Topics</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 18: Advanced Topics</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=17')">Markov Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=22')">Perron Frobenius Theorem (Page 22)</a></li>
    </ul>
  </details>

</div>





<div id="pdf-viewer-container" style="width: 100%; display: flex; justify-content: center;">
  <iframe id="pdf-viewer"
    src="https://soorajss1729.github.io/pdfjs/viewer.html?file=la1.pdf&zoom=110"
    style="width: 210mm; height: 297mm; border: none;">
  </iframe>
</div>

