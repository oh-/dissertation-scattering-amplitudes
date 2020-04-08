<!--
@import "/dissertation/assets/custom.md"
 -->

## Angular Momentum properties:

$$
\begin{aligned}
  \vec{J} &= \vec{x} \times \vec{p}\\
  &= xp_y - yp_x\\
\end{aligned}
$$

Using the a commutator:
$$
\begin{aligned}
  \commutator{J^1}{J^2} &= \commutator{x^2p^3 - x^3p^2}{x^3p^1 - x^1p^3}\\
  &= (x^2p^3 - x^3p^2)(x^3p^1 - x^1p^3) - (x^3p^1 - x^1p^3)(x^2p^3 - x^3p^2)
\end{aligned}
$$

(Only commutator with same index are non-zero)
$$
\begin{aligned}
  \commutator{J_i}{J_i} &= 0\\
  \commutator{J_i}{J_j} &\ne 0\\
\end{aligned}
$$

This leads to the formal relation of angular momentum:

\begin{equation}
  \label{eq:angmomentum_commutator}
  \commutator{J^i}{J^j} = i \hbar J^{ijk} \sigma^k J^k
\end{equation}

This related transformation and sum to Noethers theorem

## Noethers Theorem

\begin{equation}
  \label{eq:noethers_theorem}
  I = \sum_r \pdv{\L}{\dot{q}_r}\delta q_r
\end{equation}


## $SU$ Group:
### $SU(2)$

$$
\begin{aligned}
  SU(2) \to U(N) &= N\times N matrix\\
   &= U^\dagger U = \one \qq{Unitary}
\end{aligned}
$$

$SU(N)$ are a special subset of unitary matrices ($\det U = \pm 1$)

Taylor expansion of $U$:

$$
\begin{aligned}
  U &= e^{iA}\\
  e^x &= 1 + \frac{x^2}{2} + \frac{x^3}{3} \dots
\end{aligned}
$$

Impose the following conditions:
$$
\begin{aligned}
  \det{e^{iA}} = \one \implies \det{M} &= e^{\Tr (\log{M})} \\
   &= e^{\Tr (\log{(\exp(iA) )} ) }\\
   &= e^{\Tr (iA)}\\
   &= e^{i \Tr (A)} \implies \Tr (A) = 0
\end{aligned}
$$

Condition: $U^\dagger U = \one$
Special unitarity: add $\det A = \pm 1 \to SU(N)$

$$
\begin{aligned}
  U &= e^{iA}\\
  A^\dagger &= A \qq{Unitary, hermitian}\\
  \Tr A &= 0
\end{aligned}
$$

This implies we can write:

\begin{equation}
  \label{eq:unitary_group}
  U = e^{i\alpha^a \frac{\sigma^a}{2}}, \quad a = (1,2,3)
\end{equation}

where:
$$
\begin{aligned}
  e^{i\alpha^a \frac{\sigma^a}{2}} = \exp(\sum_{a=1}^3 i\alpha^a \frac{\sigma^a}{2})
\end{aligned}
$$

### Proofs:
$$
\begin{aligned}
  U^dagger U &= \one\\
  (U_1U_2)^\dagger(U_1U_2) &= \one\\
  U^\dagger_2 U^\dagger_1 U_1 U_2 & = \one
\end{aligned}   
$$