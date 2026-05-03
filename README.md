# Convex Analysis & Minimax Theory Study Plan

**Objective:** Learn about minimax theory, saddle point problems, and convex duality with the goal of eventually diving into applications such as proximal methods and their derivatives, e.g. PDHG. 

## Reading material
* **Pure Math & Topology:** *Convex Analysis* by R. Tyrrell Rockafellar
* **Theoretical Exercises:** *Fundamentals of Convex Analysis* by J.-B. Hiriart-Urruty & C. Lemaréchal
* **Applications (Computational):** *Convex Optimization* by Stephen Boyd & Lieven Vandenberghe
* **A Specialized Reference (Smooth KKT):** *Nonlinear Programming* by Olvi Mangasarian

---

## Phase 1: Geometry, Topology & Sets
*Goal: Understand how inequalities and non-smooth boundaries behave, and try to master particularly critical topological concepts such as the "relative interior."*

- [ ] **Rockafellar | Sec 1 & 2:** Affine sets and convex sets.
- [ ] **Rockafellar | Sec 4:** The calculus of convex sets.
- [ ] **Rockafellar | Sec 6:** Closure and Relative Interior. *(Crucial)*
- [ ] **Rockafellar | Sec 7 & 8:** Convex functions and closed convex functions.
- [ ] **Hiriart-Urruty | Exercises:** Complete 3-5 exercises on finding the affine hull, convex hull, and relative interior of sets.
- [ ] **Physics Mental Check:** Map separating hyperplanes to planes of constant potential; view convex combinations as valid system superpositions.

## Phase 2: Duality
*Goal: Transition from primal spaces to dual spaces. This is the rigorous, nonsmooth generalization of the Lagrangian-to-Hamiltonian mechanics ubiquituous in physics. Try to write extra notes on this particular topic.*

- [ ] **Rockafellar | Sec 11:** Conjugate functions (The Fenchel conjugate, $f^*$).
- [ ] **Rockafellar | Sec 12:** Conjugates of convex functions. *(Crucial: Focus on the biconjugate theorem $f^{**} = f$).*
- [ ] **Rockafellar | Sec 13:** Support functions.
- [ ] **Hiriart-Urruty | Exercises:** Calculate Fenchel conjugates for various functions by hand to build algebraic intuition.
- [ ] **Optional | Notes:** Understand and write some notes on the conncection between the above topics and analytical mechanics.

## Phase 3: Optimality Conditions (Subdifferentials & KKT)
*Goal: Learn to take derivatives of non-differentiable convex functions to find true minima/maxima, then see how this looks in smooth, constrained systems.*

- [ ] **Rockafellar | Sec 23:** Directional derivatives and subgradients.
- [ ] **Rockafellar | Sec 24:** Subdifferentials.
- [ ] **Hiriart-Urruty | Exercises:** Practice calculating subdifferentials for functions with "kinks" (e.g., absolute value equivalents).
- [ ] **Mangasarian | Reference Reading:** Read sections on Fritz John and Karush-Kuhn-Tucker (KKT) optimality conditions. Compare the smooth KKT inequalities to Rockafellar's subdifferential inclusions.
- [ ] **Mangasarian | Reference Reading:** Briefly review Generalized Convexity (Quasi-convex/Pseudo-convex) to see how "imperfect" potential wells are handled.

## Phase 4: Minimax & Saddle Points
*Goal: Understand the abstract mathematical conditions under which $\min \max = \max \min$.*

- [ ] **Rockafellar | Sec 33:** Convex-Concave Functions and Saddle Points.
- [ ] **Rockafellar | Sec 34:** Closures of Saddle Functions.
- [ ] **Rockafellar | Sec 36:** The Minimax Theorem.
- [ ] **Rockafellar | Sec 37:** Conjugate Saddle Functions.

## Phase 5: Applications
*Goal: Ground the abstract, infinite-dimensional saddle points in computationally heavy, physical reality.*

- [ ] **Boyd | Chapter 5:** Read "Duality". Treat this as a grand review.
- [ ] **Boyd | Exercises:** Complete numerical exercises mapping abstract minimax theorems onto concrete Lagrangians and matrix games.

---
