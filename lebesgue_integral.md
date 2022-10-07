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
