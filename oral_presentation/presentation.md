# General outline

\note{

\begin{itemize}
  \item Aim: To find and produce generators using the 'On-Shell' methods.
  \item A definition of Scattering amplitudes (what they do/ what they are for)
  \item How have they been calculated using Feynman diagrams
  \item Problem with current method of computation (using Feynman diagrams)
  \item difference between On-shell and Off-shell
  \item How do they relate to Gauge theory
  \item Gauge theories and spinor matrices for Gluons and massless particles
\end{itemize}

}

 - Scattering amplitudes
 - Feynman diagrams
 - difference between On-shell and Off-shell
 - Current methods using Gauge theories:
   - BCFW recursion / Yang Mills
   - loop level / tree level recursion
 <!-- - Aim: To find and produce generators using the 'On-Shell' methods. -->
 <!-- - Gauge theories and spinor matrices for Gluons and massless particles -->

# Scattering Amplitudes

\note{
  In Quantum Field Theory (QFT), a scattering amplitude is the mechanism for
  predicting and measuring fundamental particle interactions by mapping the
  energy and momentum associated with each entering particle to exiting
  particles while preserving Einsteins energy-momentum relationship
}

 - Predicting and measuring fundamental particle interactions.
 - Map Energy and momentum.
 - Preserve Einstein Energy momentum relation.

## Einsteins Energy momentum relationship.
$$
  E^2 = ( \vec{p} c )^2 + (mc^2 )^2
$$

## A Feynman Diagram

\centering
\feynmandiagram [horizontal=a to b] {
  i1 [particle=$\hat{1}$] -- [fermion] a -- [fermion]  i2 [particle=$\hat{2}$],
  a -- [photon] b,
  o1 [particle=$\hat{3}$] -- [fermion] b -- [fermion] o2 [particle=$\hat{4}$],
};



# Feynman diagrams

\note{
Traditionally, they have been computed using Feynman diagrams, which set the
boundary conditions to the summed values of all entering particles and those
exiting within the same interaction, such that they conserve this E-M relation
between the entering and exiting particles at the macro level.

The Feynman method makes use of virtual particles, so called because they are
gauge variant or Off-Shell (or off the mass shell) to keep tally of the
energy and momenta of all the paths the particles and interactions make, so
that an individual interaction may temporarily break the energy momentum
relations creating such a virtual particle with negative mass, or energy
@Hodges:2013aa, @Plefka:2014aa. Although it allows for broken symmetries, each
virtual particle must cancel out by the final exiting interaction, ensuring
that the system as a whole is conservative and invariant and we are only left
with On-Shell particles at the boundaries.
}
\centering
\feynmandiagram [horizontal=a to b] {
  i1 [particle=$\hat{1}$] -- [fermion] a -- [fermion]  i2 [particle=$\hat{2}$],
  a -- [photon] b,
  o1 [particle=$\hat{3}$] -- [fermion] b -- [fermion] o2 [particle=$\hat{4}$],
};

## Feynman Diagrams:
 - Set boundary conditions.
 - Energy Momentum Conservation law.
 - Virtual Particles (Off Shell)

# On and Off Shell Particles
\note{
To explain more about on and off shell: Particles are said to be "on the mass
shell," or simply "on-shell," if their behaviour satisfies the relationship
between energy and momentum given by Einstein in his theory of special
relativity. Virtual particles are those that don’t satisfy this relationship,
and are said to be "off-shell.". The diagram is to illustrate the relationship.
In momentum space, this is precisely the equation of a spherical "shell" with radius $\sqrt{mE}$
}

$$
  E^2 = ( \vec{p} c )^2 + (mc^2 )^2 \qq{, "Shell" radius} =  \sqrt{mE}
$$

\begin{figure}

\centering

\begin{tikzpicture}[scale=1.25]%,cap=round,>=latex]
  \coordinate (A) at (0,0);
  \coordinate (B) at (2,0);
  \coordinate (C) at (2,1);
  \draw (A) -- node[below] {$mc^2$} (B) -- node[right] {$pc$} (C) -- node[above] {$E$} (A);
\end{tikzpicture}
\caption{Einstein Energy momentum relationship}
\end{figure}



# On and Off Shell Particles

\note{

If you graph it, you obtain a parabolic surface for massive particles, and a cone for massless particles, like a photon.

This is known as the mass shell, it is quite literally a shell or surface. The momentum of a real particle can be represented as a vector on the surface, hence the expression on shell. Virtual particles do not have these on the surface, hence they are off shell.

The point is that real particles have momentum vectors that are on the shell – not inside it, but on it.  So when two particles (or any other objects) collide, their total momentum has to be preserved. To calculate the momentum in the final state, the momentum vectors from the initial state should be added together. 
 (with natural units this is $E^2 = p^2 + m^2$)

When two massless on-shell particles interact and produce a third particle, The momentum vector of the final particle won’t lie along the surface of the cones.

picture text: Momentum vectors for two colliding particles, (red blue). Momentum in final state given by adding v1 + v2 = v purple.

NB when purple vector is not on the surface of the cone but inside the cone.
}

 - Massless particles produce parabolic surface
 - Massive particles produce a cone shape
 - Real particles momentum vectors along "Shell surface"


