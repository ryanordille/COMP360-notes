Lecture 2 -- September 4

Network Flows (Maximum Flows)
=============================

A good is produced at a vertex *s* and we want to transport as much of it as possible to a vertex *t*. 

The difficulty is that each link (arc *a = (i, j)*) has a capacity *U<sub>ij</sub>* stating the maximum amount of the good that can be sent through the arc (in a fixed time period, say).
    - Applications:
        - sending oil through pipelines
        - current in electrical network
        - data packets in an information network
        - goods in a transportation network
        - currency flows in a financial market
        - + *many more 'strange' applications*

Formally, given a directed graph *G = (V,A)* a **flow** *f* has two properties

1. Capacity constraints: 
    *0 <= *f<sub>ij</sub> *<= *u<sub>ij</sub>
2. Flow Conservation:
    *flow.in(v) = flow.out(v)*

    > The sum of the incoming flow of all considered vertices must match the sum of the outgoing flow of all considered vertices.

The value of *|f|* of a flow is the amount of the good sent from *s* to *t*.

**ie** flow.out(s) = *|f|* = flow.in(t)
- We may assume there are no arcs into *s* or out of *t* as they are not useful for us.

Max-Flow Porblem: Find an *s-t* flow *f** of maximum value.
- *Informally, we are trying to **fit** as many *s-t* paths into *G* as possible*
- Extensions: lower bounds on the arcs; multiple sources/sinks
