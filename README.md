# General-Matrix-Decomposition
We explore the utilization of higher-order discretization techniques in optimizing the gate count needed for quantum computer based solutions of partial differential equations. To accomplish this, we present an efficient approach for decomposing $d$-band diagonal matrices into Pauli strings that are grouped into mutually commuting sets.

Using numerical simulations of the one-dimensional wave equation, we show that higher-order methods can reduce the number of qubits necessary for discretization, similar to the classical case, although they do not decrease the number of Trotter steps needed to preserve solution accuracy. This result has important consequences for the practical application of quantum algorithms based on Hamiltonian evolution.

Figure 2 is comparison of $\vec{\phi}_V (t)$ - solution obtained as $e^{-i H_k t} \vec{\psi} (t=0)$ with $\vec{u} (t) = \vec{u}_s(t)/||\vec{u_0}||$ an analytical standing wave solution at $t=1$, with $l=5$ and $c=1$ for different accuracy orders $\kappa=2k$ and different number of qubits for discretization $n$ (the total number of qubits is given by $n+1$).

Figure 3 is comparison of $\vec{\phi}_V (t)$ - solution obtained with proposed quantum algorithm with $\vec{u} (t) = \vec{u_s}_s(t)/||\vec{u_0}||$ with fixed Trotter errors of $10^{-3}$, $10^{-5}$, and $10^{-7}$, represented by different marker shapes.  Results for $4$ and $5$ qubits are given with red and green respectively (the total number of qubits is given by $n+1$). The Trotter formula is set to order $p=2$; the wave equation parameters $l=5$, $t=1$, and $c=1$.

Figure 4 is the relationship between the number of Trotter steps $r$ and the number of qubits for a discretization $n$ (total qubits $n+1$), using various discretization orders $\kappa$, necessary to reach an error of $\epsilon_{\text{ns}} = 10^{-5}$. The Trotter formula is utilized at order $p=2$, with wave equation parameters set to $l=5$, $t=1$, and $c=1$.
