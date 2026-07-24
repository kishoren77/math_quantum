---
layout: single
title: "3. The Teleportation Protocol"
permalink: /protocol/
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

*(Insert your drawing of the full Teleportation Protocol / Snake Equation here)*
`![The Teleportation Protocol](/assets/images/snake.png)`

### The Proof of Teleportation

Algebraically, the entire teleportation process can be written as the composition of Alice's measurement with the prepared state, leaving Bob's subsystem intact:

$$(\epsilon \otimes \text{id}_A) \circ (\psi \otimes \eta)$$

While this looks complex algebraically, the graphical calculus makes the outcome trivial. By tracing the wires in the diagram from bottom to top, we observe that Alice's measurement (the Cap) and the entangled state (the Cup) form a continuous, S-shaped curve connected to the input state $$\psi$$.

By the axioms of dual objects, we simply apply the **Snake Equation**:

$$(\epsilon \otimes \text{id}_A) \circ (\text{id}_{A^*} \otimes \eta) = \text{id}_A$$

Topologically, the S-shaped zigzag pulls taut into a single, straight vertical wire. The diagram formally reduces to $$\text{id}_A \circ \psi$$, which is simply $$\psi$$ on Bob's subsystem. The state has been perfectly teleported. 

*(Note: In physical systems, Alice's measurement yields classical outcomes that require Bob to apply unitary corrections. However, in the abstract categorical framework, the underlying geometric flow of information is completely captured by the deformation of the string diagram.)*

***

[Next: 4. Future Work: Topological Quantum Field Theories](/tqft/)
