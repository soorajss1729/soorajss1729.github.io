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

<!-- Include PyScript -->
<link rel="stylesheet" href="https://pyscript.net/latest/pyscript.css" />
<script defer src="https://pyscript.net/latest/pyscript.js"></script>

<!-- Main Content Style -->
<style>
.text-block {
    margin-left: 2%;
    margin-right: 2%;
    text-align: justify;
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

/* Subheading Styles */
h2, h3 {
    display: block;
    font-size: 1.3rem;
    font-weight: bold;
    text-align: left;
    margin-left: 2%;
    margin-right: 2%;
    margin-bottom: 1rem;
    text-indent: 0;
    border-bottom: 0.5px solid #f5f5f5;
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
    margin-bottom: 0.5rem;
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

<!-- Introduction Paragraph -->
<div class="text-block">
  <p>This page is a collection of detailed explorations where I unpack complex topics, break down methods, and present my analysis. Each section below contains interactive demos or explanations of key steps.</p>
</div>

<!-- Table of Contents -->
<div id="toc-container">
  <ul>
    <li><a href="#introduction">Introduction</a></li>
    <li><a href="#algorithm-outline">Algorithm Outline</a></li>
    <li><a href="#simulator">Interactive Simulator</a></li>
    <li><a href="#further-reading">Further Reading</a></li>
  </ul>
</div>

<!-- Introduction -->
<div id="introduction" class="text-block">
  <h2>Introduction</h2>
  <p>Clifford operators are a fundamental class of unitary operators in quantum computing, used for stabilizer states and error correction. Efficiently sampling these operators at random is critical for benchmarking and noise estimation. Here we explore the algorithm presented by Ewout van den Berg, then run an interactive browser-based simulation.</p>
</div>

<!-- Outline -->
<div id="algorithm-outline" class="text-block">
  <h2>Algorithm Outline</h2>
  <p>The algorithm uses the tableau representation of Pauli operators and performs hierarchical random sampling and sweeping steps to generate a uniform random Clifford circuit. Details include:</p>
  <ul>
    <li>Sampling random anticommuting Pauli pairs.</li>
    <li>Normalizing via Hadamard, Phase, and CNOT gates.</li>
    <li>Constructing the final Clifford as the inverse of the composed sweeps.</li>
  </ul>
</div>

<!-- Interactive Simulator -->
<div id="simulator" class="text-block">
  <h2>Interactive Simulator</h2>
  <p>Select the number of qubits and click "Generate" to run the algorithm in your browser. No server or installation required.</p>
  <label for="n_qubits">Number of qubits:</label>
  <input type="number" id="n_qubits" min="1" max="5" value="3" />
  <button id="gen_btn">Generate Clifford</button>
  <div id="output"></div>

  <py-script output="output" pyscript="">
import numpy as np
from qiskit import QuantumCircuit
import matplotlib.pyplot as plt
from js import document

def anticom_rows_gen(k):
    while True:
        r1 = np.random.randint(0,2,size=2*k+1)
        r2 = np.random.randint(0,2,size=2*k+1)
        ip = (r1[:2*k:2]*r2[1:2*k:2] + r1[1:2*k:2]*r2[:2*k:2]).sum() % 2
        if ip == 1:
            return r1,r2

# (Include your final sweep functions here in Python)
def random_clifford(k):
    # placeholder: return a trivial Clifford for demo
    return [("h",0),("cx",0,1)]


def build_qc(k, gates):
    qc = QuantumCircuit(k)
    for g in gates:
        t,*ps = g
        if t == "h": qc.h(ps[0])
        elif t == "sd": qc.sdg(ps[0])
        elif t == "cx": qc.cx(ps[0],ps[1])
    return qc

# Wire button

def on_click(evt):
    k = int(document.getElementById("n_qubits").value)
    dg = random_clifford(k)
    qc = build_qc(k, dg)
    fig = qc.draw("mpl")
    display(fig)

document.getElementById("gen_btn").element.onclick = on_click
  </py-script>
</div>

<!-- Further Reading -->
<div id="further-reading" class="text-block">
  <h2>Further Reading</h2>
  <p>Read the original paper and related works on quantum benchmarking and the Clifford group:</p>
  <ul>
    <li><a href="https://doi.org/10.1109/QCE52317.2021.00021" target="_blank">van den Berg, “A simple method for sampling random Clifford operators”</a></li>
    <li><a href="https://arxiv.org/abs/2003.09412" target="_blank">Bravyi & Maslov, “Hadamard-free circuits expose the structure of the Clifford group”</a></li>
  </ul>
</div>

