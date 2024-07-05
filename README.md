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


In the above equation, $p(𝑥)$ and $q(𝑥)$ are undefined at $𝑥 = 0$, but we can still apply the Frobenius method if $𝑥_0$ is a regular singular point of ODE. The solution, according to Frobenius, is by $y(x)=\sum{_{n=0}}^{{\infty}}{a_nx^{n+r}=x^r(a_0+a_1x+\ldots)}$.

$𝑥_0$ is the regular singular point of $y^{\prime\prime}+p\left(x\right)y^\prime+q\left(x\right)y=0$ if $(𝑥 − 𝑥_0)𝑝(𝑥)$ and $(𝑥 − 𝑥_0)^2𝑞(𝑥)$ exists and has valid Taylor expansion about $𝑥_0$. The exponent r (may be real or complex) number should be chosen such that $𝑎_0 ≠ 0$. Now, there exists a class of 2nd order, linear ODEs with variable coefficients of the form: 
$x^2y^{\prime\prime}+xy^\prime+{(x}^2-\ m^2)y=0$

The Bessel function of the first kind of $m^{th}$ order is given by:

$J_m(x) = \sum{_{l=0}^{\infty}}\frac{(-1)^l}{2^{2l+m}l!(m+l)!}x^{2l+m}$ 

$Y_m\left(x\right)=\ \frac{J_m\left(x\right)\cos{\pi m}-J_{-m}(x)}{\sin{\pi m}}$

The behaviour of the Bessel functions of first kind $J_m$ of order ‘m’ are shown below:

