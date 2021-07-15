---
layout: default
title: "Probability Basic"
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

## Random experiment

### Concept

**Random experiment**. A process (or mechanism) produce definitive but uncertain output (or outcome) (e.g. tossing a coin).

> *Random experiments* are often conducted repeatedly, so that the collective results
> may be subjected to *statistical analysis*.
> A fixed number of repetitions of the same experiment can be thought of as a composed
> experiment, in which case the individual repetitions are called trials. {%cite exp_wiki --file learn_books %}

Some characteristics of a random experiment includes:

- consists of multiple trials (tossing the coin multiple times). Each trial could produce a different outcome (e.g. head or tail)
- a random experiment has a set of all possible outcomes which is called **Sample space** (e.g. $\Omega = \{Head, Tail\}$)

**Sample space $(\Omega _{[omega]}$ or $S )$** . A set of all possible outcomes associated with a **Random experiment**.

**Events**. A group of outcomes. All events is a member of $\mathcal{F}$ (`\mathcal{F}`) which is a set of all events.

Studies and experiments are conducted to deal with the uncertainty by estimate the likelihood of a specified event (e.g. two tossings produces two heads)

**Probability**. Likelihood of each of the possible events, denoted as a continuous number in range $[0, 1]$. $P$ is a function mapping from events to probabilities.


{% endkatexmm %}


## References

{% bibliography --file learn_books --cited %}
