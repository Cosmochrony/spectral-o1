This repository contains the source of the **O1** Cosmochrony paper  
[*Projective Resolution Dynamics on Variable-Valence Relaxation Graphs*](out/SpectralO1.pdf).

This work extends the **spectral relaxation programme** by showing that the
asymptotic saturation of the projective resolution found in the fixed-valence
LPS model is not intrinsic to the relational substrate.

While **Spectral Relaxation** established that fixed-valence expander graphs
lead to an asymptotically static projective threshold and an inverted ADE
ordering, the present work investigates the minimal structural modification
needed to restore a non-trivial dynamics of projective resolution.

The central idea is to allow the effective relational valence of the substrate
to grow along the cascade:

$p(n) \to \infty$.

This causes the Kesten--McKay spectral support to contract and generates
a rank-dependent exit of ADE spectral levels.

# Core Result

The paper studies **variable-valence LPS sequences**

$G_n = X_{p(n),q(n)}$

with

$p(n) \to \infty$.

Along such a sequence, the width of the Kesten--McKay support satisfies

$\mathrm{width}_{KM}(p(n)) = \frac{4\sqrt{p(n)}}{p(n)+1} \to 0$.

Both support edges converge to the midpoint

$\lambda = 1$

at rate

$\frac{2}{\sqrt{p(n)}}$.

Thus, as the cascade proceeds, the spectral window contracts around its centre.

# ADE Exit Order

For the binary icosahedral case with the order-5 generating set, the three ADE levels are

$\lambda^{ADE}_1 = \frac{5}{6}, \qquad
\lambda^{ADE}_2 = 1, \qquad
\lambda^{ADE}_3 = \frac{5}{4}$.

As the Kesten--McKay support contracts, these levels leave the support in a fixed order:

1. $\lambda^{ADE}_3 = \frac{5}{4}$ exits first, at  
   $p_3^\ast = (4+\sqrt{15})^2 \approx 62$

2. $\lambda^{ADE}_1 = \frac{5}{6}$ exits second, at  
   $p_1^\ast = (6+\sqrt{35})^2 \approx 142$

3. $\lambda^{ADE}_2 = 1$ never exits for finite $p$

This exit order is determined purely by the geometry of the contracting support
and is independent of the detailed growth law of $p(n)$.

# Restored Projective Dynamics

In the fixed-valence regime, the projective threshold saturates because the
spectral gap approaches a constant lower edge of a static Kesten--McKay support.  
In the variable-valence regime, this plateau disappears.

The analysis shows that allowing $p(n) \to \infty$:

- removes the fixed-valence saturation plateau
- restores a non-trivial dynamical regime for $\Lambda_{\mathrm{proj}}(n)$
- couples admissibility to support-exit geometry rather than to a static cumulative count

This is the minimal structural modification needed to recover genuine threshold dynamics.

# Effective Mass Ordering

A spectral level that exits the support becomes non-admissible and stabilises at
the corresponding cascade rank.

Earlier exit therefore corresponds to higher effective stabilisation mass.

The support-exit order implies the mass ordering

$M_3 > M_1 > M_2$.

This corrects the fixed-valence inversion

$M_1 < M_2 < M_3$

found in **Spectral Relaxation**, and does so through a purely geometric mechanism
requiring no additional dynamical hypothesis.

# What O1 Resolves

The variable-valence mechanism resolves the main structural defect of the fixed-valence regime:

- the projective threshold is no longer asymptotically static
- the ADE levels no longer remain trapped inside a fixed support
- the ordering inversion is corrected by support geometry itself

In this sense, O1 removes the structural obstruction to a viable hierarchy.

# Residual Limitation

O1 does **not** by itself fully reproduce the observed inter-generational amplitude.

The paper shows that the variable-valence mechanism decouples the stabilisation ranks
of the generations and allows stronger suppression than the fixed-valence formula, but
the observed hierarchy

$ m_e / m_\tau \approx 3 \times 10^{-4} $

still requires additional structure.

Two directions are identified for completing the amplitude problem:

- **(O2)** a hierarchical cascade acting recursively across multiple nested levels
- **(O3)** a sub-linear energy-rank relation

Thus O1 restores the correct structural ordering, but does not close the full amplitude gap on its own.

# Conceptual Structure

O1 connects several components of the Cosmochrony framework:

1. Projective resolution from the relaxation-graph spectrum
2. Kesten--McKay support geometry in Ramanujan graph families
3. ADE spectral levels from Spectral Stratigraphy
4. Variable relational valence along the cascade
5. Geometric generation of stabilisation ordering by support contraction

The resulting framework establishes that the ordering of generations can emerge
from the geometry of a moving spectral support.

# Physical Interpretation

In the Cosmochrony framework, the relaxation graph encodes the relational connectivity
of the substrate at cascade depth $n$.

The fixed-valence regime corresponds to a substrate whose effective connectivity does
not evolve along the cascade.

The variable-valence regime

$p(n) \to \infty$

corresponds instead to an increase of effective relational valence along the cascade.
This causes the spectral support to contract and generates a genuine stratification of
stabilisation events.

Support contraction therefore acts as a spectral mechanism for generation ordering. :contentReference[oaicite:5]{index=5}

# Open Directions

Three open directions remain:

1. **Amplitude problem**  
   O1 corrects the ordering but must be combined with O2 or O3 to reach the observed
   hierarchy amplitude.

2. **Level-to-generation map**  
   The structural ordering $M_3 > M_1 > M_2$ is established, but its identification
   with specific Standard Model generations is not yet derived from first principles.

3. **Upper bound on $\Lambda_{\mathrm{proj}}(n)$**  
   The present paper controls the lower Ramanujan edge; sharper control of the upper
   Cheeger bound in the variable-valence regime remains open.

# Status

This framework is:

- spectral-geometric
- analytically explicit
- structurally minimal
- compatible with spectral admissibility, spectral stratigraphy,
  and spectral relaxation

It does not assume:

- particle fields
- quantum statistics
- additional dynamical hypotheses beyond variable relational valence

# Repository Structure
```
paper/
├── pdf/ # Compiled O1 PDF
├── tex/ # LaTeX sources
└── README.md
```

# Citation

If you reference this work, please cite:

> J. Beau, *Projective Resolution Dynamics on Variable-Valence Relaxation Graphs*, Zenodo, 2026.

# Acknowledgements

Portions of the derivations, numerical verification, and editorial
refinement benefited from iterative interactions with large language
models used as analytical assistants.  
All theoretical results and interpretations remain the sole responsibility
of the author.

# Contributions

This repository is intended as a research reference.

Critical feedback, independent spectral analyses, and alternative
variable-valence constructions are welcome.

Please open an issue to discuss conceptual points,
technical details, or possible extensions.
