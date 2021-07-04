# Introduction to Scientific Computing
## AMATH 301 Beginning Scientific Computing

AMATH 301 covers numerical methods and programming skills needed to solve physical, biological, and engineering problems. Content is transcribed from MATLAB (originally taught in the course) to Python for open source reference. Taken in Sp20 with Dr. Craig Gin.

Note: Starred topics (*) are not covered in Sp20 but covered in [previous years](https://www.youtube.com/channel/UCEirPnFv_2QbvzrM67SnKPA/videos).

### Root-Finding and Optimization
|Topic|Applications|Numerical Methods <br/> Python Skills|Jupyter <br/> Notebook|Online|
|-|-|-|:-:|:-:|
|Root finding algorithms|Solving function values|Bisection method <br/> Newton's method <br/> `scipy.optimize.root_scalar()`|[ipynb](root-finding-algorithms.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/root-finding-algorithms.html)|
|Unconstrained optimization|Finding max and min of convex functions|Golden section search <br/> Gradient descent <br/> `scipy.optimize.fminbound()` <br/> `scipy.optimize.fmin()`|[ipynb](unconstrained-optimization.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/unconstrained-optimization.html)|
|Constrained optimization*|Finding max and min of functions with constraints|Linear programming <br/> Genetic algorithm <br/> `scipy.optimize.linprog()` <br/> `scipy.optimize.differential_evolution()`|[ipynb](constrained-optimization.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/constrained-optimization.html)|
|Curve fitting and interpolation|Fitting data <br/> Interpolating between data|Sum of squared error <br/> Sum of absolute error <br/> Maximum absolute error <br/> `scipy.optimize.fmin()`<br/> `scipy.optimize.curve_fit()` <br/> `numpy.polyfit()` <br/> `numpy.polyval()` <br/> `scipy.interpolate.interp1d()`|[ipynb](curve-fitting-interpolation.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/curve-fitting-interpolation.html)|

### Linear Algebra
|Topic|Applications|Numerical Methods <br/> Python Skills|Jupyter <br/> Notebook|Online|
|-|-|-|:-:|:-:|
|Matrix operations in python|Dot product <br/> Norm <br/> Matrix multiplication|`@` <br/>`numpy.linalg.norm()`|[ipynb](matrix-operations.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/matrix-operations.html)|
|Solving linear systems <br/> with direct methods|Solving linear systems repeatedly|Matrix inversion <br/> LU decomposition <br/> `np.linalg.lu()` <br/> `scipy.linalg.solve()`|[ipynb](solving-linear-system-direct-method.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/solving-linear-system-direct-method.html)|
|Solving linear systems <br/> with iterative methods|Solving sparse linear systems|Jacobi method <br/> Gauss-Seidel method <br/> `numpy.linalg.eig()` <br/> `numpy.linalg.eigvals()`|[ipynb](solving-linear-system-iterative-method.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/solving-linear-system-iterative-method.html)|
|Singular value decomposition (SVD) <br/> (Principle component analysis, PCA)|Dimensionality reduction <br/> Image compression|SVD, PCA algorithm <br/> `scipy.linalg.svd()`|[ipynb](singular-value-decomposition-pca.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/singular-value-decomposition-pca.html)|

### Numerical Calculus
|Topic|Applications|Numerical Methods <br/> Python Skills|Jupyter <br/> Notebook|Online|
|-|-|-|:-:|:-:|
|Numerical differentiation|Differentiate functions <br/> Differentiate data|Forward difference <br/> Backward difference <br/> Central difference <br/> Other second order methods <br/> `numpy.gradient()`|[ipynb](numerical-differentiation.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/numerical-differentiation.html)|
|Numerical integration|Single integrals <br/> Double integrals <br/> Triple integrals <br/> (functions and data)|Left end point rule <br/> Right endpoint rule <br/> Midpoint rule <br/> Trapezoidal rule <br/> Simpson's rule <br/> `scipy.integrate.quad()` <br/> `scipy.integrate.dblquad()` <br/> `scipy.integrate.tplquad()`|[ipynb](numerical-integration.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/numerical-integration.html)|

### Ordinary Differential Equations (ODEs)
|Topic|Applications|Numerical Methods <br/> Python Skills|Jupyter <br/> Notebook|Online|
|-|-|-|:-:|:-:|
|Solving first-order ODEs|Solving first-order ODEs|Forward Euler <br/> Backward Euler <br/> Midpoint method <br/> Fourth-order Runge-Kutta (RK4) <br/> `scipy.integrate.solve_ivp()`|[ipynb](solving-first-order-odes.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/solving-first-order-odes.html)|
|Solving higher-order ODEs|Solving higher-order ODEs <br/> Systems of first-order ODEs|Forward Euler <br/> Backward Euler <br/> `scipy.integrate.solve_ivp()`|[ipynb](solving-higher-order-odes.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/solving-higher-order-odes.html)|
|Stability and stiffness of ODEs|Choosing integration methods <br/> Choosing time steps|Forward Euler <br/> Backward Euler <br/> `scipy.integrate.solve_ivp()`|[ipynb](ode-stability-stiffness.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/ode-stability-stiffness.html)|
|Phase portrait|Spring-mass-damper system|`scipy.integrate.solve_ivp()`|[ipynb](phase-portrait-spring-mass-damper.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/phase-portrait-spring-mass-damper.html)|
||Linear, nonlinear pendulum|`scipy.integrate.solve_ivp()`|[ipynb](phase-portrait-linear-nonlinear-pendulum.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/phase-portrait-linear-nonlinear-pendulum.html)|
||Two-eyed monster|`scipy.integrate.solve_ivp()`|[ipynb](phase-portrait-two-eyed-monster.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/phase-portrait-two-eyed-monster.html)|
||Population dynamics <br/> Predator-pray model <br/> Competition model|`scipy.integrate.solve_ivp()`|[ipynb](phase-portrait-population-dynamics.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/phase-portrait-population-dynamics.html)|
||FitzHugh-Nagumo neuron excitation model*|`scipy.integrate.solve_ivp()`|[ipynb](phase-portrait-neuron-excitation.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/phase-portrait-neuron-excitation.html)|
|Chaotic systems*|Lorenz system|`scipy.integrate.solve_ivp()`|[ipynb](chaotic-system-lorenz-system.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/chaotic-system-lorenz-system.html)|

### Fourier Transform
|Topic|Applications|Numerical Methods <br/> Python Skills|Jupyter <br/> Notebook|Online|
|-|-|-|:-:|:-:|
|Fourier transform*|Power spectrum density <br/> Noise filtering <br/> Image compression|Discrete Fourier transform <br/> Fast Fourier transform <br/> `numpy.fft.fft()` <br/> `numpy.fft.ifft()` <br/> `numpy.fft.fftfreq()` <br/> `numpy.fft.fft2()`|[ipynb](fourier-transform.ipynb)|[html](http://polarize.pw/equation-sheets/amath301/fourier-transform.html)|

### Gallery

https://user-images.githubusercontent.com/28213746/124108634-ec57e700-da98-11eb-884c-f9445fd4efa1.mp4

https://user-images.githubusercontent.com/28213746/124387428-3f3bd380-dd11-11eb-8297-a28c8c1170b8.mp4

https://user-images.githubusercontent.com/28213746/124387505-8c1faa00-dd11-11eb-99b6-60740dc88264.mp4

https://user-images.githubusercontent.com/28213746/124387609-d9038080-dd11-11eb-8e8c-37d8c09eb30d.mp4

https://user-images.githubusercontent.com/28213746/124387625-ede01400-dd11-11eb-88f5-e53396dfbff8.mp4

https://user-images.githubusercontent.com/28213746/124387640-f6d0e580-dd11-11eb-86f3-d8cb12b9b5e2.mp4

https://user-images.githubusercontent.com/28213746/124387672-0a7c4c00-dd12-11eb-9cd9-ea41135ca94c.mp4

https://user-images.githubusercontent.com/28213746/124387684-1536e100-dd12-11eb-94b5-47e98224ebaf.mp4

https://user-images.githubusercontent.com/28213746/124387692-19fb9500-dd12-11eb-9d0f-4748f6e39fba.mp4

https://user-images.githubusercontent.com/28213746/124387700-1ff17600-dd12-11eb-81ff-67a58142ef7a.mp4

https://user-images.githubusercontent.com/28213746/124387711-254ec080-dd12-11eb-83f2-d250d93c0c29.mp4

https://user-images.githubusercontent.com/28213746/124388349-1f0e1380-dd15-11eb-9d18-e1e1126f27fd.mp4

https://user-images.githubusercontent.com/28213746/124388376-41a02c80-dd15-11eb-8cc9-d7c69f0e9d87.mp4
