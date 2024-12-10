---
title: ""
permalink: /mathematics/
layout: archive
collection: mathematics
entries_layout: grid
classes: wide
---


<style>
.text-block {
    text-align: justify;
    text-indent: 2em;
    margin-right: auto;
    max-width: 8.27in; /* Constrain to A4 width */
}
.toc {
    padding: 0;
    border: none;
    max-width: 100%;
    margin: 20px 0;
    font-family: inherit;
    font-weight: normal;
}
.toc h2 {
    font-size: 1.5em;
    color: #333;
    text-align: left;
    text-transform: none;
    font-family: inherit;
    font-weight: normal;
}
.toc ul {
    list-style: none;
    padding: 0;
}
.toc li {
    margin: 10px 0;
    font-weight: normal;
    text-transform: none;
}
.toc a {
    text-decoration: none;
    font-size: 1.1em;
    font-family: inherit;
    font-weight: normal;
    color: var(--link-color); /* Matches website link color */
}
.toc a:hover {
    text-decoration: underline;
}
.toc .subsection {
    margin-left: 20px;
    font-size: 0.95em;
    counter-reset: subsection; /* Reset subsection counter */
}
.toc .subsection li {
    counter-increment: subsection; /* Increment subsection */
}
.toc .subsection li::before {
    content: counters(chapter, ".") "." counter(subsection) " "; /* Format as 1.1, 1.2 */
    color: #555;
    margin-right: 5px;
}
.toc .chapter-number {
    counter-increment: chapter; /* Increment chapter number */
}
.toc .chapter-number::before {
    content: counter(chapter) ". "; /* Add chapter number */
}
.toc .link-numbers {
    margin-left: 5px;
}
.toc .link-numbers a {
    text-decoration: none;
    font-size: 0.95em;
    font-family: inherit;
    color: var(--link-color); /* Matches website link color */
}
.toc .link-numbers a:hover {
    text-decoration: underline;
}
</style>

## Linear Algebra
<a name="linear-algebra"></a>
<div class="text-block">
 <p>Linear algebra has been a crucial part of my learning journey, especially as I ventured into quantum computing. I  started with <a href="https://archive.org/details/gilbert-strang-introduction-to-linear-algebra-fifth-edition/page/504/mode/2up">Gilbert Strang's Introduction to Linear Algebra</a> to build a strong foundation, but I often found myself exploring much deeper concepts and proofs beyond what the book covered. Throughout this process, <a href="https://math.stackexchange.com/users/223599/sooraj-soman">Mathematics Stack Exchange</a> became an invaluable resource for clarifying doubts, solving challenging problems, and learning through engaging discussions with the community.</p>
 <p>These notes are an attempt to organize and share what I’ve learned over the years. They reflect not only the material from Strang's book but also the extended explorations and insights I’ve gained while tackling questions and problems. Having enrolled in Math 6108 Applied Matrix Theory at Missouri S & T, my notes go well beyond the scope of a 6000-level advanced graduate course.</p>
</div>

<div class="toc">
    <h2>Table of Contents</h2>
    
<li>
    <a href="#viewer" onclick="document.getElementById('pdf-viewer').src = 'https://mozilla.github.io/pdf.js/web/viewer.html?file=https://drive.google.com/uc?id=1f3K9YLWhz6vVbn6-ZbezSaqHsPCz_uSk&page=75';">
        Applications in Linear Transformations
    </a>
</li>

    <ul>
        <li class="chapter-number">
            <a href="https://drive.google.com/file/d/<file_id>/preview#page=12" target="_blank">Matrices - Introduction</a>
            <ul class="subsection">
                <li>
                    Matrix Addition
                    <span class="link-numbers">
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=13" target="_blank">1</a>]
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=20" target="_blank">2</a>]
                    </span>
                </li>
                <li>
                    Matrix Multiplication
                    <span class="link-numbers">
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=15" target="_blank">1</a>]
                    </span>
                </li>
                <li>
                    Transpose of a Matrix
                    <span class="link-numbers">
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=17" target="_blank">1</a>]
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=25" target="_blank">2</a>]
                    </span>
                </li>
            </ul>
        </li>
        <li class="chapter-number">
            <a href="https://drive.google.com/file/d/<file_id>/preview#page=30" target="_blank">Determinants</a>
            <ul class="subsection">
                <li>
                    Properties of Determinants
                    <span class="link-numbers">
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=32" target="_blank">1</a>]
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=37" target="_blank">2</a>]
                    </span>
                </li>
                <li>
                    Cofactor Expansion
                    <span class="link-numbers">
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=40" target="_blank">1</a>]
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=45" target="_blank">2</a>]
                    </span>
                </li>
                <li>
                    Applications of Determinants
                    <span class="link-numbers">
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=48" target="_blank">1</a>]
                    </span>
                </li>
            </ul>
        </li>
        <li class="chapter-number">
            <a href="https://drive.google.com/file/d/<file_id>/preview#page=60" target="_blank">Eigenvalues and Eigenvectors</a>
            <ul class="subsection">
                <li>
                    Finding Eigenvalues
                    <span class="link-numbers">
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=62" target="_blank">1</a>]
                    </span>
                </li>
                <li>
                    Finding Eigenvectors
                    <span class="link-numbers">
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=67" target="_blank">1</a>]
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=70" target="_blank">2</a>]
                    </span>
                </li>
                <li>
                    Applications in Linear Transformations
                    <span class="link-numbers">
                        [<a href="https://drive.google.com/file/d/<file_id>/preview#page=75" target="_blank">1</a>]
                    </span>
                </li>
            </ul>
        </li>
    </ul>
</div>


<iframe
    src="https://soorajss1729.github.io/pdfjs/viewer.html?file=la17.pdf"
    width="100%"
    height="800px"
    style="border: none;">
</iframe>


<iframe
  src="https://drive.google.com/file/d/1cGLAdAGYLAjP9qri1R7-aXTJQUHkN7-j/preview"
  style="width: 100%; height: 100vh; border: none;">
</iframe>


<iframe
    src="https://soorajss1729.github.io/pdfjs/la17.pdf"
    width="100%"
    height="800px"
    style="border: none;">
</iframe>

<iframe
  src="https://drive.google.com/uc?export=download&id=1cGLAdAGYLAjP9qri1R7-aXTJQUHkN7-j"
  style="width: 100%; height: 100vh; border: none;">
</iframe>


<!-- https://thomasgultzow.com/ -->

