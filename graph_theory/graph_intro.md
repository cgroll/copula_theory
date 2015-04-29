---
layout: default
title: Introduction to graph theory
---

# Introduction to graph theory

As R-Vine density decompositions can be described in terms of graph
theoretic concepts, this page summarizes some basic definitions and
theorems required later on. Thereby we try to follow the definitions
of [[Kolaczyk09]](#refs) as closely as possible.

## Graphs

A graph is a combination of **vertices** (**nodes**) and **edges**.
More formally, we define:

### Definition: Edge

For a given set of vertices $$V$$ an edge is defined as a **pair of
distinct vertices** $$\{u,v\}$$, with $$u,v\in V$$.

### Definition: Directed edge

For a given set of vertices $$V$$ a directed edge or **arc** is
an ordered **pair of distinct vertices** $$\{u,v\}$$, where $$u$$ is
called **tail** and $$v$$ is called **head**.


### Definition: Graph

A graph $$G=(V,E)$$ is a tuple consisting of a **set $$V$$ of vertices**
and a **set $$E$$ of edges** associated with $$V$$.

### Definition: Directed graph

A directed graph or **digraph** is a graph $$G=(V,E)$$ where edges
$$e\in E$$ have ordered vertices: $$\{u,v\}\neq \{v,u\}$$.

Based on this general graph definition some more specific
characteristics of graphs can be derived. They are listed in a short
glossary: 

### Graph glossary

- **order**: number of vertices $$N_{v}= \lvert V \rvert$$
- **size**: number of edges $$N_{e}= \lvert E \rvert$$
- **adjacency**: 
  - two vertices $$u,v\in V$$ are called adjacent if $$\{u,v\}\in E$$
  - two edges $$e_{1},e_{2}$$ are called adjacent if they share a
    vertex $$v$$: $$v\in e_{1}$$ and $$v\in e_{2}$$
- **incident**: $$v\in V$$ is incident on $$e\in E$$ if $$v$$ is an
  endpoint of $$e$$
- vertex **degree** $$d_{v}$$: number of edges that share vertex
  $$v\in V$$
- vertex **in-degree**: number of edges pointing to a vertex in a
  directed graph
- **walk**: an alternating sequence
  $$\{v_{0},e_{1},v_{1},e_{2},\ldots,v_{l-1},e_{l},v_{l}\}$$ with
  $$e_{i}=\{v_{i-1},v_{i}\}$$ 
- **path**: walk without repeated vertices
- **cycle**: a walk with distinct vertices except that beginning and
  ending are equal
- **acyclic** graph: a graph without cycles
- **connected** graph: there exists a walk from $$v_{i}$$ to $$v_{j}$$
  for every pair of vertices $$v_{i},v_{j}\in V$$
- vertex **distance**: length of shortest path between two vertices
- walk **length**: 
  - number of vertices within a walk
  - with weighted edges: sum of weights of traversed edges

## Trees

An important special case of graphs is the concept of trees:

### Definition: Tree

A tree is a **connected graph** with **no cycles**.

### Definition: Rooted tree

A rooted tree is a directed tree with in-degree $$d_{v_{i}}^{in}<=1$$
for all $$v_{i}\in V$$, and $$d_{v_{j}}^{in}=0$$ for a single
$$v_{j}\in V$$. $$v_{j}$$ is called **root**.

Again, a short glossary that introduces terms to better describe the
characteristics of a tree:

### Tree glossary
With $$v_{i},v_{j}\in V$$:

- **parent**: for $$v_{i},v_{j}\in V$$, $$v_{i}$$ is called the parent
  of $$v_{j}$$ if there is a directed edge $$e=\{v_{i},v_{j}\}$$
- **children**: $$v_{j}$$ is called a child of $$v_{i}$$ if there is a
  directed edge $$e=\{v_{i},v_{j}\}$$
- **ancestor**: all vertices $$v_{i}$$ traversed on a path from the
  root node to $$v_{j}$$ are called ancestors of $$v_{j}$$
- **descendant**: all vertices $$v_{i}$$ traversed on a path from
  $$v_{j}$$ to a leaf node are called descendants of $$v_{j}$$
- **leaf** node: a vertex $$v$$ without children

# R-Vines: graph theoretic perspective

## Graph theoretic perspectives

An R-Vine can be fully characterized in several ways:

- a set of rooted trees:
  - one conditioning tree per variable
- a set of trees:
  - original vine representation
  - one tree per layer
  - edges become vertices in next layer

## Visualization

Furthermore, it can be perceived and visualized in a number of ways:

- a set of conditioning trees (unique)
- original vine representation (unique)
- a graph of differing complexity: (non-unique representation!)
  - fully connected: all conditional links are shown
  - partly connected: only first layers are shown

References<a name="refs"></a>
---------

<iframe src="../refs/html_refs/graph_intro.html" width="600" height="200"></iframe>
