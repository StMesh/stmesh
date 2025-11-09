## Hi there 👋
Starlike Design has developed a new approach to mesh restoration design, with prototype implementations, St*Mesh, and its successor, CO2Mesh.   The latter is a rewrite to generalize its application to multiyear designs and enable use of reinforcement learning and probabilistic programming techniques.  This website, still under construction, describes these implementations.

 

The optimization approach can be thought of as an alternative to greedy heuristics, motivated by constraint programming, that produces designs better than greedy heuristics, close to the quality of mixed integer programming (MIP) models, with more fidelity to the current state of the network and performance requirements for restoration paths.  The runtime is somewhere between the two.  Since constraint programming allows the planner to model the network in a natural way, changes can be made quickly.  And paradoxically, as more constraints and network context data are introduced, the algorithms here tend to run faster, not slower.

 

By analogy with AlphaGo, St*Mesh produces designs somewhere in between human-produced and MIP-optimized designs, in the sense that small changes in parameters or network data usually have small and predictable changes in the design.  Designs are interpretable, being produced by an AI-adaption of a sequential decision model.  In contrast, some heuristics and most MIP-optimized designs are often radically changed -- hopping from an old global minimum to a new one.

 

St*Mesh uses a relatively weak optimization technique combined an accurate problem formulation, decision reordering, partial instantiation, and limited but predictive search.   It excels at problems more complex than unit-cost, single layer networks.  Where subproblems are coupled enough that committing to a decision in an early subproblem can lead to suboptimal results, the techniques in St*Mesh can shine.   Multilayer network designs fall into this category.

 

The examples (net5, net8) shown here address the weakest case for St*Mesh:  single layer designs with no express links and unit-valued cost models.  We ask whether the St*Mesh approach can produce designs close to a good greedy heuristic algorithm, SSR, and how close to optimal solutions from a branch-and-bound algorithm.
<!--
**StMesh/stmesh** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
