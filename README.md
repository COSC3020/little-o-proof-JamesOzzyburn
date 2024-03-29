[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

## Answer
1. $f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < cg(n)$ Definition of $(n)\in o(g(n))$

2. $\forall c \Rightarrow \exists c$ Definition of $\forall c$

3. $f(n) \in O(g(n)) \iff \exists c > 0, \exists n_0 \ge 0: \forall n \ge n_0, f(n) \le cg(n)$ Definition of $f(n)\in O(g(n))$

4. $f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n) \Rightarrow \exists c>0, \exists n_0, \forall n\ge n_0:f(n) \le c g(n)$

Further Elaboration \
When we look at 4 we can see why $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$. There are two reasons for this the first being the changed $\forall c > 0$ in the little o definition to a $\exists c > 0$ in the big O definition. This makes sense as if there is a forall meaning it holds true for all then of course we can find one that is true. The seconds reason being the change from the $<$ in the litte o proof to the $\le$ in the big o. It has kinda the same resoning as the previous point being that of course something that is less than is also less then or equal to. $(f(n) < cg(n) \Rightarrow f(n) \le cg(n))$
