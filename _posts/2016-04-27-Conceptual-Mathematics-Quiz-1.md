---
layout: post
title: Conceptual Mathematics - Quiz I 
---
These are my solutions to the exercises in [Conceptual Mathematics](http://www.amazon.com/Conceptual-Mathematics-First-Introduction-Categories/dp/052171916X/ref=sr_1_1?ie=UTF8&qid=1461549144&sr=8-1&keywords=conceptual+mathematics). It's a great book.

### **Question 1**

#### Give an example of two explicit sets $A$ and $B$ and an explicit map $A\xrightarrow{f}B$ satisfying *both*:<br/>$\qquad$(a) there is a retraction for $f$, *and*<br/>$\qquad$(b) there is *no* section for $f$.<br/>Then explain how you know that $f$ satisfies (a) and (b).

Imagine $A=\lbrace a_1 \rbrace$ and $B=\lbrace b_1,b_2 \rbrace$. Let $f(a_1)=b_1$. This clearly has a retraction $r$ that maps both $b_1,b_2$ to $a_1$. However, there is no section $s$ where $f\circ{s}=1_B$, there simply cannot be since $ \lvert A \rvert  < \lvert  B \rvert$.

### **Question 2** 

#### If $C\underset{q}{\overset{p}{\rightleftarrows}}D$ satisfy $p\circ{q}\circ{p}=p$, can you conclude that<br/>$\qquad$(a)$p\circ{q} is idempotent? If so, how?

We know $pqp=p$. $pqpq=(pqp)q=pq$, Thus $pq$ is idempotent.

#### $\qquad$(b)$q\circ{p}$ is idempotent? If so, how? 

By the same logic as in (a), $qpqp=q(pqp)=qp$. 

### **Question 2\***

#### If $C\underset{q}{\overset{p}{\rightleftarrows}}D$ satisfy $p\circ{q}\circ{p}=p$, use the given maps $p$ and $q$ to devise a map $q'$ satisfying *both*:<br/>$\qquad p\circ{q'}\circ{p}=p$<br/>*and*<br/>$\qquad q'\circ{p}\circ{q'}=q'$<br/>(and explain how you know that your $q'$ has these properties.)

Let $q'=qpq$. 

$pq'p=(pqpq)p=pqp=p$ by the problem statement.

$q'pq'=(qpq)p(qpq)=(qpqp)(qpq)=qp(qpq)=(qpqp)q=qpq=q'$ where we used the solution from Question 2 (b).

### **Question 1\***

#### same question as Problem 1 at top of page, except that both sets $A$ and $B$ are required to be *infinite* sets.

Let $A=\Bbb{Z}$ and $B=\Bbb{R}$.

Now let $f(a)=a$.

It is easy to see how a retraction for $f$ would be constructed by mapping $x.0$ to $x$, and everything else to $0$. Since $\Bbb{R}$ is larger than $\Bbb{Z}$ (even though they are both infinite), there can be no section for $f$.  

