# Fibonacci Sequence: Mathematical Foundations

## Introduction
The Fibonacci sequence is a classic example of a recursive sequence that appears in many natural and mathematical contexts. In this section, we will explore its definition, properties, and connections to the golden ratio.

## Definition & Recurrence
The Fibonacci sequence is defined by the recurrence relation:

$$
F_0 = 0,\quad F_1 = 1,\quad F_n = F_{n-1} + F_{n-2} \quad \text{for } n \ge 2.
$$

The first twenty terms are:

| $n$ | $F_n$ |
|-----|-------|
| 0 | 0 |
| 1 | 1 |
| 2 | 1 |
| 3 | 2 |
| 4 | 3 |
| 5 | 5 |
| 6 | 8 |
| 7 | 13 |
| 8 | 21 |
| 9 | 34 |
| 10 | 55 |
| 11 | 89 |
| 12 | 144 |
| 13 | 233 |
| 14 | 377 |
| 15 | 610 |
| 16 | 987 |
| 17 | 1597 |
| 18 | 2584 |
| 19 | 4181 |
| 20 | 6765 |

## Closed‑Form Expression (Binet’s Formula)
Although defined recursively, Fibonacci numbers can be expressed directly using Binet’s formula:

$$
F_n = \frac{\varphi^n - \psi^n}{\sqrt{5}},
$$

where

$$
\varphi = \frac{1+\sqrt{5}}{2} \approx 1.6180339887\ldots
$$

is the **golden ratio**, and

$$
\psi = \frac{1-\sqrt{5}}{2} = 1-\varphi \approx -0.6180339887\ldots
$$

is its algebraic conjugate.

## The Golden Ratio
The golden ratio $\varphi$ satisfies the quadratic equation $\varphi^2 = \varphi + 1$. It is also the limit of successive Fibonacci ratios:

$$
\lim_{n\to\infty} \frac{F_{n+1}}{F_n} = \varphi.
$$

### Example
Compute the ratio of consecutive Fibonacci numbers for $n=10$:

$$
\frac{F_{11}}{F_{10}} = \frac{89}{55} \approx 1.61818,
$$

which is already very close to $\varphi$.

## Geometric Interpretation: The Fibonacci Spiral
If squares with side lengths equal to Fibonacci numbers are arranged in a “spiral” pattern, quarter‑circles drawn inside each square produce the famous **Fibonacci spiral**.

![Fibonacci spiral diagram](https://upload.wikimedia.org/wikipedia/commons/2/2e/FibonacciSpiral.svg)

*Construction steps:*
1. Start with a $1\times 1$ square.
2. Place another $1\times 1$ square beside it.
3. Add a $2\times 2$ square below the two $1\times 1$ squares.
4. Continue adding squares whose side lengths follow the Fibonacci sequence, rotating the direction each time.
5. Draw quarter‑circles in each square to form a smooth spiral.

## Example Problems
1. **Next terms:** Given $F_{10}=55$ and $F_{11}=89$, find $F_{12}$, $F_{13}$, and $F_{14}$.
   - *Solution:* $F_{12}=144$, $F_{13}=233$, $F_{14}=377$.

2. **Binet’s verification:** Use Binet’s formula to compute $F_5$ and $F_6$.
   - *Solution:* 
     $$
     F_5 = \frac{\varphi^5 - \psi^5}{\sqrt{5}} \approx \frac{11.09017 - (-0.09017)}{2.23607} = \frac{11.18034}{2.23607} = 5.
     $$
     Similarly, $F_6 = 8$.

3. **Ratio convergence:** Calculate $F_{15}/F_{14}$ and compare with $\varphi$.
   - *Solution:* $610/377 \approx 1.618037$, matching $\varphi$ to five decimal places.

## Connections to Biology (Preview)
The same mathematical patterns appear in many biological structures:
- **Phyllotaxis:** The arrangement of leaves, petals, and seeds often follows Fibonacci numbers (e.g., sunflowers, pinecones).
- **Golden‑ratio proportions:** The lengths of successive segments in branching systems (tree branches, veins in leaves) often approximate $\varphi$.

These connections will be explored in detail in the biology component of the lesson.

---

*This material is part of the cross‑curricular lesson “The Code of Nature: Exploring Fibonacci and Fractals.”*