\begin{figure}
  \begin{minipage}[b]{.5\linewidth}
    \centering
    \includegraphics[width=5cm]{imgs/perimeter-1-virtual-particle.jpg}%
    \subcaption{Parabolic surface for massive particles\\ Conic surface for massless particles}
  \end{minipage}%
  \begin{minipage}[b]{.5\linewidth}
    \centering
    \includegraphics[width=5cm]{imgs/perimeter2.png}%
    \subcaption{Interaction of two massive particles on the Mass Shell}
  \end{minipage}
  \caption{Source: Perimeter Institute}\label{fig:1}
\end{figure}


# Problem with current method of computation (using Feynman diagrams)
\note{
Each Feynman diagram provides an intuitive way to visualize one possible way
that particles might interact. The trouble is that there are countless other
ways, too.  A quark-quark interaction might produce more than one gluon or
involve more than one virtual-particle loop, or both. The calculations quickly
become unmanageable.

Feynman diagrams are classified by the number of external
lines and the number of closed loops they have. Loops
represent one of the quintessential features of quantum theory: virtual
particles.

Though not directly observable, virtual particles have a measurable
effect on the strength of forces. They obey all the usual laws of nature, such
as the conservation of energy and of momentum, with one caveat: their mass can
differ from that of the corresponding “real” (that is, directly observed)
particles. Loops represent their ephemeral life cycle: they pop into existence,
move a short distance, then vanish again. Their mass determines their life
expectancy: the heavier they are, the shorter they live

So here is an feynman diagram with 2 particles, and the complexity of loops within all possible interactions.

}


\begin{figure}
  \includegraphics[width=.8\linewidth]{imgs/SA-loops1.pdf}%
  \caption{Source: Scientific American}
\end{figure}

# Problem with current method of computation (using Feynman diagrams)

\note{

At very short distances and for very simple collisions, including the distances
relevant for collisions at the LHC, we can get away with
considering only uncomplicated Feynman diagrams

}
Feynman diagrams help visualise one possible way particles interact.
\begin{figure}
  \includegraphics[width=.8\linewidth]{imgs/SA-loops2.pdf}%
  \caption{Source: Scientific American}
\end{figure}

# Problem with current method of computation (using Feynman diagrams)

\note{
For messy collisions, though, the full complexity of the Feynman technique
comes rushing in.
}


\begin{figure}
  \includegraphics[width=.8\linewidth]{imgs/SA-loops3.pdf}%
  \caption{Source: Scientific American}
\end{figure}

# Gauge theories and Spinor matrices for Gluons and massless particles were

## Britto-Cachazo-Feng-Witten (BCFW) approach:
 - Allows us to calculate with ease any tree level amplitude.
 - two gluon into n = 8 gluon, 10,525,9000 contributing Feynman diagrams.
 - Particles have complex momentum.

\centering
\feynmandiagram [horizontal=a to b] {
  i1 [particle=$\hat{1}$] -- [fermion] a -- [fermion]  i2 [particle=$\hat{2}$],
  a -- [photon] b,
  o1 [particle=$\hat{3}$] -- [fermion] b -- [fermion] o2 [particle=$\hat{4}$],
};

\note{
Feynman rules allow one to write down any tree-level amplitude as a sum of all Feynman diagrams contributing.  In practice, this straightforward approach can quickly become cumbersome, as the number of Feynman diagrams typically grows factorially with the number of external legs.

To give an example: for the scattering of two gluons into n gluons the number of contributing Feynman diagrams grows from 4 (n = 2), to 220 (n = 4), to 34,300 (n = 6) to an enormous 10,525,900 for n = 8 [1]
}

# BCFW
\note{
The new approach from Cachazo et al is different.  Two real on-shell particles come enter. Each one produces two more on-shell particles – but these particles have complex momentum, meaning that the number representing their momentum comprises both real and imaginary numbers. 

If drawn on a Feynman diagram, the complex state would be coming out of the plane because we are thinking of the plane as being a real space, not a complex space. 
Below, we see two on-shell particles coming in and producing two complex on-shell particles each, which then merge and produce two more on- shell particles with real momentum.

The key to the BCFW recursion is to study how the amplitude behaves under a complex deformation of the particle momenta preserving the on-shell conditions.
For this we perform the following complex shift of the helicity spinors for two neighboring legs 1 and n
}

\centering
\feynmandiagram [horizontal=a to b] {
  i1 [particle=$\hat{1}$] -- [fermion] a -- [fermion]  i2 [particle=$\hat{2}$],
  a -- [photon] b,
  o1 [particle=$\hat{3}$] -- [fermion] b -- [fermion] o2 [particle=$\hat{4}$],
};

$$
\begin{aligned}
\lambda_1 \to \hat{\lambda}_1(z) &= \lambda_1 - z\lambda_n\\
\tilde{\lambda}_1 \to \hat{\tilde{ \lambda }}_1(z) &= \tilde{ \lambda }_1 - z\tilde{\lambda}_n
\end{aligned}
$$
