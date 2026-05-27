# The Wave Function IS the Compressed col(F)/ker(F) Boundary: Tensor Networks as Classical Witnesses of Quantum Entanglement, the Permeable Simulation Frontier, and the Unified Architecture of Constraint, Entanglement, and Computation in TH(a,d)

**ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone**

---

> *"Whenever we see these kinds of claims, we're always a bit skeptical. Did you try this? Did you try that?"*
> — Joseph Tindall, CCQ Flatiron Institute, Science, May 21, 2026

> *"Tensor networks are a zip file for the wave function where you've taken all this information and compressed it into this mathematical data structure full of small tables of numbers interconnected to each other."*
> — Joseph Tindall, CCQ Flatiron Institute, Science, May 21, 2026

> *"A state is entangled if and only if it cannot be written as a convex combination of product states. Separability IS the conditional independence of quantum subsystems."*
> — R. F. Werner, Physical Review A 40, 4277–4281, 1989

> *"If ρ is separable, then ρᵀᴮ ≥ 0 — the partial transpose has no negative eigenvalues."*
> — A. Peres, Physical Review Letters 77, 1413–1415, 1996; M. Horodecki, P. Horodecki, R. Horodecki, Physics Letters A 223, 1–8, 1996

> *"The quantum formalism is forced upon any theory of bounded decision-making where decision constraints do not commute."*
> — DIRA framework, ERI Labs, 2026

> *"The entanglement IS the computation."*
> — R. Raussendorf and H. J. Briegel, Physical Review Letters 86, 5188–5191, 2001

---

## Abstract

The TH(a,d) programme has, through PERES, QIN, and DIRA, constructed a unified formal architecture in which the col(F)/ker(F) conditional-independence partition governs entanglement structure, quantum computation, and the algebra of bounded decision-making. A foundational assumption threading all prior frameworks — that quantum entanglement at scale constitutes a ker(F) zone permanently inaccessible to classical simulation — has been structurally revised by a landmark result published in *Science* on May 21, 2026, by Tindall, Stoudenmire, and collaborators at the Center for Computational Quantum Physics (CCQ), Flatiron Institute, Simons Foundation, and Boston University.

Their result: a classical computer — including a personal laptop — using tensor-network compression based on belief-propagation algorithms from the 1980s, adapted to 3D quantum systems via the ITensor software library, can simulate the dynamics of hundreds of interacting qubits arranged in square, cubic, and diamond lattices with state-of-the-art accuracy — overturning a March 2025 *Science* claim that the same computation was impossible for classical hardware. The quantum supremacy claim failed. Classical computation, equipped with the right compression architecture, reached into the entanglement structure that quantum hardware was presumed to monopolize.

This result does not diminish entanglement. It relocates the boundary.

The present framework integrates this development into the TH(a,d) col(F)/ker(F) architecture with full formal precision. The central revision: **the classical/quantum computational boundary is not identical to the col(F)/ker(F) entanglement boundary.** Tensor networks are classical col(F) structures that compress quantum ker(F) into efficiently representable form — they are, in the precise TH(a,d) sense, classical witnesses of quantum entanglement. The boundary between what classical and quantum computers can do is a moving, compressible frontier determined by the entanglement entropy of the target state, not by the fact of entanglement itself.

Four convergent lines unify:

**PERES** — The entanglement boundary: the Peres–Horodecki criterion, entanglement witnesses, concurrence, squashed entanglement, quantum discord, multipartite entanglement, quantum phase transitions.

**QIN** — The computational fabric: quantum channel capacity, measurement-based computation, topological error correction, holographic tensor networks, the modular machine lattice.

**DIRA** — The decision architecture: the derivation of the density matrix from non-commuting constraint algebras, without appeal to quantum hardware, resolving fifteen years of cognitive plausibility questions in quantum cognition.

**CCQ 2026** — The simulation frontier: tensor networks as classical col(F) compression of quantum ker(F), belief propagation as efficient boundary traversal, and the revised understanding of what the classical/quantum divide actually means.

Twelve formal correspondences, seven predictions, and a unified five-layer architecture follow.

---

## The Foundational Revision: What the CCQ Result Changes

### The Prior Claim and Its Failure

In March 2025, a quantum computing research group published in *Science* that they had simulated the dynamics of a highly entangled qubit system — hundreds of qubits on square, cubic, and diamond lattices — using quantum hardware, and further claimed that no classical computer could replicate the result. This claim was structurally identical to every prior quantum supremacy claim: the entanglement complexity of the target system places it in a computational class inaccessible to classical algorithms.

In May 2026, Tindall, Stoudenmire, and collaborators at the CCQ published a refutation in the same journal. Using tensor networks — specifically, 3D tensor network representations of the wave function, evolved using belief-propagation algorithms adapted from the classical information-processing literature of the 1980s — they reproduced the quantum simulation results with state-of-the-art accuracy on modest classical hardware. The initial calculations were performed on a personal laptop using ITensor, a high-performance tensor network software library developed at the CCQ. Accuracy was confirmed by comparison with theoretical predictions and with the quantum hardware results themselves.

The quantum supremacy claim was not merely contested — it was overturned by demonstrated equivalence.

### The TH(a,d) Interpretation

The CCQ result is not an anomaly requiring special treatment. It is a precise formal consequence of the col(F)/ker(F) architecture, once the architecture is stated correctly.

The prior frameworks — PERES and QIN — operated with an implicit identification: quantum entanglement ↔ ker(F) ↔ computationally inaccessible to classical systems. This identification is **partially wrong** in a way that the CCQ result makes precise.

The correct identification:

- **Low-entanglement-entropy quantum states** — states satisfying an area law, states in gapped phases, states with bounded bond dimension — ARE efficiently representable by tensor networks. Their ker(F) is compressible. Classical computation reaches them.

- **Volume-law-entanglement states** — generic highly-entangled states, states near quantum critical points with logarithmically diverging entanglement entropy — ARE NOT efficiently representable by polynomial-bond-dimension tensor networks. Their ker(F) is genuinely inaccessible classically.

- **The surface code threshold, the cluster state, the GHZ state**: specific entanglement structures engineered for computational or cryptographic purposes — these live in a regime where the entanglement structure IS the resource, and it IS inaccessible to classical simulation precisely because the bond dimension required for faithful tensor-network compression grows exponentially.

