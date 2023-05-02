Download Link: https://assignmentchef.com/product/solved-computer-vision-final-project
<br>
<h1></h1>

This assignment combines all the previous steps that students have implemented and add more steps to finalize the project. This is the last guideline regarding your project. <em>Model Castle </em>images are used for the project which have been provided in the Brightspace. We provide the feature point descriptors on Brightspace for everyone.

<h2>1          Components of the Project and Grading</h2>

<ol>

 <li><strong>(.5 + 1</strong><sup>∗ </sup><strong>pt) </strong>Use relevant tools (e.g. <em>vl feat</em>: http://www.vlfeat.org) to find interest points and correspondence (matches) between consecutive images.</li>

</ol>

<strong>Note: </strong>You can get 1 bonus point if you submit a workable implementation of your own for Harris corner detection and feature matching. (Lab assignment 2).

<ol start="2">

 <li><strong>(1.5 pt) </strong>Apply normalized 8-point RANSAC algorithm to find best matches. (Lab assignment 3+5)</li>

 <li><strong>(2.5 pt) Chaining: </strong>Create point-view matrix to represent point correspondences for different camera views (Lab assignment 6).</li>

 <li><strong>(3.5 pt) Stiching:</strong>

  <ul>

   <li><strong>(1 pt) </strong>Take blocks of the point-view matrix that are composed of three and four consecutive images.</li>

  </ul></li>

</ol>

1

<ul>

 <li><strong>(1.5 pt) </strong>Estimate 3D coordinates of each block using TomasiKanade factorization (Lab assignment 4).</li>

 <li><strong>(1 pt) </strong>By an iterative manner, stitch each 3D point set to the main view using the point correspondences i.e., finding optimal transformation between shared points in your 3D point clouds. Transformation between different sets can be found using Procrustes analysis. The MATLAB procrustes function can be used in the project.</li>

</ul>

<ol start="5">

 <li><strong>(1 pt) </strong>Eliminate affine ambiguity (consult your lecture slides on affine structure from motion).</li>

 <li><strong>(1 pt) 3D Model Plotting: </strong>When you have the 3D point cloud of the castle, use the built-in surf function for the 3D surface plot. Then include RGB (texture) colour of the related points on surf visualization (interpolate colour values for the filled areas on the surface using the known points). Students are supposed to implement this in a clever way (by using built-in Matlab functions).</li>

</ol>

The final report for the project (in pdf format) together with the code must be submitted via Brightspace.

The report needs to be within 5 pages (or less) and explain and motivates your choices and results clearly.

<ul>

 <li>Use in the report as many as visualizations/intermediate results as possible, obtained from your own code.</li>

 <li>Explain as clearly as possible every step you have taken in solving every task. Please have a look at the writing guidelines here:</li>

</ul>

http://jvgemert.github.io/links.html.

The code must have one main script that calls different functions to perform the 3D reconstruction and should use relative paths and be ready to run. Each function implements one of the modules that is described in this guideline.

2