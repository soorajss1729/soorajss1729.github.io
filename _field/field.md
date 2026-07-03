---
title: "Field Theory"
permalink: /field/
layout: default
classes: wide
footer_fixed: false
---

<div class="learning-topnav">
  <a href="/learning/">‹ Back</a>
  <a href="/linalg/">Linear Algebra</a>  
  <a href="/qc#">Quantum Computing</a>  
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
  <h1>Field Theory</h1>


<div class="text-block">
  <p>Field theory has been one of the main areas where I tried to understand algebra in a deeper and more connected way. I worked through the material mainly using Isaacs’ <a href="https://www.ams.org/books/gsm/100" style="text-decoration: none;"><i>Algebra: A Graduate Course</i></a>, covering polynomial rings, field extensions, splitting fields, separability, normality, finite fields, and Galois theory.
</p> 
 <p>These notes are my attempt to organize the subject carefully and make the logical flow clear. I tried to go through each concept in depth, filling in proof details, adding relevant examples, and expanding arguments that are often presented too briefly.</p>
</div>

<div class="content-container">
  <!-- Table of Contents -->
  <div id="toc-container">


  <details>
    <summary>Chapter 12: Rings, Ideal, and Modules</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=1')">Sym($\Omega$), End(A)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=3')">Ring</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=5')">A abelian $\implies$ End(A) is a ring</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=7')">Subring</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=10')">Ring Homomorphism</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=16')">Ideals, e$\in$I$\implies$ I is a subring</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=17')">$1_R\in I\implies I=R$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=19')">Principal Ideal, (a)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=22')">Left/Right Annihilator of $X\subseteq R$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=23')">Factor Ring, $R/I$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=25')">$\pi:R\to R/I, \pi(r)=r+I$ is a ring homomorphism with $ker(\pi)=I$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=26')">Unit, $U(R)$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=30')">Division Ring</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=32')">Field</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=33')">Subfield Test</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=34')">If R commutative then: M max ideal of R$\iff$ R/M field</a></li>      
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf#page=39')">R Module</a></li>
    </ul>
  </details>
  <details>
    <summary>Chapter 16: Polynomial Rings, PIDs, and UFDs</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=1')">Ring, Subring</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=5')">Integral Domain</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=7')">Principal Ideal Domain (PID)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=8')">$R[X]$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=11')">$R[X]$ is a ring, Unitary subring</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=15')">$R$ integral domain $\implies $ $R[X]$ is integral domain</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=16')">Division Algorithm</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=18')">$F$ is field $\implies$ $F[X]$ is a PID</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=20')">Irreducible element of $R$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=22')">Wishes of a Domain</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=23')">Divisibility in a Domain</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=28')">Unique Factorization Domain (UFD)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=29')">Prime Ideal</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=31')">Prime Element</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=33')">Irreducible, Prime, and Maximal Ideals in a PID</a></li>      
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=34')">R is a PID $\implies$ R is UFD</a></li>     
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=35')">If $R$ is UFD, then $a\in R$ irreducible $\iff$ $a$ is prime element</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=37')">Coprime/Relatively elements</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=39')">$R$ is PID $\implies$ $R$ is UFD</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=40')">$R$ is UFD $\implies $ $R[X]$ is UFD</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=41')">Field of Fraction, Frac($R$)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=42')">Eisenstein criterion</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch16.pdf#page=44')">Frac(Z[i])=Q(i)</a></li>
    </ul>
  </details>
  <details>
    <summary>Chapter 17: Extension Fields</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=1')">Extension Fields</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=1')">Algebraic, Transcedental/F</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=4')">F(t)=Frac(F[t]) is a field</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=8')">Degree of field extension, $|E:F|=\dim_F(E)$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=9')">If $R$ is a domain, $F\subseteq R$ then $|R:F|<\infty\implies R$ is a field</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=11')">Minimal Polynomial of an Algebraic Element over F</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=15')">$F[ \alpha]\cong F[X]/(m_{F,\alpha})$ and $I=(m_{F,\alpha})$ is the max ideal</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=20')">$|F[\alpha]:F|=\deg(m_{F,\alpha})=\dim_F(F[\alpha])$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=22')">$\alpha$ algebraic/F $\iff$ $|F[\alpha]:F|<\infty\iff F[\alpha]=F(\alpha)$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=24')">$\alpha$ transcedental/F $\implies F[\alpha]\cong F[X]$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=25')">$F \subseteq E$ with $|E:F|<\infty\implies E$ algebraic extension</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=27')">$F \subseteq E \subseteq L\implies |L:F|=|L:E||E:F|$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=29')">$A=\{\alpha\in E|\alpha\text{ is algebraic/F}\}\implies F\subseteq A\subseteq E$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=31')">$F[\alpha,\beta]=(F[\alpha])[\beta]=(F[\beta])[\alpha]$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=33')">$F\subseteq E\subseteq L$, E algebraic/F, L algebraic/E $\implies$ L algebraic/F</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=35')">$f\in F[X]\implies \exists E\supseteq F, \alpha\in E$ st $f(\alpha)=0$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=42')">f splits/F</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=44')">Algebraically closed</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=45')">Algebraic closure</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=46')">Splitting field of f over F</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=47')">E is the sf of $f\in F[X]\implies |E:F|<\infty$</a></li>      
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=48')">Simple extension $E=F(\alpha)$, primitive element $\alpha$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch17.pdf#page=49')">Finite Subgroups of $F^×$ are Cyclic</a></li>
    </ul>
  </details>
  <details>
    <summary>Chapter 18: Galois Theory</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=2')">Galois group of the extension</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=4')">$Fix\Big(Gal(E/F)\Big)\supseteq F$ $\&$ $Gal\Big(E/Fix(G)\Big)\supseteq G$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=8')">$H_1\subseteq H_2\implies Fix(H_1)\supseteq Fix(H_2)$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=11')">Extension of Field Isomorphisms to Simple Extensions</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=18')">Uniqueness of Splitting Fields</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=22')">Gal(E/F) permutes the roots of f$\in$F[X] in E</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=27')">Fix(Gal(E/F))=F $\implies$ E galois/F</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=28')">Normal Extension</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=29')">E Normal/F$\iff$ E is sf/F for some g$\in$F[X]</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=31')">E algebraic closure of F$\implies$E is normal/F</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=31')">$|E:F|=2\implies$E is normal/F</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=36')">Repeated root of f</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=36')">Separable Extension</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=37')">f$\in$F[X] separable/F if each irreducible factor of f in F[X] has distinct roots in a sf</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=38')">F$\subseteq$K$\subseteq$E, $\alpha\in$ E then $\alpha$ normal(separable)/F$\implies\alpha$ normal(separable)/K</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=39')">Char(E)=Char(F)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=40')">Char(F)=0 or F finite$\implies$ Every alg extension is separable</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=42')">E galois extension of F$\iff$E is sf/F for some separable poly/F </a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=49')">F$\subseteq$K$\subseteq$E, E galois/F$\implies$E galois/K</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=50')">Finite degree separable ext.$\implies$E=F[$\alpha$]</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=53')">E galois/F$\iff |Gal(E/F)|=|E:F|$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=55')">G finite$\implies$ E galois/F $\&$ Gal(E/Fix(G))=G</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=58')">Fundamental Theorem of Galois Theorem (FTGT)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=76')">Algebraic Closedness Criterion: Odd-Degree Polynomials and Square Roots</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=82')">Compositum of E and L, $\langle L,E\rangle$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch18.pdf#page=83')">Natural Irrationalities</a></li>
    </ul>
  </details>
  <details>
    <summary>Chapter 19: Separability</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=1')">$\alpha$ repeated root $\iff$ $f(\alpha)=0$ $\&$ $f'(\alpha)=0$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=2')">Derivation of R</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=3')">Der(R) abelian grp under $+$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=5')">Lie Ring</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=6')">F-algebra</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=7')">F-derivation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=9')">$\delta(uv)=u\delta(v)+\delta(u)v\forall u,v\in\mathcal{B}\implies\delta$ is a derivation</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=13')">f$\in$F[X] irreducible then f has distinct roots$\iff$f'$\neq 0$</a></li>      
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=17')">Inseparable Irreducible Polynomials have the Form $g(X^p)$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=20')">$(a+b)^p=a^p+b^p$, $(ab)^p=a^pb^p\;\forall a,b\in$F</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=21')">Finite fields are perfect ($F^p=F$)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=23')">f$\in$F[X] inseparable$\implies$char(F)=p $\&$ F not perfect$\implies$F infinite</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=24')">Char(F)=0 or F perfect of Char(F)=p$\implies$all f$\in$F[X] are separable</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=25')">Irreducible Polynomials in Characteristic \(p\): \(f(X)=g(X^{p^n})\) with \(g\) Separable</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch19.pdf#page=28')">Purely Inseparable Extensions</a></li>
    </ul>
  </details>
  <details>
    <summary>Chapter 20: Cyclotomy and Geometric Constructions</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=1')">$n^{th}$ root of unity</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=2')">$n^{th}$ root of unity in F form a cyclic subgroup of F$^×$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=4')">Primitive $n^{th}$ root of unity</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=8')">$\exists$ Primitive $n^{th}$ root of unity in $E\supseteq$ F $\iff$Char(F) $\nmid$ n</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=9')">F has primitive $n^{th}$ root$\iff$ $x^n-1$ splits/F$\&$Char(F)$\nmid$n</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=10')">Primitive nth Roots and Splitting Field of $x^n-1$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=12')">$n^{th}$ cyclotomic polynomial, $\Phi_n(X)$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=15')">$n^{th}$ cyclotomic field, $Q_n=Q[\varepsilon_n]$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=17')">Set of all units in $Z/nZ$ form a multiplicative group</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=18')">$Gal(Q_n/Q)\cong (Z/nZ)^×$ is abelian</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=20')">G abelian, o(x)=n, o(y)=m, gcd(m,n)=1$\implies$o(xy)=mn</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=21')">gcd(m,n)=1$\implies Q_n\cap Q_m=Q$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=24')">Kummer Theorem</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=29')">Crossed Homomorphism</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=31')">Dedekind's Lemma</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=33')">Constructible Numbers</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=36')">$K\subseteq \mathbb{C}$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=38')">$\alpha\in K\implies\sqrt{\alpha}\in K$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=39')">Constructible Elements and Towers of Quadratic Extensions</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=42')">$\alpha\in K\implies \alpha\text{algebraic/Q}\&|Q(\alpha):Q|=2^k$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=44')">$\alpha\in K\iff \alpha\text{algebraic/Q}\&|Gal(E/Q)|=|E:Q|=2^k$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=46')">Fermat prime</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch20.pdf#page=47')">regular n-gon is constructible $\iff \varepsilon_n\in$K</a></li>
   </ul>
  </details>
  <details>
    <summary>Chapter 21: Finite Fields</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch21.pdf#page=1')">$K=\cap$(intersection of subfields of F)</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch21.pdf#page=5')">F finite field$\&$|E:F|=n<$\infty\implies$E is finite$\&|E|=|F|^n$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch21.pdf#page=6')">F finite field$\implies$Char(F)=p$\&$|F|=p^n where $|F:K|=n$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch21.pdf#page=7')">$|F|^n\&F\supseteq K$ be prime subfield$\implies$every $\alpha\in F$ is a root of f</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch21.pdf#page=8')">$|E|=|F|<\infty\implies E\cong F$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch21.pdf#page=11')">$GF(p^n)=\mathbb{F}_{p^n}$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch21.pdf#page=12')">$E=GF(p^n)\implies E$ galois/K$\&$Gal(E/K)=<$\sigma$> where $|Gal(E/K)|=n$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch21.pdf#page=16')">$|E|=p^n$ then $\exists$ ! $F\subseteq E$ with $|F|=p^m$ iff $m|n$</a></li>
   </ul>
  </details>
  <details>
    <summary>Chapter 22: Roots, Radicals, and Real Numbers</summary>
    <ul>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch22.pdf#page=1')">Radical Extension</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch22.pdf#page=2')">Repeated Radical Extension</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch22.pdf#page=4')">Galois: f is solvable by radicals $\iff$Gal(E/F) is solvable</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch22.pdf#page=10')">Generic Polynomial is Not Solvable by Radicals for $n\geq5$</a></li>
      <li><a href="javascript:void(0)" onclick="loadPdfPage('https://soorajss1729.github.io/pdfjs/viewer.html?file=fieldch22.pdf#page=12')">Every finite division ring is a field</a></li>
   </ul>
  </details>

  </div>
  



  <!-- PDF Viewer -->
  <div class="pdf-viewer">
    <iframe src="https://soorajss1729.github.io/pdfjs/viewer.html?file=ring.pdf" width="100%" height="1000px" style="border: none;"></iframe>
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


