---
title: "Linear Algebra"
permalink: /grp/
layout: default
classes: wide
---

<div class="learning-topnav">
  <a href="/learning/">Back</a>
  <a href="/linalg/">Linear Algebra</a>  
  <a href="/qc#">Quantum Computing</a>  
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
  <h1>Group Theory</h1>


<div class="text-block">
  <p>I began studying group theory after enrolling in Math 5105 Modern Algebra I at Missouri S&T, taught by <a href="https://sites.mst.edu/cjlungstrum/" style="text-decoration: none;">Dr. Clayton Lungstrum</a>. His clear and engaging teaching style made the subject both accessible and inspiring, and I consider him the best instructor I’ve had at this university. While the course provided a strong foundation, much of my deeper understanding came from self-study and working through <a href="https://edisciplinas.usp.br/pluginfile.php/5409004/mod_resource/content/2/John%20B.%20Fraleigh%2C%20Victor%20J.%20Katz%20-%20A%20first%20course%20in%20abstract%20algebra-Addison-Wesley%20%282003%29%20%281%29.pdf" style="text-decoration: none;">A First Course in Abstract Algebra by John B. Fraleigh (7th Edition)</a>.</p>
 
 <p>My notes include detailed proofs and explanations from the textbook, insights gained from solving problems, and explorations of challenging topics tackled independently. They also feature a dedicated section for problems with solutions and the project report where I contributed to the final proof for the Simplicity of the Alternating Group $A_n$. These sections include notes on number theory and cryptography, topics I studied independently alongside related areas in mathematics and quantum computing.</p>
</div>

<div class="content-container">
  <!-- Table of Contents -->
  <div id="toc-container">


  <details>
    <summary>Section 1: Introduction to Groups</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=3')">Introduction</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=7')">Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=22')">Binary Operations</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=26')">Properties of Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=39')">Three Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=57')">Subgroups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=64')">Nontrivial Subgroup of $(\mathbb{Z},+)$ is $m\mathbb{Z}$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=68')">Properties of Subgroups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf#page=77')">Cyclic Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-2.pdf#page=3')">Cyclic Groups</a></li>
    </ul>
  </details>


  <details>
    <summary>Section 2: Factor Groups and Homomorphisms</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=1')">Finitely Generated Abelian Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=4')">Homomorphisms</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=10')">Factor Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=16')">Fundamental Homomorphism Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=23')">Converse of Lagrange's Theorem is False</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=27')">Simple Groups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=29')">Maximal Normal Subgroup</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=30')">Center and Commutator Subgroups</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 3: Group Action on a Set</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=33')">G-Sets</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=35')">Isotropy Subgroups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=40')">Application of G-Sets to Counting</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-2.pdf#page=42')">Burnside's Formula</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 4: Advanced Group Theory</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=1')">First Isomorphism Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=4')">Join of Subgroups</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=6')">Second Isomorphism Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=10')">Third Isomorphism Theorem</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 5: Series of Groups</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=13')">Normal(Subnormal) Series</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=15')">Refinement of a Series</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=16')">Butterfly Lemma</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=17')">Schreier Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=22')">Composition and Principal Series</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=24')">Jordan-Holder Theorem</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 6: Sylow Theorems</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=29')">Introduction</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=33')">Cauchy's Theorem and p-Group</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=37')">Normalizer of a Subgroup</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=41')">First Sylow Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=44')">Sylow p-Subgroup</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=45')">Second Sylow Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-note-3.pdf#page=47')">Third Sylow Theorem</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 7: Problem Set</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=la2.pdf#page=1')">Will Upload Soon !</a></li>
    </ul>
  </details>

  <details>
    <summary>Section 8: Coursework Project</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-proj-report.pdf#page=3')">$A_n$ is Simple for $n\ge 5$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-proj-ppt.pdf#page=10')">Project Presentation</a></li>
    </ul>
  </details>
  <details>
    <summary>Number Theory: Book 1</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=nmbr-qca4-2.pdf#page=1')">Will upload soon !</a></li>
    </ul>
  </details>
  
  <details>
    <summary>Number Theory: Book 2</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=nmbr-qca4-2.pdf#page=3')">Euler's Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=nmbr-qca4-2.pdf#page=27')">Reduction of Factoring to Order Finding</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=nmbr-qca4-2.pdf#page=52')">Continued Fractions</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=nmbr-qca4-2.pdf#page=65')">Convergents and Their Properties</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=nmbr-qca4-2.pdf#page=78')">Dirichlet's Approximation Theorem</a></li>
    </ul>
  </details>
  <details>
    <summary>Cryptography</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=rsa.pdf#page=3')">Public Key Cryptography</a></li>        
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=rsa.pdf#page=9')">RSA Cryptosystem</a></li>   
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=rsa.pdf#page=20')">Diffie-Hellman Key Exchange</a></li>   
    </ul>
  </details>    
  </div>
  
<script>
    // Handle the click event for all TOC links
    document.addEventListener('DOMContentLoaded', () => {
        const links = document.querySelectorAll('a[href="javascript:void(0)"]');
        
        links.forEach(link => {
            link.addEventListener('click', function (event) {
                event.preventDefault(); // Prevent default link behavior
                const url = this.getAttribute('onclick').match(/'([^']+)'/)[1]; // Extract the URL from the onclick attribute
                loadPdfPage(url);
            });
        });
    });

    function loadPdfPage(url) {
        const pdfViewer = document.querySelector('.pdf-viewer iframe');
        if (pdfViewer) {
            pdfViewer.src = url; // Load the PDF into the iframe

            // For smaller screens: Scroll the page to the PDF viewer
            if (window.innerWidth <= 768) {
                scrollToElement('.pdf-viewer');
            }
        } else {
            console.error('PDF viewer iframe not found!');
        }
    }

    // Smooth scrolling function
    function scrollToElement(selector) {
        const element = document.querySelector(selector);
        if (element) {
            window.scrollTo({
                top: element.offsetTop, 
                behavior: 'smooth'
            });
        }
    }
</script>


  <!-- PDF Viewer -->
  <div class="pdf-viewer">
    <iframe src="https://soorajss1729.github.io/pdfjs/viewer.html?file=grp-qca2-1.pdf" width="100%" height="1000px" style="border: none;"></iframe>
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