![image](https://user-images.githubusercontent.com/111849605/202916473-6bd3e3f8-fbee-48f9-8d73-7e38f1ef11a9.png)

The behaviour of the Bessel functions of second kind $Y_𝑚$ of order ‘m’ are shown below:

![image](https://user-images.githubusercontent.com/111849605/202916498-5cf8a8ae-9a1b-4253-b5e2-7cfa3b497c5d.png)

A general solution of Bessel’s function for the Bessel ODE is given by 
$𝑦(𝑥) = 𝐶_1 𝐽_𝑚 + 𝐶_2 𝑌_m$

APPLICATION: CYLINDER WITH ENERGY 
GENERATION

A long solid cylinder of radius ro is initially at uniform temperature Ti. Electricity 
is suddenly passed through the cylinder, resulting in a volumetric heat generation rate 
of qm. The cylinder is cooled by convection at its surface. The heat transfer 
coefficient is considered as $h$, and the ambient temperature is considered as $T_\infty$. The 
objective is to determine the transient temperature profile of the cylinder and its evolution.

![image](https://user-images.githubusercontent.com/111849605/202916632-87f27e67-30ce-47da-aca1-85c195ad8645.png)

Assumptions:
1. One-dimensional conduction.
2. Uniform $h$ and $T_\infty$.
3. Constant conductivity.
4. Constant diffusivity.
5. Negligible end effect.


Governing Equations:
To make the convection boundary condition homogeneous, we introduce the 
following temperature variable
$θ (r,t) = T(r,t) -$ $T_\infty$ 

Based on the above assumptions, it gives

$\frac{\partial^2\theta}{\partial r^2}+\frac{1\partial\theta}{r\partial r}+\frac{q^m}{k}=\frac{1\partial\theta}{\propto\partial t}$ ---(A)

Boundary and initial conditions:

[1] $\frac{\partial\theta\left(0,t\right)}{\partial r}=0\ or\ \theta\left(0,t\right)=finite\ $

[2] $-k\frac{\partial\theta\left(r_0,t\right)}{\partial r}=h\theta\left(r_0,t\right)$

[3] $θ(r,t = 0) = T_i - T_\infty $


Solution:
Since the differential equation is non-homogeneous, we assume a solution of the form 

$𝜃(𝑟,𝑡) = 𝜑(𝑟,𝑡) + ∅(𝑟)$       ---(a)

Note that $Ψ(r-t)$ depends on two variables while $ϕ(r)$ depends on one 
variable. Substituting $(a)$ into eq. $(A)$

$\frac{\partial^2\varphi}{\partial r^2}+\frac{1\partial\varphi}{r\partial r}+\frac{d^2\emptyset}{dr^2}+\frac{1d\emptyset}{rdr}+\frac{q^m}{k}=\frac{1\partial\varphi}{\propto\partial t}$ ---(b)

The next step is to split (b) into two equations, one for Ψ(r-t) and the other 
for ϕ(r). Let

$\frac{∂^2φ}{∂r^2}+\frac{1}{r}\frac{∂φ}{∂r}= \frac{1}{\alpha}\frac{∂φ}{∂t}$  ---(c)

$\frac{d^2\emptyset}{dr^2}+\frac{1d\emptyset}{rdr}+\frac{q^m}{k} = 0$  ---(d)

To solve equations (c) and (d), we need two boundary conditions for each 
and an initial condition for (c). Substituting (a) into boundary condition (1)

$\frac{\partial\varphi(0,t)}{\partial r}+\frac{d\emptyset(0)}{dr}=0$

Let $\frac{\partial\varphi(0,t)}{\partial r}=0\ or\ \varphi(0,t)=finite\$ ---(c-1)

Thus $\frac{d\emptyset(0)}{dr}=0$ ---(d-1)

Similarly, condition (2) gives

$-k\frac{\partial\varphi\left(r_o,t\right)}{\partial r}=h\varphi(r_o,t)$ ---(c-2)

$-k\frac{d\emptyset\left(r_o\right)}{\partial r}=h\emptyset(r_o)$ ---(d-2)

Now, the initial condition gives

$\varphi\left(r,0\right)=\left(T_i-T_\infty\right)-\emptyset(r)$ ---(c-3)

Integrating (d) gives

$\emptyset\left(r\right)=-\frac{q^m}{4k}r^2+c_1lnr+c_2$  ---(3)

Equation (c) is solved by the method of separation of variables. Assume a product solution of the form

$\varphi\left(r,t\right)=R\left(r\right)\tau\left(t\right)$ ---(f)


Substituting (f) into (c), separating variables, and setting the resulting equation 
equal to a constant, $±(λ_k)^2$, gives

$\frac{d^2R_k}{dr^2}+\frac{1dR_k}{rdr}\ \mp\lambda_k^2R_k=0$ ---(g)

$\frac{d^2\tau_k}{dt}\ \mp\lambda_k^2{\alpha\tau}_k=0$ ---(h)

Since the r-variable has two homogeneous conditions, the plus sign must be 
selected in (g). Equations (g) and (h) become

$\frac{d^2R_k}{dr^2}+\frac{1dR_k}{rdr}+\lambda_k^2R_k=0$ ---(i)

$\frac{d^2\tau_k}{dt}+\lambda_k^2{\alpha\tau}_k=0$ ---(j)

Solutions to the ODE (i) are given by general Bessel representation, and (ii) is exponential decay:

$R_k\left(r\right)=A_kJ_0\left(\lambda_kr\right)+B_kY_0\left(\lambda_kr\right)$ ---(k)

and 

$\tau_k\left(t\right)=C_k\exp(-\lambda_k^2\alpha t)$ ---(l)

Application to boundary and initial conditions.
Conditions (c-1) and (c-2) give
$𝐵_𝑘 = 0$
 and
$BiJ_0(\lambda_kr_0)=\ (\lambda_kr_0)J_1(\lambda_kr_0)$ ---(m)
Where Bi is the Biot number defined as Bi = hr_0 / k. The roots of $m$ give the 
constants $λ_k$. Substituting (k) and (l) into (f) and summing all solutions

$\mathrm{\Psi}(r-t)\ =\sum{_{k=1}^{\infty}}{a_k\exp{(-{\lambda_k}^2\alpha t)}J_0(\lambda_kr).}$ ---(n)

Returning to solution (e) for $ϕ(r)$, boundary conditions (d-1) and (d-2) give the constants $C_1$ and $C_2$. Thus (e) becomes

$\phi\left(r\right)=\frac{q^m}{4k}\left({r_0}^2-r^2\right)+\frac{q^mr_0}{2h}$ ---(o)

Application of the non-homogeneous initial condition (c-3) yields

$\left(T_i-T_\infty\right)-\phi\left(r\right)\ =\sum{_{k=1}^{\infty}}{a_kJ_0\left(\lambda_kr\right).}$ ---(p)

The characteristic functions J0 ((λ_k)*r) in equation (p) are solutions to (i). This is a 
Sturm-Liouville equation guarantees that there are infinitely many eigenvalues, and the function is orthogonal when the boundary conditions are 
homogeneous w.r.t. weight function $w(r) = r$.
Multiplying both sides of (p) by $J_0(λ_kr)r dr$, integrating from $r =0$ to $r =r_0$ and invoking orthogonality gives $a_k$

$a_k=\frac{2\lambda_k\int_{0}^{r_0}{\left[\left(T_i-T_\infty\right)-\phi(r)\right]\ J_0\left(\lambda_kr\right)rdr}}{\int_{0}^{r_0}{\ {J_0}^2\left(\lambda_kr\right)rdr}}$ ---(q)

Substituting (o) into (q) and evaluating the integral gives,

$a_k=\ \frac{2\left(\lambda_kr_0\right)(T_i-T_\infty)}{({Bi}^2+\lambda_k^2r_0^2)J_0^2(\lambda_kr_0)}\left\{\left[1-\frac{q^mr_0^2}{k(T_i-T_\infty)}\left(\frac{1}{2Bi}+\frac{1}{\lambda_k^2r_0^2}\right)\right]J_1\left(\lambda_kr_0\right)+\frac{q^mr_0^2}{k(T_i-T_\infty)}\frac{J_0\left(\lambda_kr_0\right)}{\left(\lambda_kr_0\right)}\right\}$

Complete Solution:
Hence, the complete solution, expressed in dimensionless form, is

$\frac{T\left(r,t\right)-T_\infty}{T_i-T_\infty}=\frac{q^mr_0^2}{4k(T_i-T_\infty)}\left[1-\frac{r^2}{r_0^2}+\frac{2}{Bi}\right]+\frac{1}{T_i-T_\infty}\sum_{k=1}^{\infty}{a_k\exp(-\lambda_k^2\alpha t)J_0\left(\lambda_kr\right)$
