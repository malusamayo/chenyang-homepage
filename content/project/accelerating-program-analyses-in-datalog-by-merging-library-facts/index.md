---
title: Accelerating Program Analyses in Datalog by Merging Library Facts
date: 2020-10-07T05:55:37.667Z
draft: false
featured: false
external_link: https://cyyang.netlify.app/
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
Static program analysis uses sensitivity to balance between precision and scalability. However, finer sensitivity
does not necessarily lead to more precise results but may reduce scalability. Recently, a number of approaches
have been proposed to finely tune the sensitivity for different program parts. However, these approaches are
usually designed for a specific program analysis, and its abstraction adjustment is not fine enough.


In this paper we propose a new technique, 4DM, to tune abstractions for Datalog analyses. 4DM merges
values in a domain to abstract them, allowing fine-grained sensitivity tuning. 4DM uses a data-driven algorithm
for automatically learning a merging strategy for a library from a training set of programs. Unlike existing
approaches that rely on the properties of a certain analysis, our learning algorithm works for a wide range
of Datalog analyses. We have evaluated our approach on a points-to analysis and a liveness analysis, on the
DaCapo benchmark suite. Our evaluation results suggest that our technique achieves a significant speedup
and negligible precision loss, reaching a good balance.