---
title: "A Simple Method for Sampling Random Clifford Operators"
permalink: /explorations/analysis-1/
layout: default
classes: wide
---

<!-- Top Navigation Bar (Empty but maintaining design consistency) -->
<div class="learning-topnav">
  <a>&#8203;</a>
  <a>&#8203;</a>  
  <a>&#8203;</a>  
</div>

<!-- Main Content Style -->
<style>
.text-block {
    margin-left: 2%;
    margin-right: 2%;
    text-align: justify;
    margin-bottom: 1rem;
    /* text-indent: 50px;  ← remove this */
}

/* Main Title Style */
h1 {
    all: unset;
    display: block;
    font-size: 1.5rem;
    font-weight: bold;
    text-align: left;
    margin-left: 2%;
    margin-right: 2%;
    margin-bottom: 1rem;
    border-bottom: 0.5px solid #f5f5f5;
}

/* Subheading Styles (Aligned Same as Main Title) */
h2, h3, h4, h5, h6 {
    display: block;
    font-size: 1.3rem;
    font-weight: bold;
    text-align: left;
    margin-left: 2%;
    margin-right: 2%;
    margin-bottom: 0.8rem; /* Slightly reduced spacing */
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
.text-block p {
    text-indent: 50px;    /* only paragraphs get indented */
    margin-bottom: 1rem;
}


.text-block ol li {
    margin-bottom: 0.3rem; /* Reduced space between main list items */
    line-height: 1.4;
    font-size: 1rem;
}

.text-block ul {
    margin-top: 0.2rem;
    margin-bottom: 0.2rem;
    padding-left: 1rem;
    list-style-type: disc;
}

.text-block ul li {
    margin-bottom: 0.2rem; /* Reduced space between sub-list items */
    font-size: 0.95rem;    /* Slightly smaller font for sub-list */
    line-height: 1.3;
    text-indent: 0;
}

/* TOC Container Styling */
#toc-container {
    margin-left: 2%;
    margin-right: 2%;
    padding-bottom: 1rem;
}

#toc-container ul {
    list-style-type: square;
    padding-left: 20px;
}

#toc-container li {
    margin-bottom: 0.4rem; /* Slightly reduced spacing for TOC */
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
</style>


<!-- Main Heading -->
<h1>A Simple Method for Sampling Random Clifford Operators</h1>

<!-- Table of Contents -->
<div id="toc-container">
  <ul>
    <li><a href="#introduction">Introduction</a></li>
    <li><a href="#algorithm-outline">Algorithm Outline</a></li>
    <li><a href="#sweep-step">Detailed Derivation of the Sweep Step</a></li>
    <li><a href="#code-simulation">Code & Simulation</a></li>
    <li><a href="#further-reading">Further Reading</a></li>
  </ul>
</div>

<div id="introduction" class="text-block">
  <h2>Introduction</h2>
  Clifford operators are a fundamental class of unitary operators in quantum computing, widely used for stabilizer states, error correction, and randomized benchmarking. Efficiently sampling random Clifford operators is essential in applications like randomized benchmarking and noise estimation.

  König and Smolin (2014) showed that
  \[
    |C_n| = 2^{2n^2 + 2n} \prod_{j=1}^n (4^j - 1)\,,
  \]
  and used this to build a bijection between integers \(0 \le k < |C_n|\) and Clifford elements, achieving uniform sampling in \(O(n^3)\) time via symplectic transvections.

  This page focuses on the more direct tableau-based method of Ewout van den Berg (2021), which samples random Clifford operators in \(O(n^2)\) gates and \(O(n\log n)\) depth by streaming localized “sweep” steps.
</div>

<!-- The Approach in This Page -->
<div id="algorithm-outline" class="text-block">
  <h2>The Approach in The Paper</h2>
  <p>The algorithm proposed by Ewout van den Berg offers a direct and efficient approach for sampling random Clifford operators using a tableau representation. This method is notable for its simplicity and its capability to directly generate a Clifford circuit without requiring intermediate conversions or complex mappings.</p>
Pauli operators are represented using a binary vector form:
\[ P(x,z) = \prod_{j=1}^{n} i^{x_j z_j} X_j^{x_j} Z_j^{z_j} \]
where $x, z \in \mathbb{F}_2^n$. This allows efficient representation and manipulation of Pauli operators using binary matrices, known as tableaus.
  <p>At its core, the method is built around a transformation process known as sweeping. This process systematically converts a set of randomly chosen Pauli operators into a standardized form using Clifford gates. Initially, these Pauli operators are chosen at random and are in a disordered form. The sweeping process then applies a series of Clifford transformations (Hadamard, Phase, and CNOT) to each row of the tableau, gradually converting them into a standard Pauli basis. The final Clifford circuit is essentially the inverse of this sweeping transformation. This means the circuit we generate is the Clifford operator that maps the standard Pauli basis to the initial random Pauli set.</p>
<p>The method uses a tableau representation for Pauli operators. A tableau is a binary matrix where each row represents a Pauli operator. The tableau is divided into two main sections: the X-block and the Z-block. The X-block indicates which qubits have an X component, while the Z-block indicates the Z component. This binary representation makes it easy to manipulate and transform Pauli operators efficiently.</p>
</div>

