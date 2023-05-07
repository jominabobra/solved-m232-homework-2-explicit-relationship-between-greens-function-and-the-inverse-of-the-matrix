Download Link: https://assignmentchef.com/product/solved-m232-homework-2-explicit-relationship-between-greens-function-and-the-inverse-of-the-matrix
<br>
<ol>

 <li><em>This problem allows you to see the explicit relationship between Green’s function and the inverse of the matrix A in the finite difference method.</em>

  <ul>

   <li>Write out the 5 × 5 matrix <em>A </em>from (2.43) for the boundary value problem <em>u</em><sup>00</sup>(<em>x</em>) = <em>f</em>(<em>x</em>) with <em>u</em>(0) = <em>u</em>(1) = 0 for <em>h </em>= 0<em>.</em></li>

   <li>Analytically find the inverse matrix <em>A</em><sup>−1 </sup>explicitly for this problem.</li>

   <li>Use your result from (b) to determine the discrete approximation to the solution of theboundary value problem with <em>f</em>(<em>x</em>) = <em>x </em>on this grid. Plot this solution and the five Green’s functions whose sum gives this solution.</li>

  </ul></li>

 <li><em>This problem makes use of the </em>bvp 2.m <em>code to study an ill-posed boundary value problem.</em></li>

</ol>

Consider the following linear boundary value problem with Dirichlet boundary conditions:

<em>u</em><sup>00</sup>(<em>x</em>) + <em>u</em>(<em>x</em>) = 0  for <em>a &lt; x &lt; b u</em>(<em>a</em>) = <em>α,     u</em>(<em>b</em>) = <em>β.</em>

Note that this equation arises from a linearized pendulum, for example.

<ul>

 <li>Modify the m-file bvp 2.m to solve this problem. Test your modified routine on the problem with

  <ul>

   <li>= 0<em>, b </em>= 1<em>,     α </em>= 2<em>,     β </em>= 3<em>.</em></li>

  </ul></li>

</ul>

Determine the exact solution for comparison.

<ul>

 <li>Let <em>a </em>= 0 and <em>b </em>= <em>π</em>. For what values of <em>α </em>and <em>β </em>does this boundary value problem have solutions? Sketch a family of solutions in a case where there are infinitely many solutions.</li>

 <li>Solve the problem with

  <ul>

   <li>= 0<em>, b </em>= <em>π,     α </em>= 1<em>,     β </em>= −1<em>.</em></li>

  </ul></li>

</ul>

using your modified bvp 2.m. Which solution to the boundary value problem does this appear to converge to as <em>h </em>→ 0? Change the boundary value at <em>b </em>= <em>π </em>to <em>β </em>= 1. Now how does the numerical solution behave as <em>h </em>→ 0?

<ul>

 <li>You might expect the linear system in part (c) to be singular since the boundary valueproblem is not well posed. It is not because of discretization error. Compute the eigenvalues of the matrix <em>A </em>for this problem and show that an eigenvalue approaches 0 as <em>h </em>→ 0. Also show that k<em>A</em><sup>−1</sup>k<sub>2 </sub>blows up as <em>h </em>→ 0 so that the discretization is unstable.</li>

</ul>