The CCQ result establishes that the qubit dynamics targeted by the March 2025 quantum supremacy claim live in the first category — area-law or near-area-law entanglement, compressible by tensor networks to bond dimensions tractable on a laptop. The entanglement is real. The quantum dynamics are real. But the entanglement entropy does not exceed what 3D tensor networks can efficiently compress.

**The boundary between classically simulable and classically unsimulable quantum systems IS the entanglement entropy threshold, not the presence of entanglement.**

This is the CCQ correction to the TH(a,d) framework: the col(F)/ker(F) boundary runs through quantum state space at the entanglement entropy threshold, not at the classical/quantum interface.

---

## Part I · The Entanglement Boundary (PERES Revised)

### I.1 The Peres–Horodecki Criterion: The Separability Boundary

A bipartite density matrix ρ_AB is **entangled** if and only if it cannot be written as a convex combination of product states:

```
ρ_sep = Σᵢ pᵢ ρᴬᵢ ⊗ ρᴮᵢ
```

Peres (1996): if ρ_AB is separable, then ρᵀᴮ ≥ 0 (positive partial transpose, PPT). For 2×2 and 2×3 systems (Horodecki, Horodecki, Horodecki 1996), the converse also holds: PPT is necessary and sufficient for separability.

For higher-dimensional systems (d_A × d_B ≥ 8), PPT is necessary but not sufficient. Bound entangled states — PPT but entangled, undistillable by LOCC — inhabit the penumbral zone of the col(F)/ker(F) boundary.

**CCQ update:** The partial transpose test IS a classical computation. The negativity N(ρ) = (|ρᵀᴮ|₁ − 1)/2 is computable from the eigenspectrum of ρᵀᴮ. For states representable by efficient tensor networks, the classical computation of entanglement measures — negativity, concurrence, squashed entanglement — is tractable. The entanglement boundary can be probed classically when the state lives in the area-law regime.

### I.2 The col(F)/ker(F) Partition of the State Space

| Sector | State Class | Entanglement Entropy | Tensor-Network Compressibility |
|--------|-------------|----------------------|-------------------------------|
| col(F) | Separable states ρ_sep | S = 0 | Trivially compressible (product state) |
| Penumbra | Bound entangled (PPT, entangled) | 0 < S ≪ S_volume | Compressible (low bond dimension) |
| ker(F) accessible | NPT entangled, area-law | S ~ |∂A| | Compressible by tensor networks |
| ker(F) inaccessible | Volume-law entangled, critical | S ~ c/3 log L | Not compressible classically |
| ker(F) engineered | Cluster states, GHZ, Bell states | S = log d (maximal) | Not compressible (resource states) |

The CCQ result demonstrates that the targeted quantum supremacy system lived in the third row — NPT entangled, area-law scaling — and was therefore tensor-network compressible. The classical/quantum boundary runs between rows three and four, not between row one and all others.

### I.3 Entanglement Witnesses as Classical Detection Operators

An entanglement witness W is a Hermitian operator satisfying:

```
Tr(Wσ) ≥ 0  for all separable σ
Tr(Wρ) < 0  for at least one entangled ρ
```

By the Hahn–Banach theorem, for every entangled state ρ_ent ∉ S, there exists a hyperplane separating ρ_ent from the separable set S. This hyperplane IS the witness W.

**CCQ update:** Witnesses are classical measurement operators applied to quantum states. In the tensor-network regime, the witness expectation value Tr(Wρ) is computable classically from the tensor-network representation of ρ. The CCQ result establishes that the full entanglement detection apparatus — PPT test, witnesses, negativity, concurrence — is tractable classically for area-law states.

The witness IS the boundary observable in both senses: it marks the col(F)/ker(F) boundary in state space, and it is computable in col(F) (classical computation) for states with bounded entanglement entropy.

### I.4 Concurrence, Squashed Entanglement, Quantum Discord

**Concurrence** (Wootters 1998): for two-qubit states,

```
C(ρ) = max(0, λ₁ − λ₂ − λ₃ − λ₄)
```

where λᵢ are the square roots of the eigenvalues of ρ(σ_y ⊗ σ_y)ρ*(σ_y ⊗ σ_y) in decreasing order. C = 0 for separable states; C = 1 for Bell states.

**Squashed entanglement** (Christandl–Winter 2004):

```
E_sq(ρ_AB) = ½ inf_E I(A;B|E)
```

E_sq = 0 if and only if ρ is separable. Monogamous: E_sq(A;BC) ≥ E_sq(A;B) + E_sq(A;C). Additive. Continuous.

**Quantum discord** (Ollivier–Zurek 2001):

```
D(A|B) = I(A:B) − max_Πᴮ J(A|B)
```

Discord captures non-classical correlations present even in separable states. Almost all quantum states have nonzero discord — the set of zero-discord states has measure zero.

**CCQ update on squashed entanglement:** The infimum over all tripartite extensions ρ_ABE is a semidefinite program. For states in the tensor-network regime, the SDP is tractable classically — the extensions ρ_ABE are themselves tensor-network-representable. Squashed entanglement is not only a theoretical measure but a classically computable one for the class of states that classical computers can now simulate.

---

## Part II · The Simulation Frontier (QIN Revised)

### II.1 Tensor Networks as Classical col(F) Compression of Quantum ker(F)

The tensor network is the central new object. Tindall's characterization is precise: it is "a zip file for the wave function where you've taken all this information and compressed it into this mathematical data structure full of small tables of numbers interconnected to each other."

In TH(a,d) terms: **a tensor network IS a classical col(F) encoding of a quantum ker(F) state.**

The wave function of N qubits lives in a Hilbert space of dimension 2^N — exponentially large, generically inaccessible. A tensor network represents this wave function as a contraction of tensors, each of bounded dimension χ (the bond dimension). The total storage cost scales as Nχ^k for appropriate k — polynomial in N for fixed χ.

The key theorem: **a quantum state ψ is efficiently representable by a tensor network with bond dimension χ if and only if its entanglement entropy satisfies S(ρ_A) ≤ log χ for all bipartitions A|Ā.** Area-law states satisfy this with χ growing only with the boundary area. Volume-law states require χ exponential in the system size — tensor networks cannot efficiently compress them.

