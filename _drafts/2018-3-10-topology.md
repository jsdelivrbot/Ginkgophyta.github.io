---
layout: mathpost
title: "Real Numbers"
categories: math 
comments: True

---

Self-studying real analysis requires rigor that I don't seem to have. The definitions in analysis always felt elusive and unintuitive. To make my life easier, I collected the definitions that I believe are quite important: 

### Function sets
* Domain: is what goes into a function. Given a function $$f$$ such that 

    $$ f: \mathbb{R} \to \mathbb{N}$$

    then domain is the set of real numbers, $$\mathbb{R}$$

* Codomain: is what can possibly come out of a function. In function $$f$$ shown above, a codomain is a set of natural numbers, $$\mathbb{N}$$. 

* Image(or range): is a subset of a codomain that actually gets mapped from the element in the domain:

$$ R = \{y \in Y | \exists x \in X\ such\ that\ f(x) = y\} $$

### Function properties
* Injection(or one-to-one): or injective function is a function where each element in the image of the function maps to a unique element in the domain. In other words, no two elements in the domain maps to the same element in the codomain. A more rigorous mathematical expression is:

    $$ \forall a,b \in X, f(a) = f(b) \implies a = b$$

    or the contrapostive is 

$$ \forall a,b \in X, a \neq b \implies f(a) \neq f(b)$$

* Surjection(or onto): or surjective function is a function where for every element $$y$$ in the codomain, there is at least one element $$x$$ in domain $$X$$ such that $$f(x) = y$$. A mathematical notation would be:

$$ \forall y \in Y,\ \exists x \in X,\ f(x)=y$$

* Bijection(or one-to-one correspondence): or bijective function is a function that, as the name suggests, has a one-to-one correspondence. This one-to-one correspondence means that the function is both injective and surjective.

### Finite and countably/uncountably infinite sets

* Finite set: is a set that has one-to-one correspondence with $$ \{1, 2, \dots, n\}$$ for some $$ n \in \mathbb{N}$$. (Note, ane empty set is a finite set).

* Infinite set: is a set that is not finite. So if finite set is denoted as $$A$$, then infinite set is the complement of that set which is $$A^c$$. 

* Countably infinite set: is a set that has one-to-one correspondence with the set of natural numbers $$\mathbb{N}$$. Natural numbers, as the name suggests, implies a notion of countability because these numbers are natural, or God-given. So if a set can be mapped one-to-one correspondence with natural numbers, we deem that set to be countable. 

* Uncountably infinite set: is a set that is not countable. In other words, it does not have a one-to-one correspondence with natural numbers.

### Distance and Convergence

* Distance: is a function on some set $$\Omega$$ such that 

    $$ d: M \times M \to \mathbb{R}$$

    where $$M$$ is some set and $$d$$ is a metric(or distance) on set $$M$$. For function $$d$$ to be a metric function, $$\forall x,y,z \in M$$, the following must hold:
    
    * Nonnegativity: 
        
        $$d(x,y) > 0, d(x,y)=0 \longleftrightarrow x=y$$

    * Symmetry:
    
        $$ d(x,y) = d(y,x)$$

    * Triangle inequality:
    
        $$ d(x,z) \le d(x,y) + d(y,z) $$

Regardless of what function $$d$$ is, if $$d$$ satisfies those properties, then it is a metric function. 

* Convergence: is a notion where on any metric space, if there exists a sequence $$x_1, x_2, \dots $$ in set $$\Omega$$, we say the sequence converges to $$x$$ if $$d(x_n, x) \to 0$$ as $$n \to \infty$$. Mathematically, we can write this as

    $$ \lim_{n \to \infty} d(x_n, x) = 0$$
    
    A more mathematically sound definition is:

    $$ (\forall \epsilon > 0)(\exists N)(\forall n \ge N)(d(x_n, x) < \epsilon) $$

    This says for any positive number $$\epsilon$$, there exists a point $$N$$ in the sequence such that the distance between (1) point $$N$$ and all the points after point $$N$$ and (2) the point $$x$$ is less than $$\epsilon$$. 

* Divergence: is when a sequence does not converge. The definition is the negation of the convergence definition which is 

    $$ (\exists \epsilon > 0)(\forall N)(\exists n \ge N)(d(x_n, x) \ge \epsilon)$$

    This means that there is at least one point among points that come after point $n$ that has a distance to $$x$$ greater than $$\epsilon$$.


