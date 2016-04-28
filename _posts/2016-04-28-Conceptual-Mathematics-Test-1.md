---
layout: post
title: Conceptual Mathematics - Test 1
---

### **Question 1**

#### Throughout this problem $A= \enclose{circle}{\quad \begin{array}{c} &\\\ Mara &\\\ Aurelio &\\\ Andrea &\\\ & \end{array}}$

#### (a) Find an *invertible* map $A\xrightarrow{f}A$, different from the identity map $1_A$. 

Drawing the internal diagram should be pretty straight forward given the descriptions of the map.

$\begin{array}{l} f(Mara)=Aurelio &\\\f(Aurelio)=Andrea &\\\f(Andrea)=Mara \end{array}$

#### (b) Find an *idempotent* map $A\xrightarrow{e}A$, different from the identity map $1_A$.

$\begin{array}{l} f(Mara)=Aurelio &\\\f(Aurelio)=Aurelio &\\\f(Andrea)=Aurelio \end{array}$

#### (c) Find another set $B$ and two maps<br/>$\qquad B\underset{r}{\overset{s}{\rightleftarrows}}A$<br/> for which $r\circ{s}=1_B$ and $s\circ{r}=e$.

$B=\lbrace \beta \rbrace$.

$\begin{array}{l} r(Mara)=\beta &\\\ r(Aurelio)=\beta &\\\ r(Andrea)=\beta\end{array}$

$\begin{array}{l} s(\beta)=Aurelio \end{array}$

### **Question 2**

#### $\Bbb{R}$ is the set of all real numbers, and $\Bbb{R}\xrightarrow{f}\Bbb{R}$ is the map given by the explicit formula $f(x)=4x-7$ for each input $x$. Show that $f$ has an inverse map. To do this, give an explicit formula for the inverse map $g$, and then show that<br/>$\qquad (a) \quad (g\circ{f})(x)=x$, for each real number $x$, and that<br/>$\qquad (b) \quad (f\circ{g})(x)=x$ for each real number $x$.

$g=\frac{x+7}{4}$.

$(g\circ{f})(x)=g(f(x))=g(4x-7)=\frac{(4x-7)+7}{4}=x$.

$(f\circ{g})(x)=f(g(x))=f(\frac{x+7}{4})=4(\frac{x+7}{4})-7=x+7-7=x$.
