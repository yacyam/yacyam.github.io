---
layout: research
title: "Paper: Hierarchical Segments - An Addendum to Active Segments (2025)"
embed: /assets/artifacts/research/HierarchicalSegments.pdf
order: 1
---

Submitted as a final report to CS 4999, co-authored with Professor Robbert van Renesse,
and planning to *eventually* submit this to a conference after cleaning it up.

It is an addendum to [Active Segments](/research/activesegments) that more thoroughly
discusses alternative such as eBPF, and gives a more concrete implementation that
system developers can use to program their memory segments. The details of the
implementation are somewhat shoddy, but the overarching idea is still the same.

This paper will also eventually have an **evaluation** section, which will use a
self-developed python simulation of an operating system that implements the hierarchical 
segment abstraction. [Here is a link to the current simulation](https://github.com/yacyam/Hierarchical-Segments/tree/main/HierarchicalImplementation).

In this simulation, you can currently write your own per-segment page fault and 
unreachable event handlers, and track the page fault and TLB statistics.
The simulation is decently realistic, but requires more improvements such as
multicore and a file system with a unified page cache.

Here is an image of it running with different page fault handlers (one maps regular pages,
another maps mega pages, another uses finite mappings):

<img src="/assets/images/hsegsim.png" style="width:100%; border-radius:8px;">

[Here is a PDF link to the paper](/assets/artifacts/research/HierarchicalSegments.pdf)