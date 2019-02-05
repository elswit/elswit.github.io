+++
title = "Multirate Time-stepping Methods"
description = ""
date = 2014-11-18T02:13:50Z
author = "Arash Sarshar"
+++

# Multirate methods for multi-physics problems

We study the theory for derivation and applications of multi-rate time integration schemes for the evolution of multi-scale PDEs. The main idea is to integrate different splittings of the target PDE differently, according to evaluation cost and/or stability requirements. If we can identify the stiff operators that need much smaller timesteps, we can use multirate methods to advance _"fast-changing"_ parts of the PDE with smaller time-steps. In a similar approach, we can integrate the stiff parts of the PDE implicitly, thereby benefiting from increased stability, while at the same time the non-stiff parts are evaluated explicitly for computational efficiency. We show the computational efficiency of these methods in different numerical experiments when compared to conventional methods of the same class. 

See [[slides]] (https://docs.google.com/presentation/d/1M43xXqBg24S0TZVmhumRr_c_FNAICulXwpaRKIR-eTs/pub?start=false&loop=false&delayms=30000)  | [[ Report]] | [[Videos]] for this project


## Example PDE: Convection-Diffusion equation

<a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;\dpi{150}&space;\LARGE&space;\begin{align*}&space;\frac{\partial&space;u}{\partial&space;t}-&space;\underbrace{{\color{Red}&space;\varepsilon&space;\nabla^2&space;u}}_{\text{stiff}}&space;&plus;\underbrace{{\color{Blue}&space;\vec{w}&space;\cdot&space;\nabla&space;u}}_{\text{non-stiff}}&space;&=&space;0&space;\quad&space;\text{in}&space;\quad&space;\Omega&space;\end{align*}" target="_blank"><img src="https://latex.codecogs.com/png.latex?\inline&space;\dpi{150}&space;\LARGE&space;\begin{align*}&space;\frac{\partial&space;u}{\partial&space;t}-&space;\underbrace{{\color{Red}&space;\varepsilon&space;\nabla^2&space;u}}_{\text{stiff}}&space;&plus;\underbrace{{\color{Blue}&space;\vec{w}&space;\cdot&space;\nabla&space;u}}_{\text{non-stiff}}&space;&=&space;0&space;\quad&space;\text{in}&space;\quad&space;\Omega&space;\end{align*}" title="\LARGE \begin{align*} \frac{\partial u}{\partial t}- \underbrace{{\color{Red} \varepsilon \nabla^2 u}}_{\text{stiff}} +\underbrace{{\color{Blue} \vec{w} \cdot \nabla u}}_{\text{non-stiff}} &= 0 \quad \text{in} \quad \Omega \end{align*}" /></a>

{{< youtube ecansWMhTbo >}}



