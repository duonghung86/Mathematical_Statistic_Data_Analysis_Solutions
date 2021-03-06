1.2 Sample space
================

**Experiments** = Situations in which the outcomes occur randomly.

The **sample space** \(\Omega\) corresponding to an experiment is the set of all possible outcomes. An element of \(\Omega\) is denoted by \(\omega\).

An **event** is a subsets of \(\Omega\)

The **union** of two events, A and B, is the event C that either A occurs or B occurs or both occur: \(C = A \cup B\)

The **intersection** of two events, \(C = A \cap B\), is the event that both A and B occur.

The **complement** of an event, \(A^c\), is the event that A does not occur and thus consists of all those elements in the sample space that are not in A.

The **empty set**, \(\emptyset\), is the set with no elements; it is the event with no outcomes.

A and C are said to be **disjoint**, if A and C have no outcomes in common \(A \cup C = \emptyset\)

Commutative Laws:

-   \(A \cup B = B \cup A\)
-   \(A \cap B = B \cap A\)

Associative Laws:

-   \((A \cup B) \cup C = A \cup (B \cup C)\)
-   \((A \cap B) \cap C = A \cap (B \cap C)\)

Distributive Laws:

-   \((A \cup B) \cap C = (A \cap C) \cup (B \cap C)\)
-   \((A \cap B) \cup C = (A \cup C) \cap (B \cup C)\)

1.3 Probability measures
========================

1.  \(P(\Omega)=1\)
2.  If \(A \supset \Omega\), then \(P(A) \ge 0\).
3.  If A1 and A2 are disjoint, then \(P(A1 \cup A2) = P(A1) + P(A2)\)
4.  \(P(A^c) = 1− P(A)\) and \(P(\emptyset) = 0\).
5.  If \(A \subset B\), then \(P(A) \le P(B)\).
6.  *Addition Law* \(P(A \cup B) = P(A)+ P(B)− P(A \cap B)\).

1.4 Computing Probabilities: Counting methods
=============================================

The elements of \(\Omega\) all have \(\underline{\textit{equal probability}}\); so if there are N elements in \(\Omega\), each of them has probability 1/N. If A can occur in any of n mutually exclusive ways, then P(A) = n/N

\(P(A) = \frac{\textit{number of ways A can occur}}{\textit{total number of outcomes}}\)

-   **Multiplication principle**: If one experiment has m outcomes and another experiment has n outcomes, then there are mn possible outcomes for the two experiments.
-   **Extended multiplication principle**: If there are p experiments, and the first has n1 possible outcomes, the second n2, ..., and the pth np possible outcomes, then there are a total of \(n1n2...np\) possible outcomes for the p experiments.
-   A **permutation** is an ordered arrangement of objects.
-   For a set of size \(n\) and \(a\) sample of size \(r\) , there are \(n^r\) different ordered samples \(with replacement\) and \(n(n − 1)(n − 2)...(n − r + 1)=n!\) different ordered samples \(without replacement\).
-   A **combination** is unordered sample
-   The number of unordered samples of r objects selected from n objects without replacement is \(\binom{n}{r}\)
-   The numbers \(\binom{n}{r}\), called the **binomial coefficients**, occur in the expansion

\((a + b)^n = \sum^n_{k=0}\binom{n}{k}a^kb^{n-k}\)

-   In particular, \(2^n=\sum^n_{k=0}\binom{n}{k}\)
-   Suppose that n items are in a lot and a sample of size r is taken. The lot contains k defective items. What is the probability that the sample contains exactly m defectives?

\(P(A) = \frac{\binom{k}{m}\binom{n-k}{r-m}}{\binom{n}{r}}\)

-   The number of ways that \(n\) objects can be grouped into \(r\) classes with \(n_i\) in the \(i^{th}\) class, \(i = 1,..., r\), and \(\sum^r_{i=1}n_i=n\)

\(\binom{n}{n_1n_2...n_r} =\frac{n!}{n_1!n_2!...n_r!} = \textit{multinomial coefficients}\)

**Important examples**:

-   Simpson's Paradox
-   Birthday problems
-   Capture/recapture method

1.5 Conditional Probability
===========================

Let A and B be two events with \(P(B) \ne 0\). The conditional probability of A given B is defined to be

\(P(A | B) = \frac{P(A \cap B)}{P(B)}\)

-   MULTIPLICATION LAW: Let A and B be events and assume \(P(B) \ne 0\). Then \(P(A \cap B) = P(A | B)P(B)\)

-   LAW OF TOTAL PROBABILITY: Let \(B1, B2, ..., Bn\) be such that \(\bigcup^n_{i=1}B_i = \Omega\) and \(Bi \cap Bj = \emptyset\) for \(i \ne j\) , with \(P(B_i) > 0\) for all \(i\) . Then, for any event A,

\(P(A) = \sum^n_{i=1}P(A | B_i )P(B_i )\)

**BAYES' RULE**: Let A and \(B1,.., Bn\) be events where the Bi are disjoint,\(\bigcup^n_{i=1}B_i = \Omega\) and \(P(B_i) > 0\) for all \(i\). Then

\(P(B_j | A) = \frac{P(A | B_j )P(B_j )}{\sum^n_{i=1}P(A | B_i )P(Bi )}\)

1.6 Independence
================

A and B are said to be independent events if \(P(A \cap B) = P(A)P(B)\).

a collection of events, \(A_1, A_2,... , A_n\), to be **mutually independent** if for any subcollection, \(Ai1,... , Aim\) ,

\(P(A_{i_1} \cap ... \cap A_{i_m} ) = P(A_{i_1} ) · · · P(A_{i_m})\)

Special examples - Matching DNA Fragments

1.7 Remarks
===========

One might ask what is meant by the statement “The probability that this coin will land heads up is 1/2 .” Two commonly advocated views are the **frequentist approach** and the **Bayesian approach**.

-   According to the frequentist approach, the statement means that if the experiment were repeated many times, the long-run average number of heads would tend to 1/2 .
-   According to the Bayesian approach, the statement is a quantification of the speaker’s uncertainty about the outcome of the experiment and thus is a personal or subjective notion;
