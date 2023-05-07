Download Link: https://assignmentchef.com/product/solved-mae-3210-homework-6
<br>
<ol>

 <li>(a) Develop an algorithm which, for a given function of two variables <em>f</em>(<em>x,y</em>), interval bounds <em>a </em>and <em>b </em>with <em>a &lt; b</em>, and <em>c </em>and <em>d </em>with <em>c &lt; d</em>, and input integer <em>n </em>≥ 1, does the following:

  <ul>

   <li>If <em>n </em>is odd, it applies the multiple-application trapezoidal rule in</li>

  </ul></li>

</ol>

each dimension to approximate.

<ul>

 <li>If <em>n </em>is even, it applies the multiple-application Simpson’s 1/3 rule</li>

</ul>

in each dimension to approximate.

(b) Suppose the temperature T (<sup>o</sup>C) at a point (<em>x,y</em>) on a 16 m<sup>2 </sup>rectangular heated plate is given by

<em>T</em>(<em>x,y</em>) = <em>x</em><sup>2 </sup>− 3<em>y</em><sup>2 </sup>+ <em>xy </em>+ 72<em>,</em>

where −2 ≤ <em>x </em>≤ 2 and 0 ≤ <em>y </em>≤ 4 (here <em>x </em>and <em>y </em>are measured in meters about a reference point at (0<em>,</em>0)). Determine the average temperature of the plate:

<ul>

 <li>Analytically, to obtain a true value.</li>

 <li>Numerically, using the algorithm you developed in question 1(a) above, and plot the true percent relative error <em><sub>t </sub></em>as a function of <em>n </em>for 1 ≤ <em>n </em>≤ 5. Provide some interpretation of the results.</li>

</ul>

<ol start="2">

 <li>Write code for two separate algorithms to implement (a) Euler’s method and(b) the standard 4th order Runge-Kutta method, for solving a given first-order <strong>one-dimensional </strong> Design the code to solve the ODE over a prescribed interval with a prescribed step size, taking the initial condition at the left end point of the interval as an input variable.</li>

 <li>The drag force <em>F<sub>d </sub></em>(N) exerted on a falling object can be modeled as proportional to the square of the objects downward velocity <em>v </em>(m/s), with a constant of proportionality <em>c<sub>d </sub></em>(kg/m).

  <ul>

   <li>Assume that a falling object has mass <em>m </em>= 100 (kg) with a drag coefficient of <em>c<sub>d </sub></em>= 0<em>.</em>25 kg/m, and let <em>g </em>= 9<em>.</em>81 (m/s<sup>2</sup>) denote the constant downward acceleration due to gravity near the surface of the earth. Starting from Newton’s second law, explain the derivation of the following ODE for the downward velocity <em>v </em>= <em>v</em>(<em>t</em>) of the falling object:</li>

  </ul></li>

</ol>

<em>.                                      </em>(1)

<ul>

 <li>Suppose that this same object is dropped from an initial height of <em>y</em><sub>0 </sub>= 2 km. Determine when the object hits the ground by solving the ODE you derived in question 3(a) using

  <ul>

   <li>Euler’s method.</li>

   <li>the standard 4th order Runge-Kutta method.</li>

  </ul></li>

</ul>

<strong>HINT: </strong>Note that, with the velocity <em>v </em>oriented downward, the height <em>y </em>= <em>y</em>(<em>t</em>) satisfies . You are asked to find the final time <em>t<sub>f </sub></em>when the height <em>y </em>of the falling object reaches zero, i.e. when <em>y</em>(<em>t<sub>f</sub></em>) = 0. There are two ways to solve this problem.

<ol>

 <li>You can use your algorithm for solving one-dimensional ODEs (Eulerand Runge-Kutta 4) from question 2 to solve the ODE (1) to find <em>v </em>= <em>v</em>(<em>t</em>) (at discrete time points) with initial condition <em>v</em>(0) = 0. Then, you can use your one-dimensional ODE algorithms, again, to solve with initial condition <em>y</em>(0) = 2000 m, and try to identify when <em>y</em>(<em>t<sub>f</sub></em>) = 0.</li>

 <li>Alternatively, you can use your algorithm for solving two-dimensionalODEs (Euler and Runge-Kutta 4) from question 4 to solve the coupled</li>

</ol>

ODE system

<em>,</em>

with initial condition <em>y</em>(0) = 2000, <em>v</em>(0) = 0. Then, try to identify when <em>y</em>(<em>t<sub>f</sub></em>) = 0.

<ol start="4">

 <li>Write code for two separate algorithms to implement (a) Euler’s method and(b) the standard 4th order Runge-Kutta method, for solving a given first-order <strong>two-dimensional </strong>system of ODEs. Design the code to solve the system of ODEs over a prescribed interval with a prescribed step size.</li>

 <li>The motion of a damped mass spring is described by the following ODE</li>

</ol>

<em>,                                          </em>(2)

where <em>x </em>= displacement from equilibrium position (m), <em>t </em>= time (s), <em>m </em>= mass (kg), <em>k </em>= stiffness constant (N/m) and <em>c </em>= damping coefficient (N·s/m).

<ul>

 <li>Rewrite the 2nd order ODE (2) as a two-dimensional system of first orderODEs for the displacement <em>x </em>= <em>x</em>(<em>t</em>) and velocity <em>v </em>= <em>v</em>(<em>t</em>) of the mass attached to the spring.</li>

 <li>Assume that the mass is <em>m </em>= 10 kg, the stiffness <em>k </em>= 12 N/m, the damping coefficient is <em>c </em>= 3 N·s/m, the initial velocity of the mass is zero (<em>v</em>(0) = 0), and the initial displacement is <em>x </em>= 1 m (<em>x</em>(0) = 1). Solve for the displacement and velocity of the mass over the time period 0 ≤ <em>t </em>≤ 15, and plot your results for the displacement <em>x </em>= <em>x</em>(<em>t</em>),

  <ul>

   <li>using Euler’s method with step size <em>h </em>= 0<em>.</em>5, and then with step size <em>h </em>= 0<em>.</em></li>

   <li>using the standard 4th order Runge-Kutta method with step size<em>h </em>= 0<em>.</em>5, and then with step size <em>h </em>= 0<em>.</em></li>

  </ul></li>

 <li>Assume that the mass is <em>m </em>= 10 kg, the stiffness <em>k </em>= 12 N/m, the damping coefficient is <em>c </em>= 50 N·s/m, the initial velocity of the mass is zero (<em>v</em>(0) = 0), and the initial displacement is <em>x </em>= 1 m (<em>x</em>(0) = 1). Solve for the displacement and velocity of the mass over the time period 0 ≤ <em>t </em>≤ 15, and plot your results for the displacement <em>x </em>= <em>x</em>(<em>t</em>),

  <ul>

   <li>using Euler’s method with step size <em>h </em>= 0<em>.</em>5, and then with step size <em>h </em>= 0<em>.</em></li>

   <li>using the standard 4th order Runge-Kutta method with step size<em>h </em>= 0<em>.</em>5, and then with step size <em>h </em>= 0<em>.</em></li>

  </ul></li>

</ul>