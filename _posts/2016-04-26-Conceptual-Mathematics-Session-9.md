---
layout: post
title: Conceptual Mathematics - Session 9
---
These are my solutions to the exercises in [Conceptual Mathematics](http://www.amazon.com/Conceptual-Mathematics-First-Introduction-Categories/dp/052171916X/ref=sr_1_1?ie=UTF8&qid=1461549144&sr=8-1&keywords=conceptual+mathematics). It's a great book.

### **Exercise 1**

#### (In the category of sets) Show that unless the set $A$ has a point and $B$ none, then $A\lhd B$.

If $A$ has no point there are no maps from $A$. If $A$ has a point, $B$ has a point by the problem statement. This means that there is at least one function, call it $f$, that maps every element in $A$ to a single element in $B$.

### **Exercise 2**

#### (In any category) Show that<br/>(R) $A\leq_{R}A$. 

We need to find functions two functions, $s$ and $r$, $A\xrightarrow{s}A\xrightarrow{r}A$, such that $r\circ{s}=1_A$. Simply choose $r=1_A$ and $s=1_A$, clearly $1_A\circ{1_A}=1_A$.

#### (T) If $A\leq_{R}B$ and $B\leq_{R}C$ then $A\leq{R}C$.

Let $r'$ be the retraction of $f$ in $A\leq_{R}B$, $r$ be the retraction of $g$ in $B\leq_{R}C$, and $r''$ be the retraction of $g\circ{f}$ that we want to find: $A\leq_{R}C$.

Now by similar logic to exercise 8 in Article II, we choose $r'' =r'\circ{r}$.

$r'' \circ{g}\circ{f}=r'\circ{r}\circ{g}\circ{f}=r'\circ{f}=1_A$.

### **Exercise 3**

#### (In any category) Suppose that both $A\underset{r}{\overset{s}{\rightleftarrows}}B$ and $A'\underset{r'}{\overset{s'}{\rightleftarrows}}B$ split the same idempotent $B\xrightarrow{e}B$. Use these maps to construct an isomorphism $A\xrightarrow{f}A'$.

Choose $f=r'\circ{s}$ and $g=r\circ{s'}$.

Now we just need to show that these maps when composed result in the two identity maps for $1_A$ and $1_{A'}$.

$f\circ{g}=r'\circ{s}\circ{r}\circ{s'}=r'\circ{1_B}\circ{s'}=r'\circ{s'}=1_{A'}$

$g\circ{f}=r\circ{s'}\circ{r'}\circ{s}=r\circ{1_B}\circ{s}=r\circ{s}=1_A$
