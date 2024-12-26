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
a {
    text-decoration: none; /* Remove underline for all hyperlinks */
}
body {
    padding-bottom: 50px; /* Adds 50px of vertical space at the bottom of the page */
}
h2 {
  margin-top: 15px;
  border-bottom: 1px solid #ddd; /* Add a subtle underline */
  padding-bottom: 0.5rem; /* Add space between text and underline */
}
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
 <p>Linear algebra has been a crucial part of my learning journey, especially as I ventured into quantum computing. I started with <a href="https://archive.org/embed/gilbert-strang-introduction-to-linear-algebra-fifth-edition" style="text-decoration: none;">Gilbert Strang's Introduction to Linear Algebra</a> to build a strong foundation, but I often found myself exploring much deeper concepts and proofs beyond what the book covered. Throughout this process, <a href="https://math.stackexchange.com/users/223599/sooraj-soman" style="text-decoration: none;">Mathematics Stack Exchange</a> became an invaluable resource for clarifying doubts, solving challenging problems, and learning through engaging discussions with the community.</p>
 <p>These notes are an attempt to organize and share what I’ve learned over the years. They reflect not only the material from Strang's book but also the extended explorations and insights I’ve gained while tackling questions and problems. Having enrolled in Math 6108 Applied Matrix Theory at Missouri S&T, my notes go well beyond the scope of a typical 6000-level advanced graduate course.</p>
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
    <summary>Book 2: Markov Process - Subspaces</summary>
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
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la3.pdf#page=3')">NullSpace</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la3.pdf#page=12')">Reduced Row Echelon Form</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la3.pdf#page=19')">Rank of Matrix</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la3.pdf#page=21')">Rank 1 Matrix</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la3.pdf#page=30')">Complete Solution to $Ax=b$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la3.pdf#page=38')">Fredholm's Alternative</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 4: Intersection, Union, and Sum</summary>
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
    <summary>Book 5: Orthogonality</summary>
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
    <summary>Book 6: Orthogonality Continue</summary>
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
    <summary>Book 7: Eigenvalues and Eigenvectors</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la7.pdf#page=10')">Chapter 6 Eigenvalues and Eigenvectors</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la7.pdf#page=3')">Diagonalizing a Matrix</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la7.pdf#page=43')">Similar Matrices</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la7.pdf#page=44')">Fibonacci Numbers</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la7.pdf#page=60')">System of Differential Equations</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 8: Differential Equations Continue</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la8.pdf#page=3')">Difference Equations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la8.pdf#page=24')">Leapfrog Method</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la8.pdf#page=37')">Symmetric Matrices</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la8.pdf#page=45')">Schur's Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la8.pdf#page=53')">Positive Definite Matrix</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la8.pdf#page=59')">Square Root of Matrix</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 9: Singular Value Decomposition</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la9.pdf#page=3')">Chapter 6 Exercise</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la9.pdf#page=85')">Singular Value Decomposition (Page 85)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la9.pdf#page=114')">Spectral Norm</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 10: SVD Continue</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la10.pdf#page=3')">Geometry of SVD</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la10.pdf#page=6')">Spectral Norm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la10.pdf#page=18')">Echart Young Mirsky Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la10.pdf#page=23')">Polar Decomposition</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la10.pdf#page=30')">Condition Number</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la10.pdf#page=55')">Pseudo Inverse</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la10.pdf#page=64')">Pseudo Inverse - Projection</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la10.pdf#page=30')">Least Square - Dependent Columns</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 11: Linear Transformation</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la11.pdf#page=3')">Chapter 8: Linear Transformations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la11.pdf#page=26')">Change of Basis</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la11.pdf#page=71')">Jordan Canonical Form</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la11.pdf#page=79')">Fillipov's Inductive Proof</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la11.pdf#page=89')">Matrix Exponential</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la11.pdf#page=94')">Non-homogenious Differential Equation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la11.pdf#page=104')">Basis for Function Space</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 12: Fourier Series, Transform and Delta Function</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la12.pdf#page=3')">Orthogonal Basis for Function Space</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la12.pdf#page=9')">Fourier Series</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la12.pdf#page=31')">Fourier Transform</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la12.pdf#page=45')">Delta Function</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la12.pdf#page=64')">Discrete Fourier Transform</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la12.pdf#page=82')">Fast Fourier Transform</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la12.pdf#page=85')">DIT Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la12.pdf#page=103')">DIF Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la12.pdf#page=108')">Efficiency of FFT Algorithm</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 13: Legendre and Hermite</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=3')">Legendre Polynomials</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=9')">Legendre Differential Equation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=22')">Generating Function</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=27')">Recurrence Relations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=34')">Orthogonality Relations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=40')">Completeness</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=44')">Rodrigues' Formula</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=50')">Hermite Polynomials</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=64')">Generating Function</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=68')">Recurrence Relation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=73')">Rodrigues' Formula</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=75')">Orthogonality Relations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=80')">Normalized Hermite Functions</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=84')">Raising and Lowering Functions</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la13.pdf#page=9')">1D Harmonic Oscillator</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 14: Laguerre, Bessel and Chebyshev</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=3')">Laguere's Polynomials</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=9')">Generating Function</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=14')">Rodrigue's Formula</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=17')">Rodrigue's Formula</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=22')">Bessel's Functions</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=40')">Recurrence Relations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=44')">Generating Function</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=56')">Chebyshev Polynomials</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=70')">Recurrence Formula</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=74')">Rodrigue's Formula</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la14.pdf#page=78')">Isomorphism of Vector Space</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 15: Complex Vectors - Cryptography</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la15.pdf#page=3')">Linear Transformations Exercise</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la15.pdf#page=57')">Complex Vectors and Matrices</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la15.pdf#page=92')">Linear Algebra for Cryptography</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 16: Encryption - Probability</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la16.pdf#page=3')">Encryption with Hill Cipher</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la16.pdf#page=8')">Finite Fields</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la16.pdf#page=31')">Linear Algebra in Probability and Statistics</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la16.pdf#page=35')">Bessel's Correction</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la16.pdf#page=47')">Continuous Probability Distribution</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la16.pdf#page=56')">Normal Distribution</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la16.pdf#page=68')">Stirling's Formula</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la16.pdf#page=72')">Wallis' Formula</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 17: Probability and Statistics Continue</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la17.pdf#page=3')">Covariance and Joint Probability</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la17.pdf#page=37')">Correlation Matrix</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la17.pdf#page=46')">Multivariate Gaussian</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la17.pdf#page=55')">Weighted Least Squares</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la18.pdf#page=3')">Probability and Statistics Exercise</a></li>
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

