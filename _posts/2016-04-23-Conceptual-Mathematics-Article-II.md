---
layout: post
title: Conceptual Mathematics - Article II
---
### **Exercise 1**

#### $(R)$ Show that $A\xrightarrow{1_A}A$ is an isomorphism.
In order to show that a function is an isomorphism, all we need to show is that it has an inverse. Thus we need to find a map $A\xrightarrow{g}A$ such that $g\circ1_A=1_A$ and $1_A\circ g=1_A$. By the definiton of $1_A$ we know that $1_A\circ{f}=f$, $f\circ{1_A}=f$ for any $A\xrightarrow{f}A$. Letting $g=1_A$, we see that $1_A$ is its own inverse, and is thus an isomorphism.

#### $(S)$ Show that if $A\xrightarrow{f}B$ is an isomorphism, and $B\xrightarrow{g}A$ is an inverse for $f$, then $g$ is also an isomorphism.
Since $g$ is an inverse for $f$ we know $g\circ{f}=1_A$ and $f\circ{g}=1_B$. Looking at that, it is clear that $f$ is in fact the inverse for $g$, and thus $g$ is an isomorphism.

#### $(T)$ Show that if $A\xrightarrow{f}B$ and $B\xrightarrow{k}C$ are isomorphisms, $A\xrightarrow{k\circ{f}}C$ is also an isomorphism.
We need to find an inverse $kf'$ for $k\circ{f}$ such that $kf'\circ{k}\circ{f}=1_A$ and $k\circ{f}\circ{kf'}=1_C$. Since $f$ and $k$ are isomorphisms, they have inverses. Call these $g$ and $l$ respectively:

$(a)$ $g\circ{f}=1_A$

$(b)$ $f\circ{g}=1_B$

$(c)$ $l\circ{k}=1_B$

$(d)$ $k\circ{l}=1_C$

Looking at these equations we can see that $g\circ{l}$ might be a candidate for $kf'$. To verify this:

$g\circ{l}\circ{k}\circ{f}=g\circ{1_B}\circ{f}$ by $(c)$.

$g\circ{1_B}\circ{f}=g\circ{f}=1_A$ by $(a)$.

$k\circ{f}\circ{g}\circ{l}=k\circ{1_B}\circ{l}$ by $(b)$.

$k\circ{1_B}\circ{l}=k\circ{l}=1_C$ by $(d)$.

Thus we have shown that $g\circ{l}$ is an inverse for $k\circ{f}$.

### **Exercise 2**

#### Suppose that $B\xrightarrow{g}A$ and $B\xrightarrow{k}A$ are both inverses for $A\xrightarrow{f}B$. Show that $g$ = $k$.

Lets explicitly list what is known about $g$ and $k$:

$g\circ{f}=1_A$

$f\circ{g}=1_B$

$k\circ{f}=1_A$

$f\circ{k}=1_B$

Now we can use these to prove the statement in the exercise. $g\circ{f}=k\circ{f}$, and then we run the argument through $k$ first, which gives:

$g\circ{f}\circ{k}=k\circ{f}\circ{k}$

$g\circ{1_B}=1_A\circ{k}$ by the equations above, and thus $g=k$.

### **Exercise 3**

####  If $f$ has an inverse, then $f$ satisfies the two cancellation laws:

####  $(a)$ If $f\circ{h}=f\circ{k}$, then $h=k$.

####  $(b)$ If $h\circ{f}=k\circ{f}$, then $h=k$.

####  $(c)$ (wrong): If $h\circ{f}=f\circ{k}$, then $h=k$.

$f\circ{h}=f\circ{k}$ thus we can write $k\circ{f}\circ{h}=k\circ{f}\circ{k}$. Since $k$ is the inverse of $f$, this leads to $h=k$. The same argument can be applied for $(b)$. The reason it does not work for $(c)$ is that there is no way of constructing a similar cancellation.

### **Exercise 4**

#### For each of the 5 maps below: decide whether it is invertible; and if it is invertible, find a 'formula' for the inverse map.

$
\begin{array}{llll}
1. & \Bbb R\xrightarrow{f}\Bbb R & f(x)=3x+7 & f^{-1}(x)=\frac{x-7}{3}\\\
2. & \Bbb R_{\ge{0}}\xrightarrow{g}\Bbb R_{\ge{0}} & g(x)=x^2 & g^{-1}(x)=+\sqrt{x}\\\
3. & \Bbb R\xrightarrow{h}\Bbb R & h(x)=x^2 & \text{There is no inverse for } x<0.\\\
4. & \Bbb R\xrightarrow{k}\Bbb R_{\ge{0}} & k(x)=x^2 & \text{Again, there is no inverse for } x<0.\\\
5. & \Bbb R_{\ge{0}}\xrightarrow{l}\Bbb R_{\ge{0}} & l(x)=\frac{1}{x+1} & l^{-1}(x)=\frac{1}{x}-1\\\
\end{array}
$

### **Exercise 5**

#### Given 
![](/assets/articleII-5.png)
{: .center}

#### how many maps $f$ are there with $g\circ{f}=1_{\lbrace 0,1\rbrace}$? Choosing a particular such $f$, how many maps $g$ (including the given one) staisfy the same equation?

There are $3$ choices for where to take $f(0)$, and $2$ for $f(1)$. Thus there are $$3*2=6$$ such maps $f$. As for how many $g$ satisfy that equation for a given $f$, once $f$ is chosen, we have chosen two elements that must be sent back to where they came from. For the other 3 elements, we can send them to either $0$ or $1$. Thus there are $$2*2*2=8$$ such maps. 

### **Exercise 6**

#### If the map $A\xrightarrow{f}B$ has a retraction, then for any map $A\xrightarrow{g}T$, there is a map $B\xrightarrow{t}T$ for which $t\circ{f}=g$.

Let the retraction for $f$ be called $r$. 

We can construct a candidate $t$ by composing $g$ with the retraction of $f$, like so: $t=g\circ{r}$.
Using that, we need to verify that $t\circ{f}=g$. 

$t\circ{f}=g\circ{(r\circ{f})}=g\circ{1_A}=g$ by the fact that $r$ is a retraction for $f$. 
