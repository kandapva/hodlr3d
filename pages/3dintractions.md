---
layout: page
title: 3D Interactions
permalink: /3dintractions/
---

# Interactions in 3D

Welcome to the {{ site.title }} Documentation pages! Here you can quickly view various 3D interactions that help you in understanding 3D.


<div class="container">
<div class="section-title">
<h2>Hierarchical Sub-division of the domain in 3D</h2>
</div>
<p><b>Consider a box (<i>a cube</i>) in 3D which corresponds to root node in the hierarchical tree (Level 0)</b></p>
<object data="level0.html" width="500" height="500"></object> <br><br><br><br><br><br>

<p><b>Subdivision of the domain hierarchically results in 8 smaller cubes (each corresponding to 8 children nodes of the root node in the Hierarchical tree).  <i>(Level 1 Subdivision)</i></b></p>
<object data="level1.html" width="500" height="500"></object> <br><br><br><br><br><br>
<p><b>Further subdivision (Level 2) results in 64 cubes as shown below:</b></p>
<object data="lvl32.html" width="500" height="500"></object>
</div>

<div class="container">
<div class="section-title">
<h2>Different types of interactions in 3D</h2>
</div>
<p>Based on how the boxes share boundary, they can be classified as following types:</p> 
 <ul>
  <li>Vertex sharing intractions</li>
  <li>Edge sharing intractions</li>
  <li>Face sharing intractions</li>
  <li>Far field intractions</li>
</ul> 
<h3>Vertex sharing intractions</h3>
<p><b>Consider a box (<i>at level 2</i>) in 3D then it the boxes that share atmost an vertex are named<i> VERTEX sharing boxes</i></b></p>
<object data="neighbours_vertex_nodots.html" width="500" height="500"></object> <br><br><br><br><br><br>
<h3>Edge sharing intractions</h3>
<p><b>For a box highlighted in black, the edge sharing boxes are colored in green.</b></p>
<object data="neighbours_edge_nodots.html" width="500" height="500"></object> <br><br><br><br><br><br>
<h3>Face sharing intractions</h3>
<p><b>Further the face sharing boxes are shown below:</b></p>
<object data="neighbours_face_nodots.html" width="500" height="500"></object>
<h3>Far field intractions</h3>
<p><b>The boxes that do not share a boundary is said to have far field intractions.</b></p>
</div>