# Code and Erratum for *On the asymptotic category*

I collected a bit of Magma code relevant for the paper *Idempotents, traces, and dimensions in Hecke categories* <a href="https://arxiv.org/abs/2507.10061">https://arxiv.org/abs/2507.10061</a> and *Computing in the asymptotic category*
NOT YET AVAILABLE on this page.

The code is in a **.odt** file or **.n** file, respectively, that can be downloaded from this site and you can run it with Magma.

An Erratum for these papers can be found at the bottom of the page.

# Contact

If you find any errors in any of these two papers **please email me**:

[dtubbenhauer@gmail.com](mailto:dtubbenhauer@gmail.com?subject=[GitHub]%web-reps)

Same goes for any errors related to this page.


# Background

These two tandem papers study the **asymptotic (Hecke) category** A(H) attached to a diagonal H-cell H in a finite Coxeter type. Informally: start with the (diagrammatic) Hecke category, restrict to a cell, and then pass to an “asymptotic” quotient where only the leading cell-behavior remains. The outcome is a rigid, semisimple, tensor category. So, in practice, a fusion category, whose structure reflects subtle cell combinatorics.

The first paper (*Idempotents, traces, and dimensions in Hecke categories*) develops the computational toolkit:
- computing **primitive idempotents** projecting to indecomposable objects,
- computing **partial traces**, and from them
- **categorical dimensions** in A(H),
in a way that is designed to be implemented on a computer.

The second paper (*Computing in the asymptotic category*) applies this technology to identify A(H) in finite types, with only a small number of remaining cases (concentrated in type H4). A key idea throughout is that categorical dimensions are a strong invariant: they sharply constrain (and often uniquely determine) which fusion category A(H) can be.

Concretely, the outcome is:
- In **classical types** (A,B,C,D), A(H) is the expected pointed fusion category, namely Vec(G) for an elementary abelian 2-group G.
- In the **exceptional types**, we list explicit predictions and verifications case-by-case, and the Magma code below is meant to reproduce the relevant dimension/idempotent computations.

(For reference on finite Coxeter types, see the standard classification list, e.g. <a href="https://en.wikipedia.org/wiki/Coxeter_group#Classification">https://en.wikipedia.org/wiki/Coxeter_group#Classification</a>.)

# The Magma code

The Magma code can be downloaded on this page. Its called **idempotent_tests.m**. To run it:

- First, setup Joel Gibson's ASLoc which can be found here <a href="https://github.com/joelgibson/asloc">https://github.com/joelgibson/asloc</a>.

- Then you can start the file in your ASLoc folder.

- As soon as its started run one of the procedures listed below. The output will be of the form:

![Output](https://github.com/dtubbenhauer/acat/blob/main/g2.png)

The available procedures are:

```
B2_complete()
G2_complete()
H3_a1_complete()
H3_a3_complete()
H3_long_complete()
H4_complete()
H4_middle_1()
H4_middle_9()
H4_middle_19()
```

**Small warning**: Some of these run for quite some time.

# Erratum

Empty so far.