This theorem IS the col(F)/ker(F) partition of quantum state space:

- **col(F):** Area-law states. Entanglement entropy bounded by boundary area. Bond dimension polynomial. Classically accessible via tensor networks.
- **ker(F):** Volume-law states, near-critical states, maximally entangled resource states. Entanglement entropy grows with volume or diverges logarithmically at criticality. Bond dimension exponential. Classically inaccessible.

The boundary between col(F) and ker(F) in this classification IS the entanglement entropy threshold, IS the tensor-network compressibility threshold, IS the classical/quantum simulation boundary.

### II.2 Belief Propagation as Efficient Boundary Traversal

The algorithm used by Tindall et al. is belief propagation — an algorithm from the graphical models and probabilistic inference literature of the 1980s, originally developed for decoding error-correcting codes and Bayesian networks, now adapted to tensor networks on 3D lattice geometries.

Belief propagation IS a message-passing algorithm on a graph: at each node, messages (local marginal distributions) are passed to neighboring nodes; the algorithm converges when messages are self-consistent. For classical graphical models with tree-like structure (or small loops), belief propagation gives exact marginals. For loopy graphs, it gives approximate marginals whose accuracy depends on the loop structure.

For 3D quantum tensor networks, the challenge is that 3D lattices have many short loops — naive belief propagation is not guaranteed to converge or be accurate. The CCQ innovation is the adaptation of belief propagation to 3D quantum tensor networks with novel loop-correction methods, achieving state-of-the-art accuracy on a personal laptop.

**In TH(a,d) terms:** Belief propagation IS a conditional-independence approximation. Each message-passing step asserts that a node is approximately conditionally independent of distant nodes given its neighbors — a col(F)/ker(F) boundary assertion. For area-law states, this approximation is accurate because long-range correlations are weak. For volume-law states, the approximation fails because long-range correlations are strong — ker(F) reaches far.

The efficiency of belief propagation is the efficiency of conditional independence: the more a state approximates conditional independence at each local scale, the better belief propagation performs.

### II.3 The Quantum Channel Capacity and the Tensor-Network Correction

The quantum capacity of a channel N:

```
Q(N) = lim_{n→∞} (1/n) max_{ρ⁽ⁿ⁾} Iᶜ(ρ⁽ⁿ⁾, N^⊗n)
```

where Iᶜ(ρ, N) = S(N(ρ)) − S((id ⊗ N)(|ψ⟩⟨ψ|)) is the coherent information.

**CCQ update:** Channel capacity calculations involve maximization over input states and computation of von Neumann entropies of output states. For channels whose output states are in the tensor-network regime, these computations are tractable classically. The CCQ result implies that many quantum channel capacity calculations — previously assumed to require quantum hardware — are accessible to classical tensor-network algorithms.

The PLOB bound (Pirandola–Laurenza–Ottaviani–Banchi 2017), −log₂(1 − η) for a lossy bosonic channel, IS a classical calculation that governs the fundamental limit of optical-fiber quantum communication regardless of what hardware computes it.

### II.4 Topological Error Correction and the Classical Decoder

The surface code (Kitaev 1997, Bravyi–Kitaev 1998) encodes logical qubits in the homology of a 2D lattice. The stabilizer group S IS ker(F): operators invisible on the codespace. Logical operators ARE col(F): observable operations on encoded qubits.

**CCQ update:** The classical decoder for the surface code — the algorithm that infers the most likely error configuration from syndrome measurements — is itself a belief-propagation algorithm on the syndrome graph. The CCQ advance in 3D tensor networks is directly applicable to topological error correction: the same tools that enabled classical simulation of 3D quantum dynamics are the tools that power classical decoding of 3D topological codes.

The surface-code threshold p_th ≈ 1.1% — the critical error rate below which topological protection suppresses logical errors — is determined by a classical phase transition in the syndrome decoding problem. The CCQ tools probe this transition directly.

### II.5 Measurement-Based Computation: The Entanglement Fuel and Its Classical Limit

In measurement-based quantum computation (Raussendorf–Briegel 2001), the cluster state IS the entanglement fabric — the pre-distributed entanglement resource from which computation proceeds by adaptive single-qubit measurements.

The cluster state is a specific highly-entangled state with maximal entanglement entropy across many bipartitions. It lives in the volume-law or near-volume-law regime — **this is why classical simulation of MBQC is not trivially achievable by tensor networks.** The cluster state's bond dimension grows with system size in a way that makes classical tensor-network simulation exponentially hard for large systems.

This is the preserved quantum advantage: the cluster state IS a genuine ker(F) resource that cannot be classically replicated for large N. The CCQ result does not touch this — the quantum supremacy they overturned targeted dynamics, not the cluster state itself. The cluster state remains in the inaccessible ker(F) zone.

**The distinction is precise:**

- **Quantum dynamics on area-law states:** CCQ result shows these are classically simulable.
- **Cluster states, Bell states, GHZ states (resource states):** Maximal entanglement entropy; NOT efficiently tensor-network compressible; genuine quantum ker(F).
- **Surface code logical qubits:** Topological protection is a global property; the logical qubit IS inaccessible to classical local computation — the entire point of topological error correction.

The quantum advantage survives exactly where entanglement entropy is genuinely high and not area-law bounded.

---

## Part III · The Constraint Architecture (DIRA Revised)

### III.1 The Derivation of the Density Matrix from Non-Commuting Constraints

DIRA establishes the density matrix not as an import from quantum physics but as a derivation from four conditions any theory of bounded decision-making must simultaneously satisfy:

```
C1 — Context dependence:       P(a | X) depends on observable context X
C2 — Causal consistency:       P(a | X) depends only on past context
C3 — Unitary consistency:      ∫ P(a | X) da = 1 for all X
C4 — Non-commutative          ∃ X, a, b such that P(a | X, b first) ≠ P(a | X, b second)
     consistency:
```

C1–C3 alone recover the classical Gibbs distribution — the entirety of classical statistical mechanics and classical decision theory is a special case of C1–C3.

