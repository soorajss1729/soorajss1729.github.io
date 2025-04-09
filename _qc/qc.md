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
</style>
  <h1>Quantum Computing</h1>

<div class="text-block">
 <p>After strengthening my mathematical skills and establishing a solid foundation in linear algebra, I delved into quantum computing through <a href="https://profmcruz.wordpress.com/wp-content/uploads/2017/08/quantum-computation-and-quantum-information-nielsen-chuang.pdf" style="text-decoration: none;">Nielsen and Chuang</a>’s Quantum Computation and Quantum Information. I approached each topic in the book with a keen focus on understanding its mathematical constructs and nuances. Frequently, my curiosity led me to explore beyond the book, engaging with additional materials to broaden my perspective and deepen my understanding. The <a href="https://quantumcomputing.stackexchange.com/users/18369/sooraj-soman" style="text-decoration: none;">Quantum Computing Stack Exchange</a> has been an invaluable resource in navigating these challenges independently, often sparking extended discussions that enriched my understanding. <a href="https://math.stackexchange.com/users/223599/sooraj-soman" style="text-decoration: none;">Mathematics Stack Exchange</a> has similarly played a pivotal role in helping me grasp the mathematical framework of quantum computing concepts.</p>
 
  <p>These notes are an attempt to organize and share what I’ve learned over the years. They encompass not only the material from Nielsen and Chuang’s book but also the extended explorations and insights I’ve gained through tackling complex questions and problems. Having enrolled in CS5001 Introduction to Quantum Computing at Missouri S&T, my notes extend well beyond the scope of a typical 5000-level graduate course.</p>
</div>

<div class="content-container">
  <!-- Table of Contents -->
  <div id="toc-container">
    
  <details>
    <summary>Book 1: Introduction to Quantum Computing</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=3')">Postulates of Quantum Mechanics (p.3)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=46')">Distinguishing Quantum States (p.46)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=56')">Projective Measurement (p.56)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=73')">POVM Measurement (p.73)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=93')">General Measurement=Projective+Unitary</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=106')">Superdense Coding (p.106)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=121')">Tensor Product (p.121)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=165')">Multipartite System (p.165)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=182')">Schmidt Decomposition (p.182)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf#page=191')">Quantum Measurement Revisited (p.191)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 2: Density Matrix Formalism</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=3')">Density Matrix (p.17)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=31')">Density Matrix - Unitary Freedom</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=42')">Bloch Sphere (p.42)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=55')">Bloch Sphere - Mixed State</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=66')">Partical Trace (p.66)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=83')">Why Partical Trace ? (p.83)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=99')">Detecting Entanglement (p.99)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=111')">Purification (p.111)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc2.pdf#page=126')">EPR and Bell Inequality (p.126)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 3: Quantum Computation</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=3')">Single Qubit Gates (p.3)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=22')">Rotation (p.22)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=33')">Single Qubit Unitary as Rotation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=51')">Rotations About Arbitrary Axis</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=57')">Controlled Operations (p.57)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=72')">No-Cloning Theorem (p.72)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=80')">Bell States (p.80)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc3.pdf#page=90')">Conditioning on Multiple Qubits (p.90)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 4: More Quantum Computation</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=3')">Chapter 4 Exercises (p.3)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=9')">Swap and Fredkin Gates (p.9)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=22')">$C^n(U)$ Operation (p.22)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=39')">Quantum Teleportation (p.39)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=56')">Quantum Measurement Principles (p.56)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=66')">Measurement on Bell Basis (p.66)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=70')">Measuring an Operator (p.70)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc4.pdf#page=75')">Universal Quantum Gates (p.75)</a></li>
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
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc6.pdf#page=34')">Trotter Formula (p.34)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc6.pdf#page=54')">Simulating $H=Z_1\otimes Z_2\otimes\cdots\otimes Z_n$</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 7: Quantum Fourier Transform</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=5')">Quantum Parallelism (p.5)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=10')">Deutsch's Algorithm (p.10)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=16')">Deutsch-Jozsa Algorithm (p.16)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=31')">Probabilistic Classical Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=35')">Discrete Fourier Transform (p.35)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=50')">Quantum Fourier Transform (p.50)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=58')">QFT Circuit (p.58)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=75')">Inverse QFT (p.75)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=77')">Approximating QFT (p.77)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=79')">Phase Estimation (p.79)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc7.pdf#page=97')">Performance of Phase Estimation (p.97)</a></li>
    </ul>
  </details>

  <details>
    <summary>Book 8: More Quantum Algorithms</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc8.pdf#page=3')">Order Finding Algorithm (p.3)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc8.pdf#page=39')">Performance of Order Finding (p.39)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc8.pdf#page=55')">Period Finding Algorithm (p.55)</a></li>
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
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=4')">Grover's Search Algorithm (p.4)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=11')">Grover Iteration (p.11)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=24')">Complexity of Grover's Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=37')">Performance of Grover's Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=46')">Procedure of Grover's Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.pdf#page=72')">Quantum Counting (p.72)</a></li>
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
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=9')">Three Qubit Bit Flip Code (p.9)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=34')">Three Qubit Phase Flip Code (p.34)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=42')">The Shor Code (p.42)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=57')">Theory of Error Correction (p.57)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=63')">Classical linear Codes (p.63)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=80')">Dual Construction (p.80)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=83')">CSS Codes (p.83)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=93')">Steane Code (p.93)</a></li>      
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc10.1.pdf#page=96')">Stabilizer Formalism (p.96)</a></li>            
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
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=3')">Von Neumann Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=8')">Complex Logarithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=12')">Quantum Relative Entropy</a></li>            
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=16')">Klein's Inequality</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=21')">Contunuity of Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=43')">Properties Von Neumann Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=46')">$AB$ is pure state$\implies S(A)=S(B)$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=52')">Joint Entropy Theorem</a></li>      
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=54')">Entropy of Tensor Product</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=59')">Entanglement and Negative Conditional Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=60')">Measurement and Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=61')">Projective Measurement Increases Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.1.pdf#page=65')">	Generalized Measurement can Decrease Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=66')">Subadditivity</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=72')">Triangle Inequality</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=74')">Concavity of Entropy</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=80')">Entropy of a Mixture of States</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc11.2.pdf#page=87')">Strong Subadditivity</a></li>
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
  <details>
    <summary>Chapter 12 : Quantum Key Distribution</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.1.pdf#page=4')">The BB84 protocol</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.1.pdf#page=8')">The B92 protocol</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=qc12.1.pdf#page=10')">The EPR protocol</a></li>
    </ul>
  </details>  
</div>



  <!-- PDF Viewer -->
  <div class="pdf-viewer">
    <iframe src="https://soorajss1729.github.io/pdfjs/viewer.html?file=qc1.pdf" width="100%" height="1000px" style="border: none;"></iframe>
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
    height: 1000px; /* Use full viewport height */
}

/* TOC styling */
#toc-container {
    flex: 1 1 45%; /* TOC takes up 30% of the width */
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


