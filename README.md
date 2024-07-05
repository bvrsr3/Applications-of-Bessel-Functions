# Bessel-Function
- This repository contains codes for plotting and visualizing Bessel functions and their applications:

Several second-order ODEs of the form 𝒚'' + 𝒑(𝒙)𝒚' + 𝒒(𝒙)𝒚 = 𝒓(𝒙) are of practical importance have power series solution $y(x)=\sum{_{n=0}^{n=\infty}}(x-x_0)^n$


Coefficients $p(x)$, $q(x)$ and $r(x)$ can be functions instead of constant coefficients. Further, if they have valid Taylor series expansion about point $x_0$, it implies that they must be continuously differentiable about that point i.e. they are analytical at that point.
If the coefficients $p(x)$, $q(x)$, $r(x)$ are not analytical at point $𝑥_0$ but if we still require 
a power series solution at that point, in order to exploit the larger radius of 
convergence, we use the Frobenius method. The Frobenius method masks the point of 
singularity, thereby creating a feasible solution at which the power series method 
fails. Such points are called regular singular points.


Consider an ODE:
$y^{\prime\prime}+\frac{2}{x}y^\prime+\frac{1}{x^2}y=0$


In the above equation, $p(𝑥)$ and $q(𝑥)$ are undefined at $𝑥 = 0$, but we can still apply the Frobenius method if $𝑥_0$ is a regular singular point of ODE. The solution, according to Frobenius, is by $y(x)=\sum{_{n=0}^{\infty}}{a_nx^{n+r}=x^r(a_0+a_1x+\ldots)}$.

$𝑥_0$ is the regular singular point of $y^{\prime\prime}+p\left(x\right)y^\prime+q\left(x\right)y=0$ if $(𝑥 − 𝑥_0)𝑝(𝑥)$ and $(𝑥 − 𝑥_0)^2𝑞(𝑥)$ exists and has valid Taylor expansion about $𝑥_0$. The exponent r (may be real or complex) number should be chosen such that $𝑎_0 ≠ 0$. Now, there exists a class of 2nd order, linear ODEs with variable coefficients of the form: 
$x^2y^{\prime\prime}+xy^\prime+{(x}^2-\ m^2)y=0$

The Bessel function of the first kind of mth order is given by:

$J_m(x) = \sum_{l=0}^{\infty}\frac{(-1)^l}{2^{2l+m}l!(m+l)!}x^{2l+m}$ 

$Y_m\left(x\right)=\ \frac{J_m\left(x\right)\cos{\pi m}-J_{-m}(x)}{\sin{\pi m}}$

The behaviour of the Bessel functions of first kind 𝐽𝑚 of order ‘m’ are shown below:

