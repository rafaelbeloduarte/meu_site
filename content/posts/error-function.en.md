+++ 
draft = false
date = 2021-03-16T01:00:43-03:00
title = "Transport phenomena: Gauss error function and transient heat transfer"
description = ""
slug = "error-function" 
tags = ["chemical engineering", "transport phenomena"]
categories = []
externalLink = ""
series = []
+++

The Gauss error function (Equation \ref{eq1}) appears when you want to solve transient heat transfer problems.

$$
erf(x) = \frac{2}{\sqrt{\pi}} \int{e^{-x^2}} dx
\label{eq1} \tag{1}
$$

The complementary error function is:

$$
erfc(x) = 1 - erf(x)
\label{eq2} \tag{2}
$$

An example of its use is in solving the heat equation for a semi-infinite solid.

$$
\frac{\partial^2{T}}{\partial{x^2}} = \frac{1}{\alpha} \frac{\partial{T}}{\partial{t}} 
\label{eq3} \tag{3}
$$

**T** is the temperature, **x** the length (of a plate or soil depth for example), **$\alpha$** is the thermal diffusivity and **t** the time. The solution to this equation involves using a similar variable $ \eta \equiv \frac{x}{{4 \alpha t}^{1/2}} $. Derivatives of $\eta$ are calculated and replaced in Equation \ref{eq3}. After changing the variable, the partial differential equation is transformed into an ordinary differential equation that, when integrated, asks for the solution of the integral of Equation \ref{eq1}. The solution of Equation \ref{eq3} is:

$$
\frac{T(t)-T_s}{T_i-T_s} \equiv erf (\eta)
\label{eq4} \tag{4}
$$

Where **T(t)** is the temperature in time **t**, **$T_s$** the surface temperature (*constant and different from the initial temperature*) and **$ T_i $** the initial temperature.

The development, boundary conditions used and table with the values ​​of the **erf(x)** and **erfc(x)** functions are presented in detail by Incropera [^fn1].

## References

[^fn1]: Incropera, Frank P. DeWitt, David P. Bergman, Theodore L. Lavine, Adrienne S. Fundamentos de Transferência de Calor e Massa. 2008, 6ª ed. LTC: Rio de Janeiro, RJ. 










