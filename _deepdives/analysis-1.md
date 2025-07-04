---
title: "A Simple Method for Sampling Random Clifford Operators"
permalink: /deepdives/analysis-1/
layout: default
classes: wide
footer_fixed: false
---

<!-- Top Navigation Bar (Empty but maintaining design consistency) -->
<div class="learning-topnav">
  <a href="/deepdives/">‹ Back</a>
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
  A Simple Method for Sampling Random Clifford Operators
  <a href="https://doi.org/10.1109/QCE52317.2021.00021"
     target="_blank" rel="noopener"
     title="E. van den Berg et al., IEEE Quantum Comput. Eng. (2021)."
     style="font-size:0.6em; margin-left:0.5em; vertical-align:middle; color:#2f7f93; text-decoration:none;">
    📄
  </a>
</h1>

<!-- Table of Contents -->
<div id="toc-container">
  <ul>
    <li><a href="#clifford">The Clifford Group</a></li>
    <li><a href="#algorithm-outline">Approach Overview</a></li>
    <li><a href="#sweep">Detailed Sweep Steps</a></li>
    <li><a href="#code-simulation">Interactive Simulator</a></li>
    <li><a href="#further-reading">Further Reading</a></li>
  </ul>
</div>

<div id="clifford" class="text-block">
  <h2>The Clifford Group</h2>
The Pauli group \( P_n \) on \( n \) qubits is the set of all tensor products of the Pauli matrices \( \{I, X, Y, Z\} \), without any global phase factors or signs:

\[
P_n = \{ P_1 \otimes P_2 \otimes \cdots \otimes P_n | P_i \in \{I, X, Y, Z\} \}.
\]

The Clifford group \( C_n \) is defined as the set of unitary operators that preserve this Pauli group under conjugation:

\[
C_n = \{ U \in U(2^n) \mid \sigma \in \pm P^*_n \implies U \sigma U^\dagger \in P^*_n \}.
\]

where $P^*_n=P_n\backslash\{I^n\}$. i.e., any Clifford transformation maps any Pauli operator to another Pauli operator with the phase. Clifford operators are a fundamental class of unitary operators in quantum computing, widely used for stabilizer states, error correction, and randomized benchmarking. Efficiently sampling random Clifford operators is essential in applications like randomized benchmarking and noise estimation. König and Smolin (2014) showed that
  \[
    |C_n| = 2^{2n^2 + 2n} \prod_{j=1}^n (4^j - 1)\,,
  \]

<div style="margin: 2rem 0; width: 100%;">
  <details style="width: 100%;">
    <summary style="
      display: block;
      text-align: center;
      font-weight: 500;
      cursor: pointer;
      padding: 0.5em 0;
    ">
      ▶️ Proof of the formula for |C<sub>n</sub>|
    </summary>
    <div style="
      padding: 0.75rem 1rem;
      background: #f9f9f9;
      border-left: 3px solid #2f7f93;
      margin-top: 0.5rem;
      width: 100%;
    ">
      The subgroup \( C_{n-1} \) of the Clifford group \( C_n \) is the set of Clifford transformations that leave the last pair \( (X_n, Z_n) \) fixed. The group \( C_n \) is structured as a union of cosets of \( C_{n-1} \), with each coset corresponding to a distinct way of transforming \( (X_n, Z_n) \). 

The operator \( X_n \) can be mapped to any of \( \pm P_n^* \), the set of signed Pauli operators excluding the identity, providing \( 2(4^n - 1) \) distinct choices. Given a specific \( X_n \in \pm P_n^* \), the operator \( Z_n \) must be chosen from the subset of \( \pm P_n^* \) that anti-commutes with \( X_n \). Since each non-identity Pauli operator anti-commutes with exactly half of the signed Pauli operators, this yields \( 4^n \) independent choices for \( Z_n \). These choices are independent because selecting \( X_n \) does not restrict the subsequent choice of \( Z_n \). The total number of ways to assign \( (X_n, Z_n) \) is thus 

\[
2(4^n - 1) 4^n.
\]

Each of these assignments corresponds to a distinct coset of \( C_{n-1} \) in \( C_n \) because each distinct assignment of \( (X_n, Z_n) \) defines a unique transformation of these operators, creating a new way to extend \( C_{n-1} \) to \( C_n \). Since \( C_{n-1} \) is defined as transformations that leave \( (X_n, Z_n) \) fixed, any change in \( (X_n, Z_n) \) defines a transformation not covered by \( C_{n-1} \). Cosets are, by definition, disjoint subsets that partition \( C_n \). As a result, each unique assignment of \( (X_n, Z_n) \) generates a new set of transformations, forming a distinct coset of \( C_{n-1} \). Therefore, the total number of cosets of $C_{n-1}$ in $C_{n}$ is:

\[
[C_n : C_{n-1}] = 2(4^n - 1) 4^n
\]

According to Lagrange's Theorem in group theory, the size of a group \( G \) is the product of the size of any of its subgroups \( H \) and the number of distinct cosets of \( H \) in \( G \). Applying this to the Clifford group \( C_n \), with \( C_{n-1} \) as the subgroup that leaves \( (X_n, Z_n) \) fixed, we have:

