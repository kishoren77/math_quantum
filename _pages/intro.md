---
layout: single
title: "1. Categorical Quantum Mechanics"
nav_exclude: true
---
 
### Monoidal Categories and Quantum Systems

The foundational premise of Categorical Quantum Mechanics (CQM) is that the abstract structure of quantum information can be completely formalized using the framework of category theory, specifically bypassing standard matrix algebra in favor of a rigorous graphical calculus. 

We formalize a physical theory as a **strict monoidal category** $$(\mathbf{C}, \otimes, I)$$. 

* **Objects** ($$A, B, C \in \text{Ob}(\mathbf{C})$$) represent physical systems (e.g., Finite-Dimensional Hilbert Spaces, $$\mathbf{FdHilb}$$). 
* **Morphisms** ($$f: A \to B$$) represent physical processes or state evolutions (e.g., linear operators).
* **The Tensor Product** ($$\otimes: \mathbf{C} \times \mathbf{C} \to \mathbf{C}$$) represents the composition of systems.
* **The Identity Object** ($$I$$) represents the trivial system (in $$\mathbf{FdHilb}$$, this is the complex field $$\mathbb{C}$$). 

### The Graphical Calculus

Any equation in a strict monoidal category is mathematically valid if and only if it can be proven using string diagrams up to planar isotopy. We assign:

1. **Wires** to objects $$A$$. Time flows from bottom to top.
2. **Boxes** to morphisms $$f$$.
3. **Sequential Composition** ($$g \circ f$$) is drawn by stacking $$g$$ on top of $$f$$. 
4. **Parallel Composition** ($$f \otimes g$$) is drawn by placing $$f$$ and $$g$$ side-by-side.

A state vector $$|\psi\rangle \in A$$is simply a morphism from the identity object:$$\psi: I \to A$$. Graphically, this is a box with no input wires and one output wire (a triangle). 

***

[Next: Dagger and Compact Structures](/math_quantum/math/)
