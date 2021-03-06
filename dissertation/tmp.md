---
title: "test"
author: Samuel Overington | ID 170431121
numbersections: true
output:
  pdf_document:
    latex_engine: lualatex
    template: assets/template-eisvogel.latex
    path: "../thesis_output/test.pdf"
    toc: true
    toc_depth: 3
header-includes: |
  \usepackage{lmodern,mathrsfs}
  \usepackage{sectsty}
  \usepackage[skipabove=\topskip,skipbelow=\topskip]{mdframed}
  \usepackage{yfonts}
  \usepackage{bbold}
  \usepackage{amssymb}
  \usepackage{amsmath}
  \usepackage{cancel}
  \usepackage[utf8]{inputenc}
  \usepackage{siunitx,physics}
  \usepackage{mattens}
  \usepackage{tensor}
  \usepackage[compat=1.0.0]{tikz-feynman}
  \usepackage{feynmp}
  \input{assets/custom-commands}
---
<!--
  import "assets/custom.md"
-->


# Testing aligning things

$\RR$


test

<!-- /$$ccmanddmb`aV`bS\align}
V/$$n:s/\$\$//ggvS\align -->

\begin{align}
E &= \frac{1}{2} mv^2\\
p &= mv
\end{align}


# Testing my bracket commands
\begin{align}
  &\bsma{a}{m}{b}\\
  &\bsa[c]{a}{b}\\
  &\surround[p_a]{left}{right}\\
  &\bss{\alpha}{\beta}\\
  &\bss[]{\alpha}{\beta}\\
\end{align}
\qquad
\begin{align}
  \bsma{a}{m}{b} \\ %% [a|m|b>
  \bsms{a}{m}{b} \\ %% [a|m|b>
  \bas[c]{a}{b}  \\ %% <acb]
  \bas{a}{b}{c}  \\ %% <ab]c
  \bss[|]{a}{b}  \\ %% [a|b]
  \baa{a}{b}     \\ %% <ab>
  \surround[p_a]{left}{right}\\
  \bss{\alpha}{\beta}\\
  \bss[]{\alpha}{\beta}\\
\end{align}


# Testing `physics`:
\[
  \eval{x}_0^\infty
\]

\begin{align}
  testing
\end{align}

# testing `tensor`:
  when placing a prime mark in `tensor`, you need to put it in the up/down part like so:

\[
\tensor{\bar{\Psi}}{^{\prime}_{\dot{\alpha}}} \tensor{M}{_{\dot{\alpha}}^{\dot{\beta}}} \tensor{\bar{\Psi}}{_\beta}
\]

all good below

\begin{align}
  \tensor{\Psi}{^{\prime}_\alpha} &= \tensor{M}{_\alpha^\beta}\tensor{\Psi}{_\beta}\\
\end{align}

\[
  \tensor{\Psi}{^\prime_\alpha}\\
  \epsilon_{\alpha\beta} \to\\
  \tensor{M}{_\alpha^{\alpha^{\prime}}}\\
  \tensor{M}{_\beta^{\beta^{\prime}}}\\
\epsilon_{\alpha^{\prime} \beta^{\prime}}
\]

\begin{equation}
P^\mu \to \tensor{\Lambda}{^\mu_\nu} p^\nu \equiv p^{\prime \nu}
\end{equation}




# Testing `mdframed` environment
<!-- Defined in `assets/custom.tex`
\mdfdefinestyle{theoremstyle}{%
  linecolor=black,linewidth=2pt,%
  frametitlerule=true,%
  frametitlebackgroundcolor=gray!20,
  innertopmargin=\topskip,innerbottommargin=\topskip,
}
\mdtheorem[style=theoremstyle]{definition}{Definition}
 -->

\begin{definition}
  What is the set of linear transformations that make the metric invariant
\end{definition}

\begin{definition}[Metric]
  There exists a metric such that $\eta \to \Lambda \eta \Lambda = \eta$
\end{definition}

# Testing `Tikz-Feynman` diagrams

\feynmandiagram [horizontal=a to d] {
  a -- [fermion,edge label=$N$] b [dot] -- [double,with arrow=0.5,edge label=$\mathcal{R}$] c -- [fermion,edge label=$N'$] d,
  i -- [charged boson,edge label=$W^i$] b,
  c -- [charged scalar,edge label=$\pi$] o,
};

# Testing abreviated brackets  

\[
  \lthd{i}(z) \equiv  \sabrv{i}{j}\\
  \sabr{\lambda}{i}{\psi}{j}
\]

# Testing Underline:

\begin{align}
  \underline{\agl{i}{\eta}} \udots{$\sqr{\eta}{i}$} \to 0
\end{align}


<!--
  \underline{\agl{i}{\eta}} \udots{$\sqr{\eta}{i}$} \to 0
  \udots{$\agl{j}{\eta}$} \underline{\sqr{\eta}{j}} \to 0\\

  \underline{\agl{i}{\eta}} \dotuline{\sqr{\eta}{i}} \to 0\\
  \dotuline{\agl{j}{\eta}} \underline{\sqr{\eta}{j}} \to 0
-->

# testing cancel

$$
\left \{
\begin{aligned}
  \quad p_i^2(z) &=& \cancelto{0}{p_i^2} +z^2\eta^2 + 2z(p_i \cdot \eta) & = 0\\
  \quad p_j^2(z) &=& \cancelto{0}{p_j^2} +z^2\eta^2 + 2z(p_j \cdot \eta) & = 0
\end{aligned}
\right .
$$

$$
  testing \sA
$$

# ch 1
(@eqfirst) $E = mc^2$

$$
  \L
$$

\begin{equation}
  \label{eq:the_label}
  \gamma = \frac{1}{\sqrt{1-v^2/c^2}}
\end{equation}

# Section 2

$$
\begin{aligned}
  \L = this
\end{aligned}
$$

(@eqsecond) $\vec{a}\cdot\vec{b} = \abs{a}\abs{b}\cos(\theta)$

\begin{equation}
  \label{eq:the2_label}
  \gamma = \frac{1}{\sqrt{1-v^2/c^2}}
\end{equation}

\begin{equation}
  \label{eq:the3_label}
  \gamma = \frac{1}{\sqrt{1-v^2/c^2}}
\end{equation}

<!--
@import "assets/custom.md"
-->
