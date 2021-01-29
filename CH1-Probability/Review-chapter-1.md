# 1.2 Sample space

**Experiments** = Situations in which the outcomes occur randomly.

The **sample space** *Ω* corresponding to an experiment is the set of
all possible outcomes. An element of *Ω* is denoted by *ω*.

An **event** is a subsets of *Ω*

The **union** of two events, A and B, is the event C that either A
occurs or B occurs or both occur: *C* = *A* ∪ *B*

The **intersection** of two events, *C* = *A* ∩ *B*, is the event that
both A and B occur.

The **complement** of an event, *A*<sup>*c*</sup>, is the event that A
does not occur and thus consists of all those elements in the sample
space that are not in A.

The **empty set**, ∅, is the set with no elements; it is the event with
no outcomes.

A and C are said to be **disjoint**, if A and C have no outcomes in
common *A* ∪ *C* = ∅

Commutative Laws:

-   *A* ∪ *B* = *B* ∪ *A*
-   *A* ∩ *B* = *B* ∩ *A*

Associative Laws:

-   (*A* ∪ *B*) ∪ *C* = *A* ∪ (*B* ∪ *C*)
-   (*A* ∩ *B*) ∩ *C* = *A* ∩ (*B* ∩ *C*)

Distributive Laws:

-   (*A* ∪ *B*) ∩ *C* = (*A* ∩ *C*) ∪ (*B* ∩ *C*)
-   (*A* ∩ *B*) ∪ *C* = (*A* ∪ *C*) ∩ (*B* ∪ *C*)

# 1.3 Probability measures

1.  *P*(*Ω*) = 1
2.  If *A* ⊃ *Ω*, then *P*(*A*) ≥ 0.
3.  If A1 and A2 are disjoint, then
    *P*(*A*1 ∪ *A*2) = *P*(*A*1) + *P*(*A*2)
4.  *P*(*A*<sup>*c*</sup>) = 1 − *P*(*A*) and *P*(∅) = 0.
5.  If *A* ⊂ *B*, then *P*(*A*) ≤ *P*(*B*).
6.  *Addition Law*
    *P*(*A* ∪ *B*) = *P*(*A*) + *P*(*B*) − *P*(*A* ∩ *B*).

# 1.4 Computing Probabilities: Counting methods

The elements of *Ω* all have $\\underline{\\textit{equal probability}}$;
so if there are N elements in *Ω*, each of them has probability 1/N. If
A can occur in any of n mutually exclusive ways, then P(A) = n/N

$$P(A) = \\frac{\\textit{number of ways A can occur}}{\\textit{total number of outcomes}}$$

-   **Multiplication principle**: If one experiment has m outcomes and
    another experiment has n outcomes, then there are mn possible
    outcomes for the two experiments.
-   **Extended multiplication principle**: If there are p experiments,
    and the first has n1 possible outcomes, the second n2, …, and the
    pth np possible outcomes, then there are a total of
    *n*1*n*2...*n**p* possible outcomes for the p experiments.
-   A **permutation** is an ordered arrangement of objects.
-   For a set of size *n* and *a* sample of size *r* , there are
    *n*<sup>*r*</sup> different ordered samples
    *w**i**t**h**r**e**p**l**a**c**e**m**e**n**t* and
    *n*(*n* − 1)(*n* − 2)...(*n* − *r* + 1) = *n*! different ordered
    samples *w**i**t**h**o**u**t**r**e**p**l**a**c**e**m**e**n**t*.
-   A **combination** is unordered sample
-   The number of unordered samples of r objects selected from n objects
    without replacement is $\\binom{n}{r}$
-   The numbers $\\binom{n}{r}$, called the **binomial coefficients**,
    occur in the expansion
    $$(a + b)^n = \\sum^n\_{k=0}\\binom{n}{k}a^kb^{n-k}$$
-   In particular, $2^n=\\sum^n\_{k=0}\\binom{n}{k}$
-   Suppose that n items are in a lot and a sample of size r is taken.
    The lot contains k defective items. What is the probability that the
    sample contains exactly m defectives?
    $$P(A) = \\frac{\\binom{k}{m}\\binom{n-k}{r-m}}{\\binom{n}{r}}$$
-   The number of ways that *n* objects can be grouped into *r* classes
    with *n*<sub>*i*</sub> in the *i*<sup>*t**h*</sup> class,
    *i* = 1, ..., *r*, and $\\sum^r\_{i=1}n\_i=n$
    $$\\binom{n}{n\_1n\_2...n\_r} =\\frac{n!}{n\_1!n\_2!...n\_r!} = \\textit{multinomial coefficients}$$

**Important examples**:

-   Simpson’s Paradox
-   Birthday problems
-   Capture/recapture method

# 1.5 Conditional Probability

Let A and B be two events with *P*(*B*) ≠ 0. The conditional probability
of A given B is defined to be
$$P(A | B) = \\frac{P(A \\cap B)}{P(B)}$$

-   MULTIPLICATION LAW: Let A and B be events and assume *P*(*B*) ≠ 0.
    Then *P*(*A* ∩ *B*) = *P*(*A*|*B*)*P*(*B*)

-   LAW OF TOTAL PROBABILITY: Let *B*1, *B*2, ..., *B**n* be such that
    $\\bigcup^n\_{i=1}B\_i = \\Omega$ and *B**i* ∩ *B**j* = ∅ for
    *i* ≠ *j* , with *P*(*B*<sub>*i*</sub>) &gt; 0 for all *i* . Then,
    for any event A,
    $$P(A) = \\sum^n\_{i=1}P(A | B\_i )P(B\_i )$$

**BAYES’ RULE**: Let A and *B*1, .., *B**n* be events where the Bi are
disjoint,$\\bigcup^n\_{i=1}B\_i = \\Omega$ and
*P*(*B*<sub>*i*</sub>) &gt; 0 for all *i*. Then
$$P(B\_j | A) = \\frac{P(A | B\_j )P(B\_j )}{\\sum^n\_{i=1}P(A | B\_i )P(Bi )}$$

# 1.6 Independence

A and B are said to be independent events if
*P*(*A* ∩ *B*) = *P*(*A*)*P*(*B*).

a collection of events,
*A*<sub>1</sub>, *A*<sub>2</sub>, ..., *A*<sub>*n*</sub>, to be
**mutually independent** if for any subcollection,
*A**i*1, ..., *A**i**m* ,
*P*(*A*<sub>*i*<sub>1</sub></sub> ∩ ... ∩ *A*<sub>*i*<sub>*m*</sub></sub>) = *P*(*A*<sub>*i*<sub>1</sub></sub>) ·  ·  · *P*(*A*<sub>*i*<sub>*m*</sub></sub>)

Special examples - Matching DNA Fragments

# 1.7 Remarks

One might ask what is meant by the statement “The probability that this
coin will land heads up is 1/2 .” Two commonly advocated views are the
**frequentist approach** and the **Bayesian approach**.

-   According to the frequentist approach, the statement means that if
    the experiment were repeated many times, the long-run average number
    of heads would tend to 1/2 .
-   According to the Bayesian approach, the statement is a
    quantification of the speaker’s uncertainty about the outcome of the
    experiment and thus is a personal or subjective notion;
