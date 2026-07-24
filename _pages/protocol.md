---
layout: single
title: "3. The Teleportation Protocol"
permalink: /protocol/
nav_exclude: true
---

### The Setup: State Preparation and Entanglement

We can now formalize the Quantum Teleportation protocol entirely within the graphical calculus of our dagger compact category. 

Suppose Alice possesses an unknown quantum state that she wishes to transmit to Bob. We define this state as a morphism from the identity object: $$\psi: I \to A$$. 

To facilitate the teleportation, Alice and Bob must share a maximally entangled bipartite state. Using our compact structure, this is the unit (the "Cup"): 

$$\eta: I \to A^* \otimes A$$

Alice holds the subsystem $$A^*$$and Bob holds the subsystem$$A$$. Therefore, the total initial state of the system is the parallel composition of Alice's state and the entangled pair: $$\psi \otimes \eta$$.

### The Execution: Bell Measurement

To teleport the state, Alice must perform a joint measurement on the two subsystems in her possession (her original state $$A$$and her half of the entangled pair$$A^*$$). 

In our categorical dictionary, projecting two subsystems onto a scalar (a Bell measurement) is precisely the counit (the "Cap"): 

$$\epsilon: A \otimes A^* \to I$$

Graphically, Alice routes her state wire $$\psi$$ and her side of the entangled Cup into a Cap. 

### The Proof of Teleportation

Algebraically, the entire teleportation process can be written as the composition of Alice's measurement with the prepared state, leaving Bob's subsystem intact:

$$(\epsilon \otimes \text{id}_A) \circ (\psi \otimes \eta)$$

In standard matrix mechanics, proving this requires tracking 3-qubit state vectors, tensor products, and explicit Pauli unitary corrections. However, in the graphical calculus, this entire algebraic derivation reduces to a few intuitive geometric steps.

![Quantum Teleportation Protocol](/math_quantum/assets/images/teleportation.png)

Here is how the topological proof unfolds:

1. **Setup:** The initial state wire $$L$$, the Bell measurement (Cap), and the entangled pair (Cup) are assembled with the unitary transformation $$U$$.
2. **Sliding Operators:** Using the duality properties of caps and cups, the operator $$U$$ slides smoothly along the wire.
3. **Unitary Cancellation:** The operators combine and cancel out ($$U^\dagger U = \text{id}_L$$), leaving a continuous, unadorned string.
4. **Topological Simplification:** By the axioms of dual objects, we apply the **Snake Equation**:

$$(\epsilon \otimes \text{id}_A) \circ (\text{id}_{A^*} \otimes \eta) = \text{id}_A$$

Topologically, this pulls the continuous S-curve taut into a single, straight vertical wire on system $$L$$. 

Without writing a single matrix, the diagram formally reduces to $$\text{id}_A \circ \psi$$, which is simply $$\psi$$ on Bob's subsystem. The state has been perfectly teleported!


***

[Next: 4. Future Work: Topological Quantum Field Theories](/math_quantum/tqft/)