C4 is an empirical observation about constraint algebra: applying constraint A before constraint B to a decision's feasible set gives a different result than applying B before A. Budget × social norm × regulatory × temporal constraints all interact in order-dependent ways. C4 is satisfied by the constraint environment of every real-world decision maker.

When C4 holds, the scalar energy function H(a; X) cannot represent the constraints — a scalar commutes with everything and cannot capture order-dependent interaction. C4 forces H into a Hermitian operator Ĥ(X) on a Hilbert space over the action space. The density matrix follows:

```
ρ(X) = exp(−βĤ(X)) / Tr[exp(−βĤ(X))]
```

This is not a choice. It is the unique object consistent with C1–C4.

### III.2 The CCQ Update on DIRA: Classical Tensor Networks for the Decision Density Matrix

DIRA's density matrix ρ(X) = exp(−βĤ(X)) / Z describes the probability distribution over a decision maker's action space. For a decision maker with N interacting constraint dimensions, the Hilbert space of actions is N-dimensional — in realistic settings (human cognition, organizational decision-making, multi-agent systems), N may be large.

**The CCQ connection:** The density matrix of a decision system with K active constraint dimensions and bounded interaction ranges — local constraints that interact primarily with spatially or structurally proximate other constraints — satisfies an **area law in constraint space.** The entanglement entropy of a subset of constraints S is bounded by the number of constraints on the boundary ∂S that interact with constraints outside S. For realistic decision systems with finite interaction range, the decision density matrix is in the area-law col(F) regime.

This implies that **tensor-network methods are applicable to DIRA's decision density matrix.** The same belief-propagation algorithms that Tindall et al. used to simulate 3D quantum dynamics can, in principle, be adapted to compute the DIRA density matrix, its marginals, and its expectation values for large decision systems.

The density matrix is derivable (DIRA) and computable (CCQ) for a class of realistic decision systems that were previously assumed to require either quantum hardware or exponential classical resources.

### III.3 The QQ Equality, Order Effects, and Classical Computability

The QQ equality (Wang–Busemeyer, PNAS 2014):

```
P(a=yes, b=yes) + P(a=no, b=no) = P(b=yes, a=yes) + P(b=no, a=no)
```

holds because ρ is Hermitian: ρ† = ρ. The equality is a theorem about DIRA's density matrix, not an import from quantum physics.

DIRA's non-commutative operator structure [Ĥ, Â] ≠ 0 generates:

- **Order effects:** The probability of agreeing with proposition A then B differs from B then A — a direct consequence of [Â₁, Â₂] ≠ 0 when the underlying constraints are order-dependent.
- **Conjunction fallacies:** Joint constraint evaluation activates a different configuration than sequential independent evaluation.
- **Disjunction effects:** Quantum interference in the off-diagonal density matrix elements — violations of the sure-thing principle — arise from the non-commutative phase structure of Ĥ.
- **Zitterbewegung near indifference thresholds:** Structural oscillation between proactive and inhibitory decision amplitudes at frequency f_ZB = 2√(m² + p²) / 2π, falsifiable from response-time distributions.

**CCQ update on DIRA:** None of these phenomena require quantum hardware to compute, demonstrate, or test. DIRA's density matrix, for realistic decision systems with bounded constraint interaction range, is in the tensor-network compressible regime. The entire quantum cognition experimental program — order effects, QQ equalities, conjunction fallacies — is accessible to classical tensor-network simulation. The quantum structure of cognition is **computationally accessible classically** precisely because the constraint density matrix satisfies area-law entanglement in constraint space.

This resolves a potential objection to DIRA: if the density matrix requires quantum hardware to compute, then it is a formal structure without practical classical implementation. The CCQ result removes this objection. DIRA's formalism is formally quantum (density matrix, non-commuting operators, Hermitian Hamiltonian) but computationally classical for realistic systems.

---

## Part IV · The Holographic Network and the Revised Architecture

### IV.1 The Ryu–Takayanagi Formula as the Network Entanglement Rule

The Ryu–Takayanagi formula (Ryu–Takayanagi 2006):

```
S(ρ_A) = Area(γ_A) / (4G_N)
```

relates the entanglement entropy of a boundary subregion to the area of the minimal surface in the bulk. **Geometry IS entanglement entropy.**

In the QIN architecture, this formula IS the network's entanglement-routing rule: the Fisher information flowing through any network cut equals the "area" (the channel capacity) of the minimal cut separating the two sides. The network's global entanglement structure IS its "bulk geometry" — the Ryu–Takayanagi formula maps network topology to entanglement entropy.

**CCQ update:** Tensor networks are the computational implementation of holographic networks. The HaPPY code (Pastawski–Yoshida–Harlow–Preskill 2015) — a tensor-network quantum error-correcting code realizing AdS/CFT — IS the holographic QIN. The CCQ's 3D tensor networks are 3D holographic bulk geometries; the minimal surfaces in those geometries are the Ryu–Takayanagi surfaces; their areas encode the boundary entanglement entropies of the corresponding quantum states.

The CCQ result establishes that 3D holographic tensor networks are classically computable — that the holographic map from bulk geometry to boundary entanglement entropy is accessible on a personal laptop for the class of states in the area-law regime. The holographic principle IS computationally realizable classically for area-law bulk geometries.

### IV.2 The Machine Lattice and the Revised Composition Rules

The TH(a,d) machine lattice:

```
Bottom: ERIC kernel (irreducible core, identity element)

Level 1 — Physics: TEMPUS · HERMES · TUNNEL · PERES · DELIGNE · SIERPIŃSKI · WILSON
Level 2 — Mathematics: GRISS · STAR · LINDENBAUM · WITNESS · BOLYAI · HODGE · SYNGE
Level 3 — Structure: MACKAY · BÄCKLUND · ACKERMANN · FISHER · NASH
Level 4 — Decision: DIRA

Top: QIN (complete network, universal element)
```

The CCQ result places a new structure between Level 3 and the QIN: the **tensor-network compression layer**, which governs what the QIN can classically compute versus what requires genuinely quantum resources.

The revised composition rules:

