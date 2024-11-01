## Deep Learning Methods in Fluid Dynamics
<a href="https://www.iitg.ac.in/swaroop/studsup.html#:~:text=Deep%20learning%20Methods%20in%20Fluid%20Dynamics"> BTP</a>(B.Tech Project) under **Professor <a href="https://www.iitg.ac.in/swaroop/">Swaroop</a> Nandan Bora** Sir

## 1. Solving Burger equation with deep learning method.
see [burger.ipynb](https://github.com/Upeshjeengar/Deep-learning-Methods-in-Fluid-Dynamics/blob/main/burger.ipynb)
---

## 2. Solving the Wave Equation with Deep Learning Based Method
see [wave_equation.ipynb](https://github.com/Upeshjeengar/Deep-learning-Methods-in-Fluid-Dynamics/blob/main/wave_equation.ipynb)
This project solves the wave equation:

$$
\frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2}
$$

where $c = 1$, and the initial conditions are given by:

$$
u(x, 0) = \phi(x) = \sin(x), \quad u_t(x, 0) = \psi(x) = \cos(x)
$$

The boundary conditions are:

$$
u(0,t) = 0 = u(L,t)
$$

### Exact Solution

The exact solution for this problem is expressed as an infinite Fourier series:

$$
u(x,t) = \sum_{n=1}^{\infty} \sin\left(\frac{n\pi x}{L}\right) \left( A_n \cos\left(\frac{n\pi t}{L}\right) + B_n \sin\left(\frac{n\pi t}{L}\right) \right)
$$

#### Coefficients:

The coefficients $A_n$ and $B_n$ are determined using the initial conditions. They are given by:

$$
A_n = \frac{2}{L} \int_0^L \sin(x) \sin\left(\frac{n\pi x}{L}\right) dx
$$

$$
B_n = \frac{2}{n\pi L} \int_0^L \cos(x) \sin\left(\frac{n\pi x}{L}\right) dx
$$

## 3. Wave equation with external disturbances
![image](https://github.com/user-attachments/assets/d638d389-b3a8-418b-8a5a-e1cc2a241d84)

## 4. Euler Beam equation
![image](https://github.com/user-attachments/assets/cbbe40a3-1654-47c3-bd12-37571621f54a)

assume:
ϕ(x)=sin⁡(πx/L)
and
ψ(x)=0

Resources:   
1.  [Physics Informed Deep Learning](https://arxiv.org/abs/1711.10561v1)

