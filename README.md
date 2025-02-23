
This repository includes the codes, posters and presentations of my publications. 

## Robust Sample-Based Output-Feedback  Path Planning (IROS2021)
We propose a novel approach for sampling-based and control-based motion planning that combines a representation of the environment obtained via modified version of optimal Rapidly-exploring Random Trees (RRT*), with landmark-based output-feedback controllers obtained via Control Lyapunov Functions, Control Barrier Functions, and robust Linear Programming. Our solution inherits many benefits of RRT*-like algorithms, such as the ability to implicitly handle arbitrarily complex obstacles, and asymptotic optimality. Additionally, it extends planning beyond the discrete nominal paths, as feedback controllers can correct deviations from such paths, and are robust to discrepancies between the map used for planning and the real environment.
We test our algorithms first in simulations and then in experiments, testing the robustness of the approach to practical conditions, such as deformations of the environment, mismatches in the dynamical model of the robot, and measurements acquired with a camera with a limited field of view.
\
\
You can read the paper from this link:
https://arxiv.org/abs/2105.14118
\

## Robust Path Planning and Control For Polygonal Environments via Linear Programming (ACC2021)
In this folder you can find the related material to "Robust Planning and Control For Polygonal Environments via Linear Programming" paper. In this work we find the robust output-feedback controller on a cell decomposition of a polygonal environment by using Control Lyapunov Function and Control Barrier Function constraints to provide guarantees of stability and safety through Linear Programming problem. The core of our proposed method consists of a convex min-max formulation that synthesizes an output-feedback controller, based on relative displacement measurements with respect to a set of landmarks. The optimization problem is formulated using piece-wise linear Control Lyapunov Function and Control Barrier Function constraints, to provide guarantees of stability and safety. The inner maximization problem ensures that these constraints are met by all the points in each cell, while the outer minimization problem balances the different constraints to optimize robustness. We convert this min-max optimization problem to a regular Linear Programming problem, by forming the dual of the inner maximization problem. Although in principle our approach is applicable to any system with piecewise linear dynamics, in this paper as a proof of concept, we apply it to first and second order integrators. We show through simulations that the resulting controllers are robust to significant deformations of the environment.
\
\
You can read the paper from this link:
https://arxiv.org/pdf/1910.07976.pdf
\

## Computational Theory of Robust Localization Verifiability in the Presence of Pure Outlier Measurements (CDC2019)
In this folder the materials for the "A Computational Theory of Robust Localization Verifiability in the Presence of Pure Outlier Measurements" are provided. In this paper we study the problem of localization of a pose graph given the outliers by implementaing the Linear Programming problem. In practical situations, the accuracy of the relative measurements is marred by noise and outliers; hence, we have the problem of quantifying how much we should trust the solution returned by some given localization solver. In this work, we focus on the question of whether an L1-norm robust optimization formulation can recover a solution that is identical to the ground truth, under the scenario of translation-only measurements corrupted exclusively by outliers and no noise; we call this concept verifiability. On the theoretical side, we prove that the verifiability of a problem depends only on the topology of the graph of measurements, the edge support of the outliers, and their signs, while it is independent of ground truth locations of the nodes, and of any positive scaling of the outliers. On the computational side, we present a novel approach based on the dual simplex algorithm that can check the verifiability of a problem, completely characterize the space of equivalent solutions if they exist, and identify subgraphs that are verifiable. As an application of our theory, we provide a procedure to compute a priori probability of recovering a solution congruent or equivalent to the ground truth given a measurement graph and the probabilities of each edge containing an outlier. 
\
\
You can read the paper from this link:
https://ieeexplore.ieee.org/abstract/document/9029819