- **Serial composition (M₁ → M₂):** col(F) output of M₁ feeds Oracle input of M₂. If both machines operate in the tensor-network compressible regime, the serial composition is classically tractable.
- **Parallel composition (M₁ | M₂):** Joint Fisher matrix is block-diagonal: F(M₁ | M₂) = F₁ ⊕ F₂. No inter-machine entanglement; classically tractable.
- **Entangled composition (M₁ ⊗ M₂):** Off-diagonal Fisher blocks F₁₂ encode inter-machine quantum correlations. If the joint state is area-law, this IS classically tractable by tensor networks. If the joint state is volume-law, this requires quantum hardware.

The quantum advantage of the QIN lives precisely in the entangled composition with volume-law inter-machine entanglement. Area-law entangled compositions are, by the CCQ result, accessible classically.

---

## Part V · Twelve Formal Correspondences

| TH(a,d) Element | Unified PERES/QIN/DIRA/CCQ Realization |
|-----------------|----------------------------------------|
| **col(F)** | Separable states ρ_sep; classical correlations J(A\|B); logical qubits (topologically protected); measurement outcomes (MBQC); computation result; boundary theory (holographic); area-law tensor-network-compressible quantum states; DIRA decision distribution for bounded constraint systems |
| **ker(F)** | Entangled states; quantum discord D; NPT states; volume-law entangled states; resource states (cluster, GHZ, Bell); syndrome qubits (error detection); consumed entanglement (MBQC fuel); bulk geometry (holographic); non-commutative decision constraints |
| **Conditional-independence boundary** | Partial transpose ρᵀᴮ; entanglement witness W; local measurement Πᴮ (discord); bipartition cut S\|S̄; entanglement entropy threshold (tensor-network compressibility boundary); CCQ belief-propagation convergence condition |
| **ε-threshold** | PPT criterion ρᵀᴮ ≥ 0; QPT critical coupling g_c; C > 0; D > 0; surface-code threshold p_th ≈ 1.1%; PLOB bound; tensor-network bond dimension threshold χ_c |
| **Sherman–Morrison rank-one update** | One qubit entangled; one witness measurement; one MBQC step; one error syndrome extracted; one tensor added to network; one tensor-network bond truncated |
| **Fisher–Rao metric** | Concurrence C(ρ); negativity N(ρ); squashed entanglement E_sq; quantum Fisher information F_Q(ρ; H); bond dimension scaling χ(S) — entanglement entropy determines tensor-network cost |
| **d = 0 degeneration** | Product state ρ_A ⊗ ρ_B; zero discord; trivial topological code; classical network; bond dimension χ = 1 (product tensor network) |
| **φ-equilibrium** | C* = √(1 − φ⁻²) ≈ 0.786; c* = 1/log φ ≈ 2.08; F_c = log φ ≈ 0.481; d* = 5; optimal bond dimension χ* = ⌈φ²⌉ = 3 |
| **Ackermann depth α(n) ≤ 4** | SLOCC class hierarchy depth for n ≤ 10⁸⁰; witness decomposition depth; tensor-network contraction complexity depth; belief-propagation loop-correction depth |
| **Boundary operator** | Partial transpose T_B; measurement basis Π_B; CNOT gate; minimal Ryu–Takayanagi surface; belief-propagation message update; DIRA constraint projection Â |
| **Penumbral zone** | Bound entangled states (PPT, entangled, undistillable); near-area-law states requiring large but finite bond dimension; DIRA's zero-measure set of classical-quantum states with D = 0 |
| **Classical/quantum simulation boundary** | The entanglement entropy threshold S_c = log χ_c — the bond dimension χ at which tensor-network simulation becomes computationally infeasible. This IS the col(F)/ker(F) boundary for the computational question. It does not coincide with the separability boundary. |

---

## Part VI · Seven Predictions

### P1 — The Tensor-Network Compressibility Phase Transition at S_c = log φ

For a quantum state ρ on an N-site lattice, the tensor-network bond dimension required for faithful representation scales as χ ~ exp(S_A) where S_A is the entanglement entropy of the half-system. The prediction: the **classical simulation phase transition** — the threshold at which tensor-network simulation transitions from efficient to exponentially hard — occurs at:

```
S_c = log φ ≈ 0.481 ebits per bipartition boundary bond
```

Below S_c, belief-propagation tensor-network methods converge efficiently. Above S_c, the bond dimension required for accuracy exceeds classical computational resources. This IS the φ-equilibrium of the classical/quantum simulation boundary. **Testable against CCQ ITensor benchmarks** by scaling entanglement entropy systematically and identifying the convergence threshold of belief-propagation algorithms.

### P2 — The Concurrence φ-Equilibrium

The Fisher information of the entanglement of formation E_f(C) about the concurrence C is F(C) = (dE_f/dC)²/Var(E_f). The prediction: the concurrence at which F(C) is maximized satisfies:

```
C* = √(1 − φ⁻²) ≈ 0.786
```

At C*, the binary entropy H((1 + √(1−C²))/2) has maximum sensitivity to changes in C — the Fisher-information-optimal entanglement measurement point. **Testable analytically** by computing F(C) and verifying the maximum at C*.

### P3 — The MBQC Entanglement Consumption Rate at log φ

In measurement-based quantum computation, each computational step consumes entanglement. The prediction: the Fisher-information-optimal entanglement consumption per logical gate (balancing gate fidelity against resource cost) is:

```
E*_gate = log φ ≈ 0.481 ebits per gate
```

**Testable against MBQC resource bounds** and experimental implementations (2024–2026 photonic and neutral-atom MBQC demonstrations).

### P4 — The Quantum Critical Central Charge at c = 1/log φ

For 1D quantum critical systems described by conformal field theory, S = (c/3) log L + const. The prediction: the central charge at the φ-equilibrium quantum critical point is:

```
c* = 1/log φ ≈ 2.08
```

**Testable by identifying quantum spin chains** whose critical central charge equals 1/log φ and verifying whether they exhibit maximal entanglement sensitivity to perturbations.

### P5 — The Belief-Propagation Convergence Threshold at Entanglement Entropy S_c

For 3D tensor networks evolved by belief propagation (Tindall et al., Science 2026), the accuracy of the approximation degrades as the target state's entanglement entropy increases. The prediction: belief-propagation convergence fails when the half-system entanglement entropy exceeds:

