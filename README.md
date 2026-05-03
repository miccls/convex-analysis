# Convex Analysis & Minimax Theory Study Plan

**Objective:** Learn about minimax theory, saddle point problems, and convex duality with the goal of eventually diving into applications such as proximal methods and their derivatives, e.g. PDHG. 

## Reading material
* **Pure Math & Topology:** *Convex Analysis* by R. Tyrrell Rockafellar  
* **Theoretical Exercises:** *Fundamentals of Convex Analysis* by J.-B. Hiriart-Urruty & C. Lemaréchal  
* **Applications (Computational):** *Convex Optimization* by Stephen Boyd & Lieven Vandenberghe  
* **A Specialized Reference (Smooth KKT):** *Nonlinear Programming* by Olvi Mangasarian  

---

## Phase 1: Geometry, Topology & Sets
*Goal: Mathematical fundamentals for the rest of the studies. Covering convex sets and functions as well as separation theorems. Try to master particularly critical topological concepts such as the "relative interior."*

- [ ] **Rockafellar | Sec 1, 2 & 3:** Affine sets and convex sets.
- [ ] **Rockafellar | Sec 4:** The calculus of convex sets.
- [ ] **Rockafellar | Sec 6:** Closure and Relative Interior. *(Crucial)*
- [ ] **Rockafellar | Sec 7 & 8:** Convex functions and closed convex functions.
- [ ] **Hiriart-Urruty | Convex sets:** Separation theorems and supporting hyperplanes. Particularly A.4 if the rest feels like it has been covered by Rockafellar. *(Crucial)*
- [ ] **Hiriart-Urruty | Exercises:** Complete 3–5 exercises on affine hull, convex hull, and relative interior.
- [ ] **Hiriart-Urruty | Exercises:** Do 2–3 exercises involving separation or supporting hyperplanes.
- [ ] **Checkpoint:** Be able to state and interpret a separation theorem geometrically and in inequality form.

---

## Phase 2: Duality
*Goal: Transition from primal spaces to dual spaces. This is the rigorous, nonsmooth generalization of the Lagrangian-to-Hamiltonian mechanics ubiquitous in physics.*

- [ ] **Rockafellar | Sec 11:** Separation Theorems. *(Crucial)*
- [ ] **Rockafellar | Sec 12:** Conjugates of convex functions.
- [ ] **Rockafellar | Sec 13:** Support functions.
- [ ] **Rockafellar | (within these sections):** Fenchel duality theorem (statement and interpretation).
- [ ] **Hiriart-Urruty | Exercises:** Compute Fenchel conjugates for several functions.
- [ ] **Hiriart-Urruty | Exercises:** Derive simple dual problems of the form $\inf_x f(x) + g(Ax)$.
- [ ] **Checkpoint:** Understand separation as existence of a linear functional distinguishing convex sets.
- [ ] **Checkpoint:** Be able to interpret dual problems as $\inf \sup$ structures.
- [ ] **Optional | Notes:** Brief notes linking conjugates, duality, and Legendre transform ideas.

---

## Phase 3: Optimality Conditions (Subdifferentials & KKT)
*Goal: Learn to take derivatives of non-differentiable convex functions to find true minima/maxima, then see how this looks in smooth, constrained systems.*

- [ ] **Rockafellar | Sec 23:** Directional derivatives and subgradients.
- [ ] **Rockafellar | Sec 24:** Subdifferentials.
- [ ] **Boyd | 5.1–5.3:** Lagrangian, dual function, weak/strong duality.
- [ ] **Boyd | 5.5:** KKT conditions.
- [ ] **Task:** Rewrite constrained problems as  
  $\inf_x \sup_{\lambda \ge 0} L(x,\lambda)$ and $\sup_{\lambda \ge 0} \inf_x L(x,\lambda)$.
- [ ] **Task:** Interpret KKT conditions as a saddle point condition.
- [ ] **Hiriart-Urruty | Exercises:** Compute subdifferentials for nonsmooth functions.
- [ ] **Boyd | Exercises:** Select problems on forming duals and verifying KKT.
- [ ] **Checkpoint:** Move between subdifferentials, KKT conditions, and saddle point formulations.
- [ ] **Mangasarian | Optional:** Read Fritz John and KKT conditions for comparison.
- [ ] **Mangasarian | Optional:** Brief look at generalized convexity.

---

## Phase 4: Minimax & Saddle Points
*Goal: Understand the abstract mathematical conditions under which $\min \max = \max \min$.*

- [ ] **Rockafellar | Sec 33:** Convex–concave functions and saddle points.
- [ ] **Rockafellar | Sec 34:** Closures of saddle functions.
- [ ] **Rockafellar | Sec 36:** The minimax theorem.
- [ ] **Rockafellar | Sec 37:** Conjugate saddle functions.
- [ ] **Supplement:** Sion’s minimax theorem (as a clean reference statement).
- [ ] **Task:** Rewrite results in the form $\inf_x \sup_y f(x,y) = \sup_y \inf_x f(x,y)$.
- [ ] **Task:** Identify assumptions (convexity, compactness, closure) and their roles.
- [ ] **Checkpoint:** Explain minimax as a consequence of convex–concave structure and duality.

---

## Phase 5: Applications
*Goal: Ground the abstract, infinite-dimensional saddle points in computational settings.*

- [ ] **Boyd | Chapter 5 (review):** Revisit duality and KKT.
- [ ] **Boyd | 5.6 (selected):** Work through concrete duality examples (QP, LP, norm problems).
- [ ] **Boyd | Exercises:** Focus on:
  - deriving dual problems  
  - verifying KKT conditions  
  - checking strong duality  
- [ ] **Task:** Map each example to a saddle-point formulation.
- [ ] **Optional Extension:** Identify how these structures relate to primal–dual methods (e.g., PDHG at a high level).

---

## Minimal global checkpoints

At the end of the plan, you should be able to:

- Rewrite optimization problems as saddle problems  
- Explain when $\inf \sup = \sup \inf$  
- Move between:
  - conjugates  
  - dual problems  
  - KKT conditions  
  - minimax theorems  