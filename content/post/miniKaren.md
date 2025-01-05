+++
title = 'MiniKaren'
date = 2025-01-04T20:53:06-06:00
draft = false
+++

## [Relational Programming in miniKaren](https://github.com/webyrd/dissertation-single-spaced/blob/master/thesis.pdf)

The promise of logic programming is that programs can be written relationally,
without distinguishing between input and output arguments. Relational programs
are remarkably flexible—for example, a relational type-inferencer also performs type
checking and type inhabitation, while a relational theorem prover generates theo-
rems as well as proofs and can even be used as a simple proof assistant.
Unfortunately, writing relational programs is difficult, and requires many inter-
esting and unusual tools and techniques. For example, a relational interpreter for
a subset of Scheme might use nominal unification to support variable binding and
scope, Constraint Logic Programming over Finite Domains (CLP(FD)) to imple-
ment relational arithmetic, and tabling to improve termination behavior.
In this dissertation I present miniKanren, a family of languages specifically de-
signed for relational programming, and which supports a variety of relational idioms
and techniques. I show how miniKanren can be used to write interesting relational
programs, including an extremely flexible lean tableau theorem prover and a novel
constraint-free binary arithmetic system with strong termination guarantees. I also
present interesting and practical techniques used to implement miniKanren, includ-
ing a nominal unifier that uses triangular rather than idempotent substitutions and
a novel “walk”-based algorithm for variable lookup in triangular substitutions.
The result of this research is a family of languages that supports a variety of
relational idioms and techniques, making it feasible and useful to write interesting
programs as relations.

### Source

[William E. Byrd website](http://webyrd.net/)
