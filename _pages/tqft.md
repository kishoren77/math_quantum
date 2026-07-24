---
layout: single
title: "4. Future Work: TQFT"
permalink: /tqft/
nav_exclude: true
---

### From Strings to Surfaces

In the previous sections, we modeled quantum mechanics using 1-dimensional string diagrams. However, the category of finite-dimensional Hilbert spaces ($$\mathbf{FdHilb}$$) shares a deep structural equivalence with the category of 2D cobordisms ($$\mathbf{Bord}_2$$). 

My future research for this program will involve inflating our 1D string diagrams into 2D topological surfaces.

### The Geometry of $$\mathbf{Bord}_2$$

In the topological category $$\mathbf{Bord}_2$$, we replace discrete points and wires with manifolds:
* **Objects** are 1D closed manifolds (circles). A single qubit system is represented by a circle.
* **Morphisms** are 2D surfaces (cobordisms) that connect these circles as time flows upward.
* **The Identity** ($$\text{id}_A$$) is a straight cylinder (a circle moving forward in time undisturbed).
* **The Cup** (State Preparation) is a U-shaped tube (like a piece of macaroni). It starts smooth and closed at the bottom and opens into two circles at the top.
* **The Cap** (Measurement) is an upside-down tube (like a pair of pants). It takes two circles at the bottom, merges them, and closes them smoothly at the top.

### Topological Teleportation

If we reconstruct the teleportation protocol in $$\mathbf{Bord}_2$$, we plug Alice's input cylinder and the U-shaped Cup into the upside-down Cap measurement. 

Topologically, this forms a continuous, hollow **"S"-shaped pipe**. 

Because $$\mathbf{Bord}_2$$ is governed by smooth deformations, pulling on the ends of an "S"-shaped rubber pipe perfectly straightens it out into a single, straight cylinder. Therefore, the geometry natively proves the Snake Equation: an S-pipe is topologically equal to an Identity cylinder. Teleportation is simply the act of straightening a tube!

### The TQFT Functor

To make this mathematically rigorous, my next step is to study Topological Quantum Field Theories (TQFTs). A TQFT is formally defined as a symmetric monoidal functor mapping the topological category to the quantum category:

$$Z: \mathbf{Bord}_2 \to \mathbf{FdHilb}$$

This functor acts as a perfect translation manual. It maps the geometric stretching of 2D surfaces directly onto the linear operators of standard quantum mechanics, uniting the geometry of manifolds with the flow of quantum information.

***

[Back to Home](/)
