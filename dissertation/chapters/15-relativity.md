<!-- ## Building a scattering amplitude / Relativity -->
# The Relativity Principle

In order to begin understanding such interactions, we must first understand the
rules by which we can describe an individual particles motion and then build up
a language for how these motions interact in a system of particles.  We open
here by exploring current methods available to us, in the forms of mathematical
formalisms, and how we might use certain properties to expand on this
knowledge, in order to represent systems, or groups of particles, and how they
interact.


## Principle of relativity



<!--
   - Frames of reference
  -->

We will begin by inspecting the systems and rules by which interactions between
free particles can be described, and build our theory from there.  We need to
have a system by which we make measurements , and that measurement will take
the same form, in all other inertial frames of reference. This is the principle
of relativity.

For example, taking a look at two frames of reference (see Figure
\ref{fig:frames_of_ref}); we have two frames \(K, K\prime\) with orthogonal
axes \(\vec{x},\vec{y},\vec{z}\) and
\(\vec{x}\prime,\vec{y}\prime,\vec{z}\prime\).

\begin{figure}
\begin{center}
\begin{tikzpicture}
\def\tick{0.05}
\def\th{205}
 \foreach \x [count = \ra] in {,'}{
    \def\r{\ra};
    \coordinate(O) at (0+\r, 0+\r);
    \coordinate(X) at ((7 + \r, 0 + \r);
    \coordinate(Y) at (\r, 3+\r);
    \coordinate(Z) at ({3 * cos(\th) + \r}, {3 * sin(\th) + \r});
    \draw [thick,->]  (O) -- (X)  node[below]{\small $\vec{x}\x$}; % X
    \draw [thick,->]  (O) -- (Y)  node[above]{\small $\vec{y}\x$}; % Y
    \draw [thick,->]  (O) -- (Z)  node[left ]{\small $\vec{z}\x$}; % Z
    \draw [decorate,decoration={brace,amplitude=7}] (0.2+\r,0+\r) -- (2.2 + \r, 0 + \r) node [midway,above,yshift=7] {\small $\Delta \vec{x\x}$};
    \foreach \z in {0.2, 0.4,  ..., 6.9} {
      \draw (\z+\r, -\tick+\r) -- (\z+\r, \tick+\r);
    }
  }
\end{tikzpicture}
\end{center}
\caption{Two inertial frames of reference, \(K\) and \(K\prime\)}%
\label{fig:frames_of_ref}
\end{figure}




\begin{definition}[Inertial frame of reference]

  A moving body exists in an inertial reference frame, if does not have an
  external force acting upon it, and therefore moves with a constant velocity,
  which might be with a velocity of 0.  Any frame in constant motion with this frame is thus also
  an inertial frame of reference.

  The two inertial reference frames \(K\), and  \(K\prime\) from Figure \ref{fig:frames_of_ref} are related by:

  \begin{equation}
    \Delta \vec{x} = \vec{x}-\vec{x}\prime
  \end{equation}

  where \(\dv{x}{t}=0 \to x\) and \(x\prime\) have same inertial property.

\end{definition}



The equations expressing the laws of nature are invariant with respect to
transformations of coordinates and time from one inertial system to another.
This means that the equation describing any law of nature, when written in
terms of coordinates and time in different inertial reference systems, has one
and the same form. 

The laws of nature are identical in all inertial systems of reference. Experiments show that instantaneous interactions interactions are impossible principle of relativity is valid [See @Landau:1975aa]


In their classical form, the any changes or interactions which happen to a body
in an inertial frame, will happen instantaneously; for example the effects of
a gravitational field, or the electro-magnetic field. Changes to a body within
this frame will be propagated to all other bodies in this or any other inertial
frame instantaneously.

Experiments have shown [For example see @Einstein:1916aa; translation
@Bose:2016aa; @Abbott:2016aa ] that this is not the case, and that in fact the
effects of any such change or interaction must propagate out with a maximum
finite velocity, which we will refer to as the \textit{maximum velocity of
propagation}. This in turn implies that any such behavior of freely moving
bodies within this frame will be limited to the same rules, and therefore must
also have a maximum velocity. This is a universal constant \(c\), the constant
velocity of light in a vacuum:


\begin{equation}
  c =  \SI{299792458}{\m\per\s} \label{eq:c_velocity}
\end{equation}


<!-- c is large numnber, therefore classical approximation c->intfy is good
approximation -->

Due to the fact that this velocity is such a large number, and that in our
every day dealings of velocities, it would be an irregular occurrence for
freely moving bodies to be traveling at such speeds; mostly we are dealing with
velocities where \(v \ll c \).  For such velocities, classical mechanics, or
the Newtonian limit is a fair approximation (where \(c \to \infty \)), and does
not need to take into account any changes needed to account for differences in
the mechanics of interactions, until the velocity of the freely moving body
approaches that order of magnitude i.e. where \(v \approx c\).  Such
differences were introduced in in the \textit{principle of relativity of Einstein} in
1905. Mechanics based on this principle are named \textit{Relativistic}.

Some differences between Classical and Relativistic mechanics:

 - **Space**: the classical definition of distances between points only takes
 on a meaning when we properly specify which from which system we have made
 that reference. Relative 

 - **Time**: in classical mechanics time is an absolute property of the
 universe; and is independent of the frame of reference, as well as the
 coordinate system in which an event is measured,

meaning that two independent events which happen In Re

NOTES:

We now turn our attention towards the question of how to construct a method of
transforming from one set of coordinates to another, 
<!-- UPTO:HERE -->
or one frame of reference

to another.  We need to make a way that we can make a measuremaent and it truly
doesn't matter which frame of reference we were in, or coordinate system we
have used to take this measurement... we need to find a way of keeping this
measurement constant irrespective of the coordinate system or frame from which
we are makeing the measurement.

In classical mechanics, the "distance" betweem two points depend only on the
spatial dinstance between them being kept constant; so a distance in this sense
is purly spatially relative. In relativistic physics, this distance relies on
both spatial and time coordinates being kept constant.



### Spacetime intervals

Event: described by the place where it occurred and times

\begin{equation}
  e_1 = [t,x,y,z]
\end{equation}

### Spacetime transformations



# TOEDIT:

### Transformations

groups of
particles; such that their positions and velocities may be described by
coordinates. Next we must ensure two things:


This is to ensure that the equations describing the laws of physics have the
same form in all admissible frames of reference.

This will ensure that there is no special place in space or time by which
we can make the measurement that will be different from any other. It will also
ensure that distances between points remain unchanged before and after this
transformation. 


 under a closed group of transformations acting on them.

We will also make sure that this system of measurement and
group of transformations remain unchanged when comparing 



as well as in any other system out side of the current system.


classical mechanics, moving between intertial reference frames is relatively
simple becuase of the static nature of time, events int the two reference
frames can be calcuculated  The Galileo Transformation [see @Landau:1975aa] 

#### Relative distances


### Moving Beyond Galilean Mechanics



Using reference systems or co-ordinates.  This fist step will allow us to set a
time and spatial dimensions of the system, and allow us to compare two systems
in relation to one another, and measure the change in this relation as one of
the systems evolves over time in relation to the other.






#### Einsteins dispersion relation

<!-- previously this section was named Interactions -->

At the heart of an interaction between free particles, is the Einsteins
conservative energy and momentum associated with each entering particle to
exiting particles using *De Broglie dispersion relations*, which connects the
energy, momentum, and mass of particles through relativistic dispersion
relation:

\begin{equation}
  \label{eq:einstein_energymomentum}
  E^2 = ( \vec{p} c )^2 + (mc^2 )^2
\end{equation}


currently available to us for exploring interactions from their fundamental
rules in physical systems and building up the language we need in order to
model how they interact. From this, we explore further formalisms which

<!-- TODO:discussion of einstein energy momentum dispersion relation -->

form of relativistic interactions, which themselves have been bootstrapped from
classical mechanics.

setting out the notation for which we will use throughout the duration of this
paper, in order to be able to concisely explain

In order to take into account relativistic effects, we begin here by working
through the formalism of the Lorentz Group to arrive at the relativistic
formalisms for

the a special group called the Lorentz Group,

Let us first take a look at the Lagrangian equation, and how they differ from
their relativistic to non-relativistic formulations.