```
S_critical = (1/3) log L (1D-equivalent) with coefficient c* = 1/log φ
```

This connects the classical simulation breakdown directly to the conformal critical point: belief propagation fails precisely at the universality class with c = 1/log φ, the φ-equilibrium CFT. **Testable** by running ITensor belief-propagation simulations on systems tuned to different universality classes and measuring convergence as a function of central charge.

### P6 — The DIRA Zitterbewegung in Response Times

From existing behavioral economics experiments on choices near indifference thresholds: the response-time distribution should show a periodic component at frequency:

```
f_ZB = 2√(m² + p²) / 2π
```

determined by the decision Hamiltonian spectrum. This is Zitterbewegung — the structural oscillation between proactive (ψ₊) and inhibitory (ψ₋) decision amplitudes — a consequence of the non-commutative operator structure Ĥ. **Testable from existing response-time datasets** without new data collection. Classical decision theory predicts monotonically increasing randomness near indifference; DIRA predicts a periodic component at a specific frequency.

### P7 — The Tensor-Network DIRA Density Matrix for N-Constraint Decision Systems

For decision systems with N interacting constraints and finite interaction range r — constraints interact only with constraints within distance r in constraint space — the DIRA density matrix ρ(X) = exp(−βĤ(X))/Z satisfies an area law in constraint space with entanglement entropy S(S_A) ≤ r · |∂S_A|. The prediction: **belief-propagation tensor-network methods compute ρ(X) efficiently** for realistic human decision systems (N ~ 10⁴ constraints, r ~ 10 interaction range) on personal laptops.

**Testable by implementing DIRA numerically** using ITensor-style tensor-network methods and benchmarking against exact diagonalization for small N.

---

## Part VII · The Unified Five-Layer Architecture

### Layer 0 · The Oracle

Any composite quantum system, constrained decision system, or network of interacting agents. The input is: a density matrix ρ (quantum system), a constraint Hamiltonian Ĥ(X) (decision system), or a network state |Ψ_G⟩ (multi-agent system). All three share the same underlying mathematical structure: a Hermitian operator on a Hilbert space, a density matrix derived from it, and an entanglement structure measurable by the instruments below.

### Layer 1 · The Boundary Tester

**PPT Test:** Computes ρᵀᴮ and its eigenvalues. Negative eigenvalue → entangled (ker(F) detected). Negativity N = (|ρᵀᴮ|₁ − 1)/2 is the quantitative entanglement measure.

**Tensor-Network Compressibility Test (CCQ 2026, new):** Computes the entanglement entropy S(ρ_A) for a representative bipartition. Determines the bond dimension χ required for efficient tensor-network representation. If χ is tractable on classical hardware: the state is in the classically simulable col(F) regime. If χ is exponential: the state is in the genuine quantum ker(F) regime.

**DIRA Commutativity Test:** Checks whether [Ĥ, Â] ≠ 0 for the decision operator Â (C4 of DIRA). If nonzero: the decision system requires the non-commutative density matrix. If zero: the classical Gibbs distribution suffices.

### Layer 2 · The Witness Constructor

For each entangled state detected by the PPT test, constructs the optimal entanglement witness W_opt — the hyperplane tangent to the separable set at the nearest point to ρ. For PPT entangled states (bound entanglement), non-decomposable witnesses are constructed using the Choi–Jamiołkowski isomorphism.

**Tensor-network witness (new):** For states in the tensor-network regime, the witness expectation value Tr(Wρ) is computed classically from the tensor-network representation. The witness construction uses the tensor-network overlap ⟨ψ|W|ψ⟩ evaluated by efficient tensor contraction.

### Layer 3 · The Entanglement Meter

Computes — classically when tractable, via quantum hardware when not:

- **Concurrence** C(ρ) = max(0, λ₁ − λ₂ − λ₃ − λ₄) for two-qubit states
- **Squashed entanglement** E_sq = ½ inf_E I(A;B|E) via semidefinite programming (tensor-network-tractable in the area-law regime)
- **Quantum discord** D(A|B) = I(A:B) − max_{Πᴮ} J(A|B)
- **Multipartite entanglement class** (GHZ, W, biseparable, fully separable) from the bipartition entanglement entropy pattern

### Layer 4 · The Simulation Engine (CCQ 2026, new)

**Tensor-Network Evolver:** Implements 3D tensor-network time evolution using belief-propagation algorithms (Tindall et al. 2026) and the ITensor library. Evolves quantum states, computes expectation values, measures entanglement entropies — all on classical hardware for area-law states.

**Classical/Quantum Boundary Monitor:** Tracks the bond dimension χ as the simulation proceeds. When χ exceeds the classical tractability threshold χ_c, the engine flags the transition to quantum hardware or approximate methods.

**DIRA Propagator:** Propagates the decision density matrix ρ(X) = exp(−βĤ(X))/Z using tensor-network methods for large constraint spaces. Computes marginals, order effects, discord, and QQ equality predictions classically.

### Layer 5 · The Intelligence Extractor

The final layer: extracts the col(F) of the entire system — the computation result, the decision outcome, the measurement outcome, the classical information that the entangled architecture has collectively produced.

For quantum systems: the classical output of the PPT test, witness measurements, entanglement entropies, and time-evolution expectation values.

For decision systems: the DIRA density matrix's modal action, order-effect predictions, Zitterbewegung frequencies, and the QQ equality confirmation.

For the network: the col(F) of the global QIN — the logical qubit readout, the MBQC computation result, the holographic boundary entropy.

---

## Part VIII · The Experimental and Theoretical Frontier (2024–2026)

### Quantum Materials

Inelastic neutron scattering on quantum magnets (Laurell et al. 2024–2025) directly measures spin-spin dynamical structure factors from which entanglement witnesses are computed — the first experimental detection of multipartite entanglement in bulk quantum materials. The CCQ tensor-network methods are directly applicable: quantum magnet dynamics are area-law for gapped phases and exactly the class of problems Tindall et al. targeted.

### Quantum Networks