\[
|C_n| = [C_n : C_{n-1}] |C_{n-1}|
\]

Therefore, the size of the Clifford group \( C_n \) is:

\begin{align}
|C_n| &= 2(4^n - 1) 4^n |C_{n-1}|\\
&=\prod_{j=1}^n 2(4^j - 1) 4^j\\
&=2^{n^2+2n}\prod_{j=1}^n (4^j-1)
\end{align}

    </div>
  </details>
</div>


and used this to build a bijection between integers \(0 \le k < |C_n|\) and Clifford elements, achieving uniform sampling in \(O(n^3)\) time via symplectic transvections.

  This page focuses on the more direct tableau-based method of Ewout van den Berg (2021), which samples random Clifford operators in \(O(n^2)\) gates and \(O(n\log n)\) depth by streaming localized “sweep” steps.
</div>

<!-- The Approach in This Page -->
<div id="algorithm-outline" class="text-block">
  <h2>Approach Overview</h2>
The algorithm proposed by Ewout van den Berg offers a direct and efficient approach for sampling random Clifford operators using a tableau representation. This method is notable for its simplicity and its capability to directly generate a Clifford circuit without requiring intermediate conversions or complex mappings.
Pauli operators are represented using a binary vector form:
\[ P(x,z) = \prod_{j=1}^{n} i^{x_j z_j} X_j^{x_j} Z_j^{z_j} \]
where $x, z \in \mathbb{F}_2^n$. This allows efficient representation and manipulation of Pauli operators using binary matrices, known as tableaus.
<p class="no-indent">At its core, the method is built around a transformation process known as sweeping. This process systematically converts a set of randomly chosen Pauli operators into a standardized form using Clifford gates. Initially, these Pauli operators are chosen at random and are in a disordered form. The sweeping process then applies a series of Clifford transformations (Hadamard, Phase, and CNOT) to each row of the tableau, gradually converting them into a standard Pauli basis. The final Clifford circuit is essentially the inverse of this sweeping transformation. This means the circuit we generate is the Clifford operator that maps the standard Pauli basis to the initial random Pauli set.</p>
<p class="no-indent">The method uses a tableau representation for Pauli operators. A tableau is a binary matrix where each row represents a Pauli operator. The tableau is divided into two main sections: the X-block and the Z-block. The X-block indicates which qubits have an X component, while the Z-block indicates the Z component. This binary representation makes it easy to manipulate and transform Pauli operators efficiently.</p>
</div>

<!-- Sweep Step: Derivation (Compact, No Line Breaks) -->
<div id="sweep" class="text-block">
  <h2>Detailed Sweep Steps</h2>
The sweeping step is the core of the algorithm, transforming a pair of anticommuting Pauli operators into standard form using Clifford gates:
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
  <h2>Interactive Simulator</h2>

  <!-- toolbox: key-functions toggle + GitHub link side by side -->
  <div id="sim-tools" style="display:flex; align-items:center; gap:1rem; margin:1rem 0;">
    <details style="margin:0;">
      <summary style="display:flex; align-items:center; gap:0.5rem; font-weight:500; cursor:pointer; padding:0.25em 0.5em; border-radius:4px; transition:background-color 0.2s;">
        ▶️ Expand to see the core routines.
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

    <a href="https://github.com/soorajss1729/clifford-sim/blob/main/streamlit_app.py"
       target="_blank" rel="noopener"
       style="display:flex; align-items:center; gap:0.5rem; text-decoration:none; font-weight:500; color:#2f7f93; padding:0.25em 0.5em; border-radius:4px; transition:background-color 0.2s;">
      📂 View full implementation on GitHub
    </a>
  </div>

  <!-- primary call-to-action -->
  <div style="text-align:center; margin:1.5rem 0;">
    <a href="https://soorajss1729-clifford-sim-streamlit-app-baqysj.streamlit.app"
       target="_blank" rel="noopener"
       style="display:inline-block; padding:0.75em 1.5em; background:#2f7f93; color:#fff; border-radius:4px; font-weight:500; text-decoration:none;">
      ▶️ Launch Simulator
    </a>
  </div>

This Python demo implements the tableau‐based “sweep” algorithm from van den Berg’s paper, letting you interactively sample random Clifford operators.
</div>




<!-- Further Reading -->
<div id="further-reading" class="text-block">
  <h3>Further Reading</h3>
For a deeper understanding, refer to the original research paper, as well as other related works that explore Clifford operators, tableau representation, and their applications in quantum computing.
  <ul>
    <li><a href="https://doi.org/10.1109/QCE52317.2021.00021" target="_blank" style="text-decoration: none;">van den Berg, “A Simple Method for Sampling Random Clifford Operators”</a></li>
    <li><a href="https://arxiv.org/abs/2003.09412" target="_blank" style="text-decoration: none;">Bravyi & Maslov, “Hadamard-free circuits expose the structure of the Clifford group”</a></li>
  </ul>
</div>

