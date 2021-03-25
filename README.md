<meta http-equiv="content-type" content="text/html; charset=utf-8" />
<link rel="stylesheet" type="text/css" href="style.css" media="screen" />
<h1 align="middle">Path Tracer Write-up</h1>

  <h2 align="middle">Overview</h2>
   This is a cpu based path tracer that implements the core rendering loop from ray generation and intersection to global illumination. It has acceleration strategy like bounding volume hierachy and adaptive sampling and supports various materials, environment lighting and depth of field. Each core functionality is demonstrated in this writeup. This project builds upon the starter code of UC Berekeley CS184 Assignment 3.     
   
  <h2 align="middle">Part 1: Ray Generation and Scene Intersection</h2>
    To compute the color information for each pixel we need to trace many rays to the scene and retrieve the information of the object surface that they intersects. For each pixel, we take random sample of position within the unit square, transform the sample point to camera space and parametrize a ray with this point and the origin. Then the ray in camera spacee is transformed to world space so that we can perform intersections.  
  <div class="row">
    <img src="images/ray/CBsphere_n.png" width="300px" />
    <img src="images/ray/CBgem_n.png" width="300px" />
  </div>