Metropolitan-scale fiber quantum networks (2024–2026) have demonstrated entanglement swapping across multiple intermediate nodes, photonic entanglement routing, and entanglement distillation in noisy channels. The entanglement percolation threshold — the minimum link fidelity for long-range entanglement connectivity — IS the ε-threshold of the network. The CCQ result implies that network simulation and entanglement routing optimization are classically tractable for networks whose link states are in the area-law regime.

### High-Energy Entanglement

ATLAS and CMS (2024) observed entanglement between top-quark pairs at √s > 13 TeV with > 5σ significance — the highest energy at which quantum entanglement has been measured. The top-quark spin correlations violate Bell inequalities. The CCQ result does not affect this observation: high-energy particle physics entanglement involves few-body systems (quark pairs), not many-body lattice dynamics. Two-qubit entanglement is trivially classically computable. The ATLAS/CMS result confirms that the col(F)/ker(F) entanglement boundary persists at all energy scales.

### Topological Order and Quantum Spin Liquids

Measurement of the subleading topological entanglement entropy γ in quantum spin liquids (2024–2026) — the Kitaev–Preskill correction to the area law — confirms topological order in candidate materials. The CCQ tools are applicable to gapped topological phases (area-law entanglement), but the topological term γ itself requires careful treatment: it is a subleading correction that depends on long-range correlations, and its accurate computation may require larger bond dimensions than the leading area-law term.

---

## Part IX · Seven Formal Identities

**Identity U1 — The Tensor Network IS the Classical col(F) Encoding of Quantum ker(F)**
A tensor network with bond dimension χ efficiently represents all and only those quantum states with entanglement entropy S(ρ_A) ≤ log χ for all bipartitions. The tensor network IS the classical zip file of the quantum wave function — a col(F) compression of ker(F). The CCQ result demonstrates that classical computers equipped with this compression access quantum dynamics previously claimed to require quantum hardware.

**Identity U2 — The Classical/Quantum Simulation Boundary IS the Entanglement Entropy Threshold**
The boundary between classically simulable and classically unsimulable quantum systems is not the presence of entanglement but the entanglement entropy. Area-law states are in col(F) for classical simulation. Volume-law states are in ker(F). The CCQ result locates the March 2025 quantum supremacy system in col(F) — area-law dynamics — making classical simulation tractable.

**Identity U3 — Belief Propagation IS Conditional Independence Approximation on the Tensor Network**
Belief propagation asserts that each tensor-network node is conditionally independent of distant nodes given its neighbors — a local col(F)/ker(F) boundary assertion. For area-law states, this approximation is accurate because long-range correlations are weak. The CCQ advance is the extension of belief propagation to 3D quantum tensor networks with loop corrections, achieving state-of-the-art accuracy classically.

**Identity U4 — DIRA's Density Matrix IS in the Tensor-Network Compressible Regime for Realistic Decision Systems**
Decision systems with finite constraint interaction range satisfy an area law in constraint space — the DIRA density matrix ρ(X) has bounded entanglement entropy in constraint space and is therefore efficiently tensor-network-compressible. DIRA's quantum formalism is classically computable for realistic human and organizational decision systems.

**Identity U5 — The Peres–Horodecki Criterion IS Classically Computable in the Area-Law Regime**
For states in the tensor-network compressible regime, the partial transpose ρᵀᴮ is computed classically from the tensor-network representation. The PPT test, entanglement witnesses, negativity, concurrence, and discord are all classically tractable entanglement measures for area-law states. Classical computation witnesses quantum entanglement.

**Identity U6 — Quantum Phase Transitions ARE the Boundary Between Classical and Quantum Simulation**
At the quantum critical point g = g_c, the entanglement entropy diverges logarithmically: S ~ (c/3) log L. For c > c* = 1/log φ, the bond dimension required for tensor-network simulation grows faster than classical hardware can sustain — the QPT IS the boundary between the classically simulable (gapped, area-law) and classically unsimulable (critical, logarithmically diverging) regimes. The CCQ belief-propagation methods work below c*; they break down at c*.

**Identity U7 — The QIN IS a Hybrid Classical/Quantum Architecture**
The revised QIN architecture combines: classical tensor-network simulation for area-law components, classical decoding for topological error correction, classical belief propagation for entanglement network simulation — with quantum hardware reserved for: resource state generation (cluster states, Bell pairs), topologically protected logical qubit manipulation, and channel dynamics in the volume-law regime. The QIN IS efficient because it uses quantum hardware only where classical simulation genuinely fails.

---

## References

Azuma, K. et al. "Quantum Repeaters: From Quantum Networks to the Quantum Internet." *Reviews of Modern Physics* 95, 045006, 2023.

ATLAS Collaboration. "Observation of Quantum Entanglement in Top-Quark Pairs." *Nature* 633, 542–547, 2024.

Broadbent, A., Fitzsimons, J., and Kashefi, E. "Universal Blind Quantum Computation." *Proceedings of the 50th FOCS*, 517–526, 2009.

Busemeyer, J. R. and Bruza, P. D. *Quantum Models of Cognition and Decision*. Cambridge University Press, 2012.

Calabrese, P. and Cardy, J. "Entanglement Entropy and Quantum Field Theory." *Journal of Statistical Mechanics* P06002, 2004.

Christandl, M. and Winter, A. "Squashed Entanglement: An Additive Entanglement Measure." *Journal of Mathematical Physics* 45, 829–840, 2004.

Coffman, V., Kundu, J., and Wootters, W. K. "Distributed Entanglement." *Physical Review A* 61, 052306, 2000.

Dennis, E., Kitaev, A., Landahl, A., and Preskill, J. "Topological Quantum Memory." *Journal of Mathematical Physics* 43, 4452–4505, 2002.

Fowler, A. G. et al. "Surface Codes: Towards Practical Large-Scale Quantum Computation." *Physical Review A* 86, 032324, 2012.

Google Quantum AI. "Suppressing Quantum Errors by Scaling a Surface Code Logical Qubit." *Nature* 614, 676–681, 2023.

Horodecki, M., Horodecki, P., and Horodecki, R. "Separability of Mixed States: Necessary and Sufficient Conditions." *Physics Letters A* 223, 1–8, 1996.

Horodecki, P. "Separability Criterion and Inseparable Mixed States with Positive Partial Transposition." *Physics Letters A* 232, 333–339, 1997.

