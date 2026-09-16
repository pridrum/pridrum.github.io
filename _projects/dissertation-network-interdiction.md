---
layout: page
title: Dissertation · Collaborating Agents & Network Interdiction
description: How multi-agency collaboration improves labor trafficking interdiction outcomes
importance: 1
category: research
related_publications: true
---

## Overview

My dissertation develops **network interdiction models** to understand and improve how
law enforcement agencies, NGOs, and government entities collaborate to disrupt labor
trafficking in U.S. agricultural supply chains.

**Advisor:** Prof. Kayse Lee Maass, Operations Research & Social Justice Lab, Northeastern University  
**Committee:** Dr. Shahin Shahrampour · Dr. Gabriela Gongora Svartzman  
**Expected completion:** 2026

---

## Motivation

Anti-trafficking organizations rarely operate in isolation — yet the operations research
literature has largely modeled interdiction as a single-agent problem. In practice,
Homeland Security investigators, labor departments, NGOs, and local law enforcement
all play roles in detecting and disrupting labor trafficking, particularly in agriculture
where H-2A guest worker programs create structural vulnerabilities.

What happens when these agencies share information, coordinate interdiction resources,
or divide enforcement territory? When does collaboration help, and when does it create
unintended consequences? These are the central questions of my dissertation.

---

## The four papers

**Paper 1, the scoping review.** _Multiple non-independent interventions on the same network
element._ A PRISMA-ScR review registered on OSF, across four databases with two independent
reviewers. It establishes that independence, or the absence of same-element multiplicity
altogether, is the norm in the literature, which is the gap the rest of the dissertation
addresses.  
_Working paper with K. L. Maass. Revision complete, submitting to Networks, September 2026_

**Paper 2, the model. [Job market paper]** _Collaboration in anti-trafficking efforts: a network
interdiction problem with multiple dependent attacks._ Rather than committing to one algebraic
form for how interventions combine, it defines the class of effect functions satisfying four
axioms and shows the standard independence assumption sits at the boundary of that class, with an
exact linearization and dual bounds. Two results are aimed at a management audience: the cost of
assuming independence, and the coordination gap between a centralized task force and the same
organizations spending the same total separately.  
_Working paper with K. L. Maass. Results analysis. Target: Production and Operations Management_

This paper is the work funded by the **DHS CINA Center of Excellence** project,
[Network Interdiction Models to Improve Effectiveness of Coordinated Labor Trafficking Disruption
Efforts](https://cina.gmu.edu/projects/network-interdiction-models-to-improve-effectiveness-of-coordinated-labor-trafficking-disruption-efforts/),
PI Kayse Maass, Co-PI Amy Farrell.

**Paper 3, theory and complexity.** _Optimal bounds and complexity for network interdiction with
dependent multiple interventions._ Under a logarithmic transform the problem is shortest-path
interdiction and therefore NP-hard. The narrower and more useful claim is that structure discovery
is polynomial and independent of the choice of function, and that the optimal intervention can be
restricted to a candidate set determined by which parts of the network are in play.  
_Working paper with K. L. Maass. Results analysis. Target: Naval Research Logistics or IISE
Transactions_

**Paper 4, the algorithm and computational study.** _Algorithms for network interdiction problems
with non-convex functional attacks._ A three-phase procedure, structure recovery, depth
determination, and budget allocation with re-optimization after each commitment, verified against
exhaustive enumeration on instances small enough to permit it and reported by structural case.  
_Working paper with K. L. Maass. Model and algorithm ready, coding in progress_

---

## Related work

**The empirical companion.** _Network interdiction to improve labor trafficking detection in the
U.S. agricultural sector_, grounded in the H-2A violation data modeled in our PLOS ONE paper
{% cite jafari2024enhancing %}.  
_Revise and resubmit at Decision Sciences. With Jafari, Bhimani, Farrell and Maass_

**Picking up after the degree.** _Unintended consequences of enforcement in labor trafficking
networks: geographic displacement, operational fragmentation, and compliance switching._ How
enforcement that looks optimal for one agency can displace an operation or fragment it rather than
disrupt it.  
_Research in progress with K. L. Maass. Ideation and literature review, resuming after degree
completion_

---

## Methods

- **Network interdiction** (bilevel programming, mixed-integer programming)
- **Multi-agent optimization** (cooperative and non-cooperative settings)
- **Python** with Gurobi for computational experiments
- **Public datasets**: H-2A violation records, DOL enforcement data (500,000+ records)
- Funded by the DHS CINA Center of Excellence, and developed with agricultural labor enforcement practitioners

---

## Selected Presentations

- INFORMS Annual Meeting 2025 — Atlanta, GA _(podium talk)_
- INFORMS Annual Meeting 2024 — Seattle, WA
- INFORMS Annual Meeting 2023
- INFORMS Annual Meeting 2022
- RISE Research Expo, Northeastern University 2024 _(poster)_
- MIE Research Expo, Northeastern University 2023 _(poster)_

---

## Related Publication

{% cite jafari2024enhancing %}