![image](https://user-images.githubusercontent.com/111849605/202916473-6bd3e3f8-fbee-48f9-8d73-7e38f1ef11a9.png)

The behaviour of the Bessel functions of second kind $𝑌_𝑚$ of order ‘m’ are shown below:

![image](https://user-images.githubusercontent.com/111849605/202916498-5cf8a8ae-9a1b-4253-b5e2-7cfa3b497c5d.png)

A general solution of Bessel’s function for the Bessel ODE is given by 
𝑦(𝑥) = 𝐶_1 𝐽_𝑚 + 𝐶_2 𝑌_m

APPLICATION: CYLINDER WITH ENERGY 
GENERATION

A long solid cylinder of radius ro is initially at uniform temperature Ti. Electricity 
is suddenly passed through the cylinder resulting in volumetric heat generation rate 
of qm. The cylinder is cooled by convection at its surface. The heat transfer 
coefficient is considered as h and the ambient temperature is considered as T∞. The 
objective is to determine the transient temperature of the cylinder.

![image](https://user-images.githubusercontent.com/111849605/202916632-87f27e67-30ce-47da-aca1-85c195ad8645.png)

Assumptions:
1. One dimensional conduction.
2. Uniform h and T∞.
3. Constant conductivity.
4. Constant diffusivity.
5. Negligible end effect.


Governing Equations:
To make the convection boundary condition homogeneous, we introduce the 
following temperature variable
θ (r,t) = T(r,t) - T∞.

Based on the above assumptions, gives
![image](https://user-images.githubusercontent.com/111849605/202916684-d1567327-02f0-4df0-af1b-827bedbc45ed.png)

Boundary and initial conditions:
![image](https://user-images.githubusercontent.com/111849605/202916698-af4de2b0-91d0-48af-802c-f905b65733be.png)

Solution:
Since the differential equation s non-homogeneous, we assume a solution of 
the form
𝜃(𝑟,𝑡) = 𝜑(𝑟,𝑡) + ∅(𝑟)       (a)

Note that Ψ(r-t) depends on two variables while ϕ(r) depends on one 
variable. Substituting (a) into eq. (A)

![image](https://user-images.githubusercontent.com/111849605/202916775-2f6bba63-c6d3-427b-a271-5f4f25a00214.png)   (b)




The next step is to split (b) into two equations, one for Ψ(r-t) and the other 
for ϕ(r). Let..

![image](https://user-images.githubusercontent.com/111849605/202916818-234dcd21-bb41-4d11-ba03-ad559e0b231a.png)  (c)
![image](https://user-images.githubusercontent.com/111849605/202916837-365981ec-514c-4567-be2e-fedc62962083.png)  (d)

To solve equations (c) and (d) we need two boundary conditions for each 
and an initial condition for (c). Substituting (a) into boundary condition (1)

![image](https://user-images.githubusercontent.com/111849605/202916857-25467901-9a32-4a32-8ce6-e0e984838731.png)

![image](https://user-images.githubusercontent.com/111849605/202916914-895f8fef-e4f2-4129-bc00-044e6f9f7e1c.png)

![image](https://user-images.githubusercontent.com/111849605/202916978-cfed8d9d-5ebb-434d-9e81-127fdb314762.png)

Similarly, condition (2) gives

![image](https://user-images.githubusercontent.com/111849605/202917007-ed29c56c-9371-4eea-8f6c-ea6f64fdc33d.png)

![image](https://user-images.githubusercontent.com/111849605/202917022-0093bf68-a6c4-482b-a8e7-12b49d201bf8.png)

Now, the initial condition gives
𝜑(𝑟, 0) = (𝑇𝑖 − 𝑇∞) − ∅(𝑟)          (c-3)

Integrating (d) gives
∅(𝑟) = −(𝑞_𝑚/4𝑘)*𝑟^2 + 𝑐1𝑙𝑛𝑟 + 𝑐2        (e)


Equation (c) is solved by the method of separation of variables. Assume a product 
solution of the form
𝜑(𝑟,𝑡) = 𝑅(𝑟)𝜏(𝑡) (f)
Substituting (f) into (c), separating variables, and setting the resulting equation 
equal to a constant, ±(λ_k)^2, gives

![image](https://user-images.githubusercontent.com/111849605/202917183-d13aa5b0-274a-4ba2-b427-0407881fb6c8.png)

![image](https://user-images.githubusercontent.com/111849605/202917204-8166cbd1-d77f-4c07-ae46-22ae38c741b7.png)

ince the r-variable has two homogeneous conditions, the plus sign must be 
selected in (g). Equations (g) and (h) become

![image](https://user-images.githubusercontent.com/111849605/202917221-2104658c-0620-486d-95aa-530f3a4ca9e5.png)

![image](https://user-images.githubusercontent.com/111849605/202917234-ee908b3a-fc90-41c6-9767-7c7a7186b15e.png)

Solutions to the ODE (i) is given by general Bessel representation and (ii) is 
exponential decay:
𝑅_𝑘(𝑟) = (𝐴_𝑘)*𝐽0
(𝜆_𝑘)*r + (𝐵_𝑘)*𝑌0*(𝜆_𝑘)*r               (k)

and 
𝜏_𝑘(𝑡) = (𝐶_𝑘)exp(−𝛼*𝑡*(𝜆_𝑘)^2)                    (l)

Application to boundary and initial conditions.
Conditions (c-1) and (c-2) give
𝐵_𝑘 = 0
 and
Bi*𝐽0*(𝜆_𝑘)𝑟0 = (𝜆_𝑘)*𝑟0*𝐽1*(𝜆_𝑘)*𝑟0                   (m)
Where Bi is the Biot number defined as Bi = hr0 / k. The roots of (m) give the 
constants λk. Substituting (k) and (l) into (f) and summing all solutions

![image](https://user-images.githubusercontent.com/111849605/202917491-935c8203-346d-494b-88a9-bba8b48b4727.png)

Application of the non-homogeneous initial condition (c-3) yields

![image](https://user-images.githubusercontent.com/111849605/202917526-28953577-6e23-4583-a7f6-d2c00d55b6ce.png)

The characteristic functions J0 ((λ_k)*r) in equation (p) are solutions to (i). This is a 
Sturm-Liouville equation that guarantees that there are infinitely many eigen 
values and the function is orthogonal when the boundary conditions are 
homogeneous w.r.t. weight function w(r) = r.
Multiplying both sides of (p) by J0((λ_k)*r)*r dr, integrating from r =0 to r =r0 and 
invoking orthogonality gives a_k

![image](https://user-images.githubusercontent.com/111849605/202917723-7e7599a0-7fc5-4cfa-9c0d-e4181a94436b.png)

Substituting (o) into (q), and evaluate the integral gives,


![image](https://user-images.githubusercontent.com/111849605/202917743-a2920a33-547f-44b9-b88f-49dbc5c2b1bf.png)

Complete Solution:
Hence the complete solution, expressed in dimensionless form, is

![image](https://user-images.githubusercontent.com/111849605/202917779-b8c32fa7-6895-4b59-8f58-c38bb36caf74.png)