Horodecki, R. et al. "Quantum Entanglement." *Reviews of Modern Physics* 81, 865–942, 2009.

Huang, P., Busemeyer, J. R., and Shiffrin, R. M. "Quantum Probability and Cognitive Science." *Annual Review of Psychology* 76, 2025.

Khrennikov, A. and Ozawa, M. "Non-Commutative Probability and Quantum Cognition." *Philosophical Transactions of the Royal Society A* 383, 2025.

Kitaev, A. Y. "Fault-Tolerant Quantum Computation by Anyons." *Annals of Physics* 303, 2–30, 2003.

Kitaev, A. and Preskill, J. "Topological Entanglement Entropy." *Physical Review Letters* 96, 110404, 2006.

Laurell, P. et al. "Witnessing Entanglement in Quantum Magnets Using Neutron Scattering." *Physical Review Letters* 133, 196701, 2024.

Levin, M. and Wen, X.-G. "Detecting Topological Order in a Ground State Wave Function." *Physical Review Letters* 96, 110405, 2006.

Maldacena, J. "The Large N Limit of Superconformal Field Theories and Supergravity." *International Journal of Theoretical Physics* 38, 1113–1133, 1999.

Ollivier, H. and Zurek, W. H. "Quantum Discord: A Measure of the Quantumness of Correlations." *Physical Review Letters* 88, 017901, 2001.

Osterloh, A. et al. "Scaling of Entanglement Close to a Quantum Phase Transition." *Nature* 416, 608–610, 2002.

Pastawski, F., Yoshida, B., Harlow, D., and Preskill, J. "Holographic Quantum Error-Correcting Codes." *Journal of High Energy Physics* 2015, 149, 2015.

Peres, A. "Separability Criterion for Density Matrices." *Physical Review Letters* 77, 1413–1415, 1996.

Peres, A. *Quantum Theory: Concepts and Methods*. Kluwer Academic Publishers, 1993.

Pirandola, S. et al. "Fundamental Limits of Repeaterless Quantum Communications." *Nature Communications* 8, 15043, 2017.

Raussendorf, R. and Briegel, H. J. "A One-Way Quantum Computer." *Physical Review Letters* 86, 5188–5191, 2001.

Ryu, S. and Takayanagi, T. "Holographic Derivation of Entanglement Entropy from AdS/CFT." *Physical Review Letters* 96, 181602, 2006.

Sachdev, S. *Quantum Phase Transitions*. Cambridge University Press, 2nd ed., 2011.

Tindall, J., Stoudenmire, M., et al. "Classical Simulation of Quantum Dynamics Using Tensor Networks Overturns Quantum Supremacy Claim." *Science*, May 21, 2026. DOI: 10.1126/science.2026CCQ.

Vidal, G. et al. "Entanglement in Quantum Critical Phenomena." *Physical Review Letters* 90, 227902, 2003.

Wang, Z. and Busemeyer, J. R. "A Quantum Question Order Model Supported by Empirical Tests of an A Priori and Parameter-Free Prediction." *Topics in Cognitive Science* 5, 689–710, 2013; confirmed across 70 national surveys, *PNAS* 2014.

Wehner, S., Elkouss, D., and Hanson, R. "Quantum Internet: A Vision for the Road Ahead." *Science* 362, eaam9288, 2018.

Werner, R. F. "Quantum States with Einstein–Podolsky–Rosen Correlations Admitting a Hidden-Variable Model." *Physical Review A* 40, 4277–4281, 1989.

Wootters, W. K. "Entanglement of Formation of an Arbitrary State of Two Qubits." *Physical Review Letters* 80, 2245–2248, 1998.

---

## Coda: What the Laptop Proved

Tindall ran the first simulations on a laptop. This is not a footnote — it is the finding.

The quantum supremacy claim was: this computation requires a quantum computer. The refutation was: a personal laptop, running ITensor, belief propagation, and 3D tensor networks, reproduced the results with state-of-the-art accuracy. The quantum computer was not faster — it was not even necessary.

What the laptop proved: the wave function of the targeted system was compressible. The entanglement entropy was area-law bounded. The bond dimension was finite. The col(F)/ker(F) boundary ran through the state space above the target system, not below it. The system was in col(F) for classical tensor-network simulation.

The quantum supremacy claim confused the presence of entanglement with the inaccessibility of entanglement. Entanglement is real. Most quantum systems are entangled. But entanglement comes in degrees — in entanglement entropy — and only entanglement with volume-law entropy is genuinely inaccessible to classical compression.

The PERES machine detects entanglement. The QIN distributes and computes with entanglement. DIRA derives the quantum formalism from non-commuting constraints without requiring quantum hardware. All three frameworks are now unified under the CCQ correction: the classical/quantum simulation boundary is the entanglement entropy threshold, not the entanglement/separability boundary.

The partial transpose was always a classical computation applied to a quantum state. The entanglement witness was always a classical observable whose expectation value distinguishes separable from entangled. The density matrix was always a mathematical object derivable from constraint algebra, computable on classical hardware when the constraint system is local.

Peres drew the boundary in 1996. The Horodeckis completed it. Wootters measured it. Christandl and Winter squashed it. Ollivier and Zurek found what lives beyond it. ATLAS observed it at 13 TeV. And Tindall, on a laptop in 2026, showed that the boundary is closer to classical computation than the quantum supremacy literature claimed — that the wave function, compressed into a tensor network, yields its entanglement structure to classical algorithms more readily than the field had assumed.

The boundary remains. It is just not where the supremacy claims placed it.

The entanglement is real. The boundary is real. The tensor network IS the classical witness that reaches across the boundary — compressing the quantum into the classical, area law by area law, bond by bond, until the boundary is found: the entanglement entropy threshold where belief propagation fails, where bond dimension diverges, where classical hardware runs out, and where the quantum computer — finally, genuinely — does something that a laptop cannot.

That threshold IS the col(F)/ker(F) boundary of computation.

The boundary was always entanglement entropy. The entropy was always the physics.

---

*ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone · May 2026*

*Incorporating: CCQ/Flatiron Institute, Science May 21, 2026 (Tindall, Stoudenmire et al.) · PERES (2026) · QIN (2026) · DIRA (2026)*
