---
toc: true
layout: post
description: "haha."
categories: ["imaging"]
title: "The Mathematics Behind Magnetic Resonance Imaging"
image: images/2020-06-13-mri_files/_display.png
badges: true
comments: true
hide: true
search_exclude: true
permalink: /mri/
---



# Introduction
Magnetic Resonance Imaging (MRI) is one of the most imaging technique 


# Background
Hydrogen


# The Bloch Equation

$$
\frac{d\mathbf{M}}{dt} = \gamma \mathbf{M}\times \mathbf{B} - \frac{<M_x,M_y,0>}{T_2} - \frac{<0,0,M_z-M_{eq}>}{T_1}
$$


$$
\frac{dM_x}{dt} = \gamma B_0 M_y(t) - \frac{M_x(t)}{T_2}
$$


$$
\frac{dM_y}{dt} = -\gamma B_0 M_x(t) - \frac{M_y(t)}{T_2}
$$

$$
\frac{dM_z}{dt} = -\frac{M_z(t)-M_{eq}}{T_1}
$$


$$
M_x(t) = e^{-t/T_2} \left(  M_x(0)\cos(\omega_0 t) - M_y(0)\sin(\omega_0 t)    \right)
$$

$$
M_y(t) = e^{-t/T_2} \left(  M_x(0)\sin(\omega_0 t) + M_y(0)\cos(\omega_0 t)    \right)
$$

$$
M_z)t) = M_z(0) e^{-t/T_1} + M_{eq}\left(   1-e^{-t/T_1}   \right)
$$
where $\omega_o = -\gamma B_0$. 



# The RF Field

$$
\mathbf{B}_1 = <2B_1\cos(\omega t),0,0>
$$

# RF Pulse Sequences: $T_1$ and $T_2$

$90^\circ$ pulse filps


# Gradients and Slice Selection

$$
\mathbf{B}_G(\mathbf{p}) = <0,0,G_1 x + G_2 y + G_3 z> = <0,0,\mathbf{G}\cdot\mathbf{p}>
$$


# The Imaging Equation

$$
S(t) = K \int M^*(t,\mathbf{p})\exp(-i\omega t) d \mathbf{p}
$$


# References


