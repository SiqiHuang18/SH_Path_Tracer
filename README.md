<meta http-equiv="content-type" content="text/html; charset=utf-8" />
<link rel="stylesheet" type="text/css" href="style.css" media="screen" />
<h1 align="middle">Path Tracer Write-up</h1>

  <h2 align="middle">Overview</h2>
   This is a cpu based path tracer that implements the core rendering loop from ray generation and intersection to global illumination. It has acceleration strategy like bounding volume hierachy and adaptive sampling and supports various materials, environment lighting and depth of field. Each core functionality is demonstrated in this writeup. This project builds upon the starter code of UC Berekeley CS184 Assignment 3.     
   
  <h2 align="middle">Part 1: Ray Generation and Intersection</h2>
  <p>Describe what you did in Part 1. etc...</p>
          <div align="center">
              <table style="width=100%">
                  <tr>
                      <td align="middle">
                      <img src="images/ray/CBsphere_n.png" width="480px" />
                      <figcaption align="middle">Results Caption: my bunny is the bounciest bunny</figcaption>
                  </tr>
              </table>
          </div>
