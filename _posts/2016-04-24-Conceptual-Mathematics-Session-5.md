---
layout: post
title: Conceptual Mathematics - Session 5
---
### **Exercise 1**

#### (a) Show that if there is a map $g$ for which $h=g\circ{f}$, the for any pair $a_1,a_2$ of points $\Bbb{1}\rightarrow A$ of the domain $A$ of $f$ (and of $h$) we have: <br/> $\qquad$if $fa_1=fa_2$ then $ga_1=ga_2$. <br/> (So, if for some pair of points one has $fa_1=fa_2$ but $ha_1\ne ha_2$, then $h$ is not determined by $f$.)

Since we know that $fa_1=fa_2$ and $ha_1=ha_2$, we can rewrite this as $ha_1=gfa_1=gfa_2=ha_2$.

#### (b) Does the converse hold? That is, if maps (of sets) $f$ and $h$ satisfy the conditions above ('for any pair ... then $ha_1=ha_2$'), must there be a map  $B\xrightarrow{g}C$ with $h=g\circ{f}$.

Yes, we can construct $g$ in such a way that $g(f(a))=h(a)$. We can do this since the domain of $f$ and $g$ is the same, and the size of their ranges is the same due to the conditions satisfied above (they collapse the same number of elements).   

### **Exercise 2**

#### (a) Show that if there is an $f$ with $g\circ{f}=h$, then $h$ and $g$ satisfy: For any $a$ in $A$ there is at least one $b$ in $B$ for which $h(a)=g(b)$.

Choose some $a$. Call $f(a)=b$. Now $g(b)=h(a)$ otherwise $g\circ{f}\ne{h}$.