<!-- Sweep Step: Derivation (Compact, No Line Breaks) -->
<div id="sweep" class="text-block">
  <h2>The Sweeping Step Explained</h2>
  <p>The sweeping step is the core of the algorithm, transforming a pair of anticommuting Pauli operators into standard form using Clifford gates:</p>
  <ol>
    <li><strong>Clear the Z-block of the First Row:</strong> For each index \( j \) where \( z_{aj} = 1 \): <ul><li>Apply a Hadamard gate \( H(j) \) if \( x_{aj} = 0 \), swapping \( Z \) and \( X \) components.</li><li>Apply a Phase gate \( S(j) \) if \( x_{aj} = 1 \), which modifies \( Y \) into \( X \).</li></ul> This ensures the \( Z \)-block of the first row is cleared, leaving only \( X \)-components.</li>
    
    <li><strong>Collapse the X-block of the First Row:</strong> Identify all indices \( j \) with \( x_{aj} = 1 \). Use CX gates to pair these active \( X \)-components until only one remains. If the final active \( X \)-component is not at the first qubit, apply a three-CX "swap" sequence to move it.</li>
    
    <li><strong>Move Support to the Target Qubit:</strong> If the remaining active \( X \)-component is not on the target qubit \( i \), perform a three-CX "swap" sequence to move it.</li>
    
    <li><strong>Normalize the Second Row:</strong> If the second row is already in \( \pm Z_1 \) form, this step is skipped. Otherwise: <ul><li>Apply a Hadamard \( H(1) \) to the first column, converting \( X \) to \( Z \) and vice versa.</li><li>Re-apply Steps 1 and 2 to the second row: <ul><li>Clear the \( Z \)-block using \( H \) or \( S \) as needed.</li><li>Collapse the \( X \)-block using CX gates until only one active \( X \)-component remains.</li></ul></li><li>Apply another \( H(1) \) to ensure the second row is in \( \pm Z_1 \) form.</li></ul> This step is crucial for ensuring the second row is aligned and properly standardized.</li>
    
    <li><strong>Clear Sign Bits:</strong> Adjust the sign bits of the rows for consistent phase tracking: <ul><li>If \( s_a = 0 \) and \( s_b = 1 \), apply \( X_1 \), which commutes with \( X_1 \) and anticommutes with \( Z_1 \).</li><li>If \( s_a = 1 \), apply \( Y_1 \) if \( s_b = 1 \) and \( Z_1 \) otherwise.</li></ul> This ensures consistent phase alignment across the rows.</li>
    
    <li><strong>Repeat for All Pairs:</strong> This sweeping process is repeated for each pair of rows in the tableau, ensuring that all rows are transformed into a consistent, standardized form.</li>
  </ol>
</div>


<div id="code-simulation" class="text-block">
  <h2>Interactive Random Clifford Operator Generator</h2>

  <!-- Collapsible key-functions snippet -->
  <details style="margin: 1rem 0;">
    <summary style="cursor: pointer; font-weight: 500;">
      ▶️ Show key Python functions
    </summary>
    <pre><code>def anticom_rows_gen(k):
    """Generate two random binary rows that anticommute."""
    found = False
    while not found:
        r1 = np.random.randint(0, 2, size=2*k+1)
        r2 = np.random.randint(0, 2, size=2*k+1)
        ip = (r1[::2] @ r2[1::2] + r1[1::2] @ r2[::2]) % 2
        if ip == 1:
            found = True
    return r1, r2

def clear_z_block(row, k, sx, sz, gates):
    """Clear the Z-block of one row using H or S gates."""
    for j in range(k):
        if sz[row, j]:
            if not sx[row, j]:
                gates.append(("h", j))
                sx[:, j], sz[:, j] = sz[:, j].copy(), sx[:, j].copy()
            else:
                gates.append(("s", j))
                sz[:, j] ^= sx[:, j]

def sweep_x_to_pivot(row, k, sx, sz, gates):
    """Collapse all X’s in the row down to a single pivot via CX gates."""
    J = [j for j in range(k) if sx[row, j]]
    while len(J) > 1:
        a, b = J[0], J[1]
        gates.append(("cx", a, b))
        sx[:, b] ^= sx[:, a]
        J = J[2:] + ([a] if len(J) % 2 else [])
    if J and J[0] != 0:
        for (c, t) in [(0, J[0]), (J[0], 0), (0, J[0])]:
            gates.append(("cx", c, t))
            sx[:, t] ^= sx[:, c]
</code></pre>
  </details>

  <p>
    <a href="https://github.com/soorajss1729/clifford-sim/blob/main/streamlit_app.py"
       target="_blank" rel="noopener"
       style="font-size:0.9rem; text-decoration:none;">
      📂 View full implementation on GitHub
    </a>
  </p>

  <div style="text-align:center; margin:1.5rem 0;">
    <a href="https://soorajss1729-clifford-sim-streamlit-app-baqysj.streamlit.app"
       target="_blank" rel="noopener"
       style="display:inline-block;
              padding:0.75em 1.5em;
              background:#2f7f93;
              color:#fff;
              border-radius:4px;
              font-weight:500;
              text-decoration:none;">
      ▶️ Launch Simulator
    </a>
  </div>

  <p>Here, you can explore a Python implementation of the algorithm for sampling random Clifford operators. The code is explained in a step-by-step manner, with key functions highlighted.</p>
</div>



<!-- Further Reading -->
<div id="further-reading" class="text-block">
  <h3>Further Reading</h3>
  <p>For a deeper understanding, refer to the original research paper, as well as other related works that explore Clifford operators, tableau representation, and their applications in quantum computing.</p>
  <ul>
    <li><a href="https://doi.org/10.1109/QCE52317.2021.00021" target="_blank">van den Berg, “A Simple Method for Sampling Random Clifford Operators”</a></li>
    <li><a href="https://arxiv.org/abs/2003.09412" target="_blank">Bravyi & Maslov, “Hadamard-free circuits expose the structure of the Clifford group”</a></li>
  </ul>
</div>

