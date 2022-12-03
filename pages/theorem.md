---
layout: page
title: Theorem in 3D
permalink: /theorem/
---

# Rank of Off-diagonal blocks of Laplacian Kernel in 3D
We consider a cube domain in 3D, then a hierarchical subdivision performed using a oct tree of level L. Then, for any level $$l$$ where $$0<l\leq L$$, we have four different types of interactions, viz., 
  * Well-separated interactions
  * Vertex-sharing interactions
  * Edge-sharing interactions
  * Face-sharing interactions
   
<blockquote style="border: 2px solid #666; padding: 10px; background-color: #ccc;">
<h3>Theorem</h3>
Let \(\{q_j\}_{j=1}^N\) be \(N\) uniformly located charges at \(\{z_j\}_{j=1}^N\) inside a box \(B_1\) of side length \(l\). Let \(Q = \sum_{i=1}^N |q_i|\). The potential due to these \(N\) charges at \(M\) locations \(\{w_i\}_{i=1}^M\), with \(M \geq N\), inside another box \(B_2\) is given by \(\phi_i = \sum_{j=1}^N \frac{q_j}{|w_j-z_j|}\). 
In matrix-vector parlance, we have
		                            $$\vec{\phi}=A\vec{q}$$
where \(\vec{q} \in \mathbb{R}^{N \times 1}\), \(\vec{\phi} \in \mathbb{R}^{M \times 1}\) and \(A \in \mathbb{R}^{M \times N}\) with \(A_{ij} = \frac{1}{|w_j-z_j|}\). Then we claim that for a hierarchical subdivision using an oct tree, given \(\epsilon > 0\), there exists a matrix \(\tilde{A} \in \mathbb{R}^{M \times N}\) with rank of \(\tilde{A}\) at most \(\tau\), where \(\tau \in \mathcal{O} (R(N)\log^2_8(\frac{S(N)Q}{l\epsilon}))\) that approximates \(\phi_i\) such that \(|\phi_i-\{\tilde{A}q\}_i| < \epsilon\), where
<ul>
  <li>\(R(N) = 1,S(N)=1\) if the boxes \(B_1\) and \(B_2\) are at least one box away, i.e., \(\text{dist}(B_1,B_2) \geq l\).</li>
   <li> \(R(N) = \log(N),S(N)=\sqrt[3]{N}\) if the boxes \(B_1\) and \(B_2\) are vertex sharing neighbors.</li>
   <li>\(R(N) = \sqrt[3]{N}, S(N)=\sqrt[3]{N^2}\) if the boxes \(B_1\) and \(B_2\) are edge sharing neighbors.</li>
    <li>\(R(N) = \sqrt[3]{N^2}, S(N)=N\) if the boxes \(B_1\) and \(B_2\) are face sharing neighbors.</li>
</ul> 
</blockquote>

In this page, we would like to show in an interactive way of how the cube considered is subdivided. Following that the construction of a sphere that ensures for $$\epsilon$$ we have a rank $$\tau$$ approximation. For detailed proof and steps, please refer the [article](https://kandapva.github.io/hodlr3d/).
## Case 1 : Far field intractions
<div class="container">
<div class="box">
  <iframe src="Far_level.html" frameborder="0" scrolling="no" height="300" width="300" align="left"> </iframe>
</div>
<div class="box">
  <iframe src="Far_level_sphere.html" frameborder="0" scrolling="no" height="300" width="300" align="left"></iframe>
</div>
</div>

<hr style="clear:both;">

## Case 2 : Vertex sharing intractions

<div class="container">
<div class="box">
<iframe src="Vertex_level_0.html" frameborder="0" scrolling="no" height="300" width="300" align="left"></iframe>
</div>
<div class="box">
<iframe src="Vertex_level_1.html" frameborder="0" scrolling="no" height="300" width="300" align="left"></iframe>
</div>
<div class="box">
<iframe src="Vertex_level_sphere.html" frameborder="0" scrolling="no" height="300" width="300" align="left"></iframe>
</div>
</div>

<hr style="clear:both;">

## Case 3 : Edge sharing intractions

<div class="container">
<div class="box">
<iframe src="Edge_level_0.html" frameborder="0" scrolling="no" height="300" width="300" align="left"></iframe>
</div>
<div class="box">
<iframe src="Edge_level_1.html" frameborder="0" scrolling="no" height="300" width="300" align="left"></iframe>
</div>
<div class="box">
<iframe src="Edge_level_sphere.html" frameborder="0" scrolling="no" height="300" width="300" align="left"></iframe>
</div>
</div>

<hr style="clear:both;">

## Case 4 : Face sharing intractions

<div class="container">
<div class="box">
<iframe src="Face_level_0.html" frameborder="0" scrolling="no" height="300" width="300" align="left" title="Face sharing intractions"></iframe>
</div>
<div class="box">
<iframe src="Face_level_1.html" frameborder="0" scrolling="no" height="300" width="300" align="left"></iframe>
</div>
<div class="box">
<iframe src="Face_level_sphere.html" frameborder="0" scrolling="no" height="300" width="300" align="left"></iframe>
</div>
</div>

<hr style="clear:both;">



