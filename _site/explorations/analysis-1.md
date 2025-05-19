<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>A Simple Method for Sampling Random Clifford Operators</title>
  <script defer src="assets/js/pyscript.js"></script>
  <style>
    body { font-family: Arial, sans-serif; margin: 2%; }
    h1 { font-size: 1.8rem; margin-bottom: 1rem; }
    #output { 
        margin-top: 1rem; 
        padding: 1rem; 
        background-color: #f4f4f9; 
        border: 1px solid #ddd; 
        white-space: pre; 
        font-family: monospace; 
    }
    button { 
        padding: 0.5rem 1rem; 
        background-color: #2f7f93; 
        color: #fff; 
        border: none; 
        border-radius: 5px; 
        cursor: pointer; 
        transition: background 0.3s; 
    }
    button:hover { background-color: #1a5e73; }
  </style>
</head>
<body>
  <h1>A Simple Method for Sampling Random Clifford Operators</h1>
  <p>You can interactively explore and simulate random Clifford operators directly below:</p>

  <h2>Interactive Clifford Operator Simulator</h2>
  <label for="n_qubits">Number of qubits:</label>
  <input type="number" id="n_qubits" min="1" max="5" value="3" />
  <button id="gen_btn">Generate Clifford</button>
  <div id="output"></div>

  <py-script>
import numpy as np
from qiskit import QuantumCircuit
from pyodide.ffi import create_proxy
from js import document

# Function to generate random Clifford
def random_clifford(k):
    gates = []
    for i in range(k):
        gates.append(("h", i))
        if i < k - 1:
            gates.append(("cx", i, i + 1))
    return gates

# Function to build and display the circuit
def build_qc(k, gates):
    qc = QuantumCircuit(k)
    for g in gates:
        t, *ps = g
        if t == "h":
            qc.h(ps[0])
        elif t == "sd":
            qc.sdg(ps[0])
        elif t == "cx":
            qc.cx(ps[0], ps[1])
    return qc

# Function to handle button click
def generate_clifford(event):
    k = int(document.getElementById("n_qubits").value)
    gates = random_clifford(k)
    qc = build_qc(k, gates)
    # Display the circuit as text (ASCII)
    circuit_str = qc.draw(output="text").__str__()
    document.getElementById("output").innerHTML = f"<pre>{circuit_str}</pre>"

# Attach event listener
proxy = create_proxy(generate_clifford)
document.getElementById("gen_btn").addEventListener("click", proxy)
  </py-script>
</body>
</html>

