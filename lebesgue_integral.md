# Explaining Measure Theory

## Introduction : what is wrong with current teaching of measure theory (and probably a lot of other mathematical stuff)

A lot of measure theory courses are beginning with "lol let's define a $\sigma\text{-algebra}$" without really justifying why all thoses theorems are useful
(see e.g. https://www.imo.universite-paris-saclay.fr/~jflegall/IPPA2.pdf). The aim here is to fill this conceptual gap.

Some vulgarization work has already be done. See e.g. https://www.youtube.com/watch?v=LDNDTOVnKJk. But still, it lacks a exhaustive and rigorous link between its
contents and the tools developed in the  $\sigma\text{-algebra}$ like courses. To understand what I mean, let me take an example : in the previously mentioned course,
the **monotonous class lemma** is introduced. But nowhere, neither in this course, nor in the video mentioned above, is it explicitely justified why this lemma really
interesting and crucial is. 

Actually, a partial answer is available in the course. Given two "measures" (functions with special rules detailed below) $u$ and $v$ defined on a space $E$
($E$ also having special rules), we want to know the form of the smallest set of "slices" of $E$ where, if on each slice, $u(\text{slice})$ = $v(\text{slice})$, then
$u$ = $v$. The amount and the properties of the set of slices is, in the course, progressively decreased to its minimum, and the monotonous class lemma is the last piece
of the puzzle, used to give the "real" minimal amount of slices. 

But, in my opinion, this problem should be exposed and developed in the introduction and each of the hypothesis developed in the courses should be contextualized as a
way to answer this question.

You can find some answer drafts when you enter something like "why are sigma-algebra useful" in your favorite search engine. But for now, the best resource I found describing the whys is this course from Terence Tao (https://terrytao.files.wordpress.com/2012/12/gsm-126-tao5-measure-book.pdf), that has a real introduction and contextualization. Nevertheless, after reading the introduction, I still had unanswered questions. 

## TODO : 1) Why is measure useful ? Example of hybrid laws !

## TODO : 1) bis (from T. Tao) 


## TODO : 2) What kind of problems do you encounters when you want to define what is a measure (example of Vitali's set, which is not measurable) ?

The main problem of the previous definition/example is that not every set can be measured. Otherwise, one would not need the sigma-algebra. Let us try to define such
an unmeasurable set. Let us suppose $\mathbb{R}$, and the Lebesgue measure $\mu$ associated $\mu([a, b]) = b - a$. The aim here is to find a list of sets $V_k$ that are dense enough to have a strictly positive measure, but sufficiently sparse so that $(V_k)_{k \in \mathbb{N}}$  is a partition of $[0,1]$

Let us define such a set : $V$ containing some elements, so that for each $r \in [0, 1]$, there is one and only one $v \in V$ so that $v + r \in \mathbb{Q}$.

It is even possible to build such a set ? Yes, using the axiom of choice. # TODO

Let then define $V_k = V + q_k$, for each $q_k \in [-1, 1]$. Each $V_k$ are of the same "size", so their measures should be identical. Plus, $[0, 1] \subseteq \cup{V_k}$. Actually, if $r \in [0, 1]$, it exists $v \in V$, so that $v + r = q$. It exists a $k$ where $q = q_k$ So, $r \in V_k$.

So $1 \le \cup{\mu(V_k)}$, and $\mu(V) > 0$. But $\cup{V_k} \in [-1,2]$ so that $\mu(V) = 0$, contradiction !

## TODO : 3) Why does sigma-algebra solves this problem.

What does it implies ? Actually, in the "standard" measure theory, that you need to check wether a set is measurable before talking about its measure. That is why, along with the space of elements your set may be composed of. you have to define the list of every actually measurable set.

## TODO : 4) Back to lebesgue integral : why useful ? Example of irrationnal numbers, maybe example of convergence.
