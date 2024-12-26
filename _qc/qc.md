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
  <a href="/grp/">Group Theory</a>
</div>

<style>
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
  <h1>Quantum Computing</h1>

<a name="qc"></a>
<div class="text-block">
 <p>After strengthening my mathematical skills and establishing a solid foundation in linear algebra, I delved into quantum computing through <a href="https://profmcruz.wordpress.com/wp-content/uploads/2017/08/quantum-computation-and-quantum-information-nielsen-chuang.pdf" style="text-decoration: none;">Nielsen and Chuang</a>’s Quantum Computation and Quantum Information. I approached each topic in the book with a keen focus on understanding its mathematical constructs and nuances. Frequently, my curiosity led me to explore beyond the book, engaging with additional materials to broaden my perspective and deepen my understanding. The <a href="https://quantumcomputing.stackexchange.com/users/18369/sooraj-soman" style="text-decoration: none;">Quantum Computing Stack Exchange</a> has been an invaluable resource in navigating these challenges independently, often sparking extended discussions that enriched my understanding. <a href="https://math.stackexchange.com/users/223599/sooraj-soman" style="text-decoration: none;">Mathematics Stack Exchange</a> has similarly played a pivotal role in helping me grasp the mathematical framework of quantum computing concepts.</p>
 
  <p>These notes are an attempt to organize and share what I’ve learned over the years. They encompass not only the material from Nielsen and Chuang’s book but also the extended explorations and insights I’ve gained through tackling complex questions and problems. Having enrolled in CS5001 Introduction to Quantum Computing at Missouri S&T, my notes extend well beyond the scope of a typical 5000-level graduate course.</p>
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
    <summary>Book 1: Introduction to Quantum Computing</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=3')">Postulates of Quantum Mechanics</a></li>
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
  </details>

  <details>
    <summary>Book 2: Density Matrix Formalism</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=3')">Density Matrix (Page 17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=31')">Density Matrix - Unitary Freedom</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=42')">Bloch Sphere</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=55')">Bloch Sphere - Mixed State</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=66')">Partical Trace</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=83')">Why Partical Trace ?</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=99')">Detecting Entanglement</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=111')">Purification</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=126')">EPR and Bell Inequality</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 3: Quantum Computation</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=3')">Single Qubit Gates</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=22')">Rotation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=33')">Single Qubit Unitary as Rotation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=51')">Rotations About Arbitrary Axis</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=57')">Controlled Operations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=72')">No-Cloning Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=80')">Bell States</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=90')">Conditioning on Multiple Qubits</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 4: More Quantum Computation</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=3')">Chapter 4 Exercises</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=9')">Swap and Fredkin Gates</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=22')">$C^n(U)$ Operation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=39')">Quantum Teleportation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=56')">Quantum Measurement Principles</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=66')">Measurement on Bell Basis</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=70')">Measuring an Operator</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=75')">Universal Quantum Gates</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=80')">Two-level Gates are Universal</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 5: Universal Quantum Gates</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc5.pdf#page=4')">Single Qubit and CNOT Gates are Universal</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc5.pdf#page=22')">Approximating Unitary Operators</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc5.pdf#page=33')">Discrete Sets of Universal Operation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc5.pdf#page=35')">Hadamard+$\pi/2$=Single Qubit Unitary</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc5.pdf#page=62')">Hadamard, Phase, CNOT, Toffoli are Universal</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc5.pdf#page=76')">Quantum Circuit Model of Computation</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 6: Simulating Quantum Systems</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc6.pdf#page=3')">Simulations of Quantum Systems</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc6.pdf#page=14')">Baker-Campbell-Hausderff Formula</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc6.pdf#page=34')">Trotter Formula</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc6.pdf#page=54')">Simulating $H=Z_1\otimes Z_2\otimes\cdots\otimes Z_n$</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 7: Quantum Fourier Transform</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=5')">Quantum Parallelism</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=10')">Deutsch's Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=16')">Deutsch-Jozsa Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=31')">Probabilistic Classical Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=35')">Discrete Fourier Transform</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=50')">Quantum Fourier Transform</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=58')">QFT Circuit</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=75')">Inverse QFT</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=77')">Approximating QFT</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=79')">Phase Estimation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=97')">Performance of Phase Estimation</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 8: More Quantum Algorithms</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc8.pdf#page=3')">Order Finding Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc8.pdf#page=39')">Performance of Order Finding</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc8.pdf#page=55')">Period Finding Algorithm</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 9: Hidden Subgroup Problem</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc9.pdf#page=3')">Discrete Logarithm Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc9.pdf#page=16')">The Hidden Subgroup Problem</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 10: Quantum Search</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=4')">Grover's Search Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=11')">Grover Iteration</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=24')">Complexity of Grover's Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=37')">Performance of Grover's Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=46')">Procedure of Grover's Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=72')">Quantum Counting</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 11: </summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=1')">Will Upload Soon !</a></li>
    </ul>
  </details>
  
  <details>
    <summary>Book 12: Quantum Operations</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.pdf#page=5')">Classical Noice</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.pdf#page=17')">Quantum Operations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.pdf#page=23')">Environment and Quantum Operations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.pdf#page=37')">Operator Sum Representation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.pdf#page=63')">Interpretation of Operator Sum Representation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.pdf#page=69')">Non-trace-preserving Operations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.pdf#page=79')">System Environment Models</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.pdf#page=89')">Mocking up a Quantum Operation</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 13: Quantum Noice</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc13.pdf#page=3')">Axiomatic Approach to Quantum Operations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc13.pdf#page=20')">Choi Matrix</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc13.pdf#page=35')">Unitary Freedom in Operator Sum Representation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc13.pdf#page=42')">Theorem 8.3</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc13.pdf#page=57')">Geometry of Single Qubit Operation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc13.pdf#page=68')">Bit Flip and Phase Flip Channels</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc13.pdf#page=83')">Depolarizing Channel</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc13.pdf#page=94')">Amplitude Damping</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc14.pdf#page=3')">Exercises</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 14: Quantum Tomography</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc15.pdf#page=4')">Quantum State Tomography</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc15.pdf#page=19')">Quantum Process Tomography</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc15.pdf#page=23')">Chi Matrix Representation of Quantum Operation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc15.pdf#page=26')">Alternative Method: Choi Matrix</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc15.pdf#page=45')">Quantum Process Tomography for Single Qubit</a></li>
    </ul>
  </details>

  <details>
    <summary>Chapter 9: Distance Measures</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc9.1.pdf#page=4')">Classical Distance Measures</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc9.1.pdf#page=26')">Quantum Trace Distance</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc9.1.pdf#page=34')">Quantum Fidelity</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc9.1.pdf#page=41')">Relationship between Distance Measures</a></li>
    </ul>
  </details>

  <details>
    <summary>Chapter 10: Quantum Error Correction</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=9')">Three Qubit Bit Flip Code</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=34')">Three Qubit Phase Flip Code</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=42')">The Shor Code</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=57')">Stabilizer Formalism</a></li>
    </ul>
  </details>
  
  <details>
    <summary>Chapter 11 (Part 1): Entropy and Information</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=4')">Quantifying Information</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=16')">Rational Behind Log for Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=30')">Shannon Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=40')">Binary Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=56')">Relative Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=67')">Conditional Entropy and Mutual Information</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=77')">Properties of Shannon Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=93')">Data Processing Inequality</a></li>
    </ul>
  </details>

  <details>
    <summary>Chapter 11 (Part 2): Entropy and Information</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=1')">Will Upload Soon !</a></li>
    </ul>
  </details>

  <details>
    <summary>Chapter 11 (Part 3): Entropy and Information</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.3.pdf#page=4')">Lieb's Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.3.pdf#page=24')">Relative Entropy is Jointly Convex</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.3.pdf#page=31')">Conditional Entropy is Concave</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.3.pdf#page=33')">Strong Subadditivity</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.3.pdf#page=43')">Conditioning Reduces Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.3.pdf#page=49')">Subadditivity of Conditional Entropy</a></li>
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

