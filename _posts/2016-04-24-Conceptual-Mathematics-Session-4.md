---
layout: post
title: Conceptual Mathematics - Session 4
---
### **Exercise 1**

#### Finish checking that $d$ is an isomorphism in our category by showing that $h\circ{d}$ and $d\circ{h}$ are indeed identity maps.

$h\circ{d}(x)=h(2x)=\frac{1}{2}(2x)=x$.

$d\circ{h}(x)=d(\frac{x}{2})=2(\frac{x}{2})=x$.

### **Exercise 2**

#### Find an isomorphism $(\lbrace odd, even \rbrace,+)\xrightarrow{f}(\lbrace positive,negative \rbrace,\times)$.

$
\begin{array}{lcl}
&f&\\\
odd & \rightarrow & negative\\\
even & \rightarrow & positive\\\
\end{array}
$

Now we need to check the "combining rules:"

$f(odd + odd)=f(odd)\times f(odd)=negative\times negative = positive = f(even)$. 
$f(even + even)=f(even)\times f(even)=positive\times positive = positive = f(even)$. 
$f(even + odd)=f(even)\times f(odd)=positive\times negative = negative = f(odd)$. 

### **Exercise 3**

#### An unscrupulous importer has sold to the algebraic category section of our zoo some creatures which are *not* isomorphisms. Unmask the imposters$$\\\ (a)\space(\Bbb{R},+)\xrightarrow{p}(\Bbb{R})\space\text{by 'plus 1': } p\space x = x+1.\\\ (b)\space(\Bbb{R},\times)\xrightarrow{sq}(\Bbb{R},\times)\space\text{by 'squaring': } sq\space x = x^2. \\\ (c)\space(\Bbb{R},\times)\xrightarrow{sq}(\Bbb{R}_{\ge{0}},\times)\space\text{by 'squaring': } sq\space x = x^2. \\\ (d)\space(\Bbb{R},+)\xrightarrow{m}(\Bbb{R},+)\space\text{by 'minus': } m\space x = -x. \\\ (e)\space(\Bbb{R},\times)\xrightarrow{m}(\Bbb{R},\times)\space\text{by 'minus': } m\space x = -x.\\\ (f)\space(\Bbb{R},\times)\xrightarrow{c}(\Bbb{R}_{\gt{0}},\times)\space\text{by 'cubing': } c\space x = x^3$$.

$
\begin{array}{ll}
(a)&\text{This is }\textbf{not}\text{ an isomorphism in our category, } (a+b)+1 \ne (a+1)+(b+1) \\\
(b)&\text{This map 'loses' information, and does }\textbf{not}\text{ have an inverse.} \\\
(c)&\text{For similar reasons, this map is }\textbf{not}\text{ an isomorphism.} \\\
(d)&(-a)+(-b)=-(a+b)=-a-b\implies \text{This }\textbf{is}\text{ an isomorphism.} \\\
(e)&-(ab)\ne (-a)(-b)\text{ This is }\textbf{not}\text{ an isomorphism.} \\\
(f)&\text{This }\textbf{isn't}\text{ a map with the given domain and codomain.} \\\
\end{array}
$
