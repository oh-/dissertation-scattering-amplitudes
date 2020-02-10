---
title: "test"
author: Samuel Overington | ID 170431121
numbersections: true
output:
  pdf_document:
    /* latex_engine: lualatex **/
    template: assets/template.tex
    path: "../thesis_output/test.pdf"
    toc: true
    toc_depth: 3
header-includes: |
  \usepackage{lmodern,mathrsfs}
  \usepackage{sectsty}
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
---

# Testing `Tikz-Feynman` diagrams

\feynmandiagram [horizontal=a to d] {
  a -- [fermion,edge label=$N$] b [dot] -- [double,with arrow=0.5,edge label=$\mathcal{R}$] c -- [fermion,edge label=$N'$] d,
  i -- [charged boson,edge label=$W^i$] b,
  c -- [charged scalar,edge label=$\pi$] o,
};

# Testing abreviated brackets  

$$
  \lthd{i}(z) \equiv  \sabrv{i}{j}\\
  \sabr{\lambda}{i}{\psi}{j}
$$

Testing Underline:
$$
\begin{aligned}
  \underline{\agl{i}{\eta}} \udots{$\sqr{\eta}{i}$} \to 0
\end{aligned}
$$

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