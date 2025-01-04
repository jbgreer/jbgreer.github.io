+++
title = 'CPS'
date = 2025-01-04T16:55:14-06:00
draft = false
+++

## Continuation-passing Style

[Into CPS, never to return](https://bernsteinbear.com/blog/cps/)

CPS, or continuation-passing style, is an intermediate representation for programs,
particularly functional programs. It’s used in compilers for languages such as SML and Scheme.
Much of its utility comes from its support for tail calls and nonlocal control flow such as
call/cc, but it can also be used as an optimization target just as SSA, or static single
assignment, often is.

In CPS, there are two rules: first, that function/operator arguments must always be trivial;
second, that function calls do not return. From this, a lot falls out.

In this post, we’ll introduce CPS by building a simple (Plotkin1) CPS transform from a small
Scheme-like language. We’ll sketch some optimizations on the IR. Then we’ll look at a couple of
the common ways to actually compile the IR for execution.

### Source

[Max Bernstein blog](https://bernsteinbear.com)
