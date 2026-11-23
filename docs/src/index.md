# LyapunovStability.jl

Lyapunov stability analysis for dynamical systems in Julia.

`LyapunovStability.jl` provides tools for stability verification and
invariance-based analysis of polyhedral sets.

Positive Invariance is a property of a set whose trajectory, once inside that set, remains in it. It is particulary usefull when dealing with constraints in a control problem.

We can represent the constraints as a set of linear inequalities that can define bounds on the variables.

Such inequalities in the state space define a convex polyhedron on `mathbb{R}^n` writed as:

``\Omega = \{x \in \mathbb{R}^n : Fx \leq w\}, \quad
F \in \mathbb{R}^{f \times n}, \quad w \in \mathbb{R}^f.
``

In this pkg we work with this type of 

## Installation

Install the package directly from GitHub:

```bash
git clone https://github.com/Nicholas-Wallace/LyapunovStability.jl
```

After clone the repository you can add this package to any julia project by running

```julia
julia> ]
pkg> dev path/to/LyapunovStability.jl 
```

The package will also be available from the General registry once registered.

## Quick start

A quick-start example to start using the pkg.

To define a polyhedral set 

## Contents

- [Systems](guide/systems.md)
- [Invariance](guide/invariance.md)
- [Trajectories](guide/trajectories.md)
- [Plotting](guide/plotting.md)
- [Examples](examples.md)
- [API Reference](api.md)
