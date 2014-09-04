ALGORITHM DESIGN
----------------
We say that an algorithm is **good** if:

- *A* runs in time polynomial in the input size n.
- Scales multiplicatively with incrasing computational power

Runtime  | P | 2P 
---|---|---|
n   | T | 2T 
n^2 | sqrt(T) | sqrt(2)sqrt(t)
2^n | logT | log(2T) = logT + 1

**Moore's Law**: Computational power doubles roughly every 2 years. 
> Exponential time algorithms will **never** work on large problems

This defintion of "goodness" is robust.
All reasonable models of computation are polynomially equivalent.
- If not, one model can do, say an exponential number of operations in the time it takes another model to do 1 operation.

> The goal of this course is to understand which problems have good algorithms and which don't.
