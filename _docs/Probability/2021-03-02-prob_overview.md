---
layout: default
title: "Overview"
parent: "Probability"
categories: probability theory
nav_order: 1
---
<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

{% katexmm %}

## Concepts

### 1. Random experiment

Studies and experiments are conducted to deal with the uncertainty by estimate the likelihood of a specified event (e.g. two tossings produces two heads).

**Random experiment**. A process (or mechanism) produce definitive but uncertain output (or outcome) (e.g. tossing a coin).

> *Random experiments* are often conducted repeatedly, so that the collective results
> may be subjected to *statistical analysis*.
> A fixed number of repetitions of the same experiment can be thought of as a composed
> experiment, in which case the individual repetitions are called trials. {%cite exp_wiki --file learn_books %}

Some characteristics of a random experiment includes:

- consists of multiple trials (tossing the coin multiple times). Each trial produces one and only one outcome (e.g. head or tail)
- a random experiment has a set of all possible outcomes, called **Sample space**, denoted as $\Omega$ or $S$ (e.g. $\Omega = \{Head, Tail\}$)

***

### 2. Sample space, Event

> The finest-grained list of outcomes for an experiment is the sample space of the experiment {%cite uor --file learn_books.bib%}

**Sample space $(\Omega _{[omega]}$ or $S )$** . A set of all possible outcomes associated with a **Random experiment**. Each **Outcome** is an element of the **Sample space**.

Sample space's cardinality (i.e. size of a set)—represented as $n(A)$—could be 'finite, countably infinite, or noncountably infinite'.

To summary, there are 3 different types of Sample spaces:

| Countability | Cardinality | Discrete/Continuous | Example |
|:------------:|:-----------:|:------------:|:--------|
| Countable    | Finite      | Discrete     |$\{heads, tails\}$ in the simple toss of a coin|
| Countable    | Infinite    | Discrete     |$\{1, 2, 3, ...\}$ describing the possible number of fire alarms in a city during a year|
| Noncountable | Infinite    | Continuous   |$\{0 \leq x \leq 10, 0 \leq y \leq 10\}$, describing the possible locations of required on-the-scene social services in a city 10 by 10 miles square. |

**Events**. A group of zero or more outcomes. All events is a member of $\mathcal{F}$ (`\mathcal{F}`) which is a set of all events.

***

Editing
{: .label .label-yellow }

- [ ] Key operations details
- [ ] Algebraic details

**Algebra of Events:**

<dl>
  <dt>3 key operations</dt>
  <dd>Union</dd>
  <dd>Intersection</dd>
  <dd>Complement</dd>
  <dt>7 algebraic axioms</dt>
  <dd>Commutative law</dd>
  <dd>Associative law</dd>
  <dd>Distributive law</dd>
  <dd>Complement of the complement</dd>
  <dd>Complement of the intersection</dd>
  <dd>Intersection of self-complement</dd>
  <dd>Intersection with the universe of events</dd>
</dl>

***

### 3. Probability

Back to aforementioned statement in the [previous section](#1-random-experiment):

> Studies and experiments are conducted to deal with the uncertainty by estimate the likelihood of a specified event.

So where does the uncertainty in the event occurence come from?

According to {%cite prob_primer --file learn_books %}, there are 3 kinds of source leading to the random behavior in a [classification] system:

1. True random component, e.g., random noise in measurement
2. Random component due to modeling, e.g., systems learn from sampled data
3. Incomplete information, e.g., unknown domain knowledge or knowledge on the phenomena

To address these uncertain elements, we assign a *Probability*—a value between 0 and 1—to an event.

**Probability**. Likelihood of each of the possible events (on a single trial), denoted as a continuous number in range $[0, 1]$. $\mathbf{P}$ is a function mapping from events to probabilities.

***
**Axioms of Probability**:

1. Axiom 1: For any event $A, \mathbf{P}(A)\geq 0$.
2. Axiom 2: $\mathbf{P}(S) = 1$, $S$ is the Sample space
3. Axiom 3: Suppose $A_{1..n}$ are disjoint events: $\mathbf{P}(A_1 \cup A_2 \cup ...) = \mathbf{P}(A_1) + \mathbf{P}(A_2) + ...$

***

{% endkatexmm %}


## References

{% bibliography --file learn_books --cited %}
