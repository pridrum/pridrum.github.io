---
layout: page
permalink: /teaching/busing-case/
title: the busing case
description: A school closing, a linear program, and the questions I ask before students formulate anything
nav: false
---

A district closes a middle school and has to reassign every student to the three that remain,
minimizing total busing cost. It is solvable in an afternoon, and the objective is wrong.

The mathematics is Hillier's Case 4.3, carried from a linear program through sensitivity analysis to
a binary formulation across three chapters. The questions below are mine, and they are the reason I
use this case rather than another one. Every student has been to school and had to get there somehow,
so they can feel what the objective function leaves out.

- [The data a reader needs in order to run it](/assets/pdf/teaching/BusingCase_Data.xlsx)

The case text itself is Hillier's and I do not reproduce it here. It is available on request, and
the question set stands without it.

## The questions I ask before anyone formulates anything

**On stakeholder representation.** Who is making decisions in this problem, and whose voices are
absent? The school board sets the constraints and the objective. Students, families, and teachers
are not in the model at all. What could those groups tell us that would change how we frame the
problem?

**On the objective function.** The stated goal is minimizing total busing cost. What does that choice
prioritize and what does it leave out? We could instead minimise the maximum travel time for any
one student, or equalize access across neighborhoods, or optimize for safety. How would the optimal
solution differ under each? When we optimize for cost, we give a voice only to the people who care
about cost.

**On the constraints. **The requirement that each grade make up between 30 and 36 percent of each
school's population looks neutral. What does it assume? In a city with a history of residential
segregation, splitting or not splitting a neighborhood does not land the same way on every
community.

**On the data.** Some assignments are marked infeasible with a dash. What makes an assignment
infeasible, who decided that, and what does it mean for the students who live there? The cost
structure of nothing, 200 dollars, and 300 dollars by distance treats every student's time and
safety as interchangeable. Is that valid across all six areas?

**On the policy options. **The later parts of the case ask students to evaluate eliminating busing for
shorter distances, and frame it as a trade-off between cost and safety. A trade-off for whom?
Consider which neighborhoods have sidewalks, crossing guards, and safe routes, and which families
can drive a child themselves if the bus stops coming.

## What happens when they solve it

The optimal assignment splits several residential areas across multiple schools. Then the board
objects that it wants to keep each neighborhood together, which is a constraint the first model
treated as optional. The adjusted solution costs more.

I frame that increase not as the model failing but as the price of a value that was left out of the
optimization. Community cohesion, carpools, siblings at the same school, and neighborhood identity
were never in the objective, so the model could not have protected them.

The last parts ask for a recommendation weighing cost against safety equally, and the case never
says how to measure the second one. The model computes the cost saving precisely and cannot compute
the safety impact at all. So I ask students what they would need. Accident rates by neighborhood?
Sidewalk coverage? Survey data on which families have another way to get a child to school? A
defensible answer compares the options on several criteria instead of collapsing them into one
number.

Students leave able to build the model. They also leave knowing that a model is a limited
representation, that it encodes whose interests count, and that they carry responsibility for how it
is used.

## One note on the context

School closures and busing optimization have a history in the United States, and optimization
methods were used both to advance and to resist school integration. I raise it briefly rather than
resolve it. Acknowledging it is itself the critical stance I am asking students to take toward their
own models.
