+++
order = 6
tags = ["math", "algebra", "systems-of-equations", "substitution", "elimination", "linear"]
+++

# Algebra — Systems of Linear Equations

## 6.1 What a System of Equations Is

C: A [system of equations] is a collection of two or more equations involving the same variables, whose solution is any assignment of values that satisfies all equations simultaneously.

Q: Why is solving a system different from solving a single equation?
A: Because a single equation in two or more variables has infinitely many solutions (a curve or surface), while a system of equations picks out the points that lie on *all* of the curves simultaneously. Finding this intersection often pins down a unique solution — turning an underdetermined problem (one equation, two unknowns) into a determined one (two equations, two unknowns).

## 6.2 Solutions of a Two-Variable System

Q: What are the three possible outcomes when solving a 2-equation, 2-variable linear system?
A: (1) Exactly one solution — the two lines intersect at a single point. (2) No solution — the lines are parallel and never meet (inconsistent system). (3) Infinitely many solutions — the two equations describe the same line (dependent system). Every 2×2 linear system falls into exactly one of these three cases.

C: A 2×2 linear system has either one solution, [no solution], or infinitely many solutions — corresponding to intersecting, parallel, and coincident lines respectively.

## 6.3 The Substitution Method

Q: How does the substitution method for solving a linear system work?
A: Solve one of the equations for one variable in terms of the other, then substitute that expression into the second equation, reducing it to one equation in one unknown. Solve that, then back-substitute to find the other variable. Example: $y = 2x + 1$ and $3x + y = 11$ → substitute $y$: $3x + (2x + 1) = 11\Rightarrow 5x = 10\Rightarrow x = 2$, so $y = 2(2) + 1 = 5$.

Q: When is the substitution method most convenient?
A: When one of the equations is already solved for a variable (or is easy to solve for), so you can plug it directly into the other. It's most awkward when both equations are in general form and require manual rearrangement — in such cases, elimination (next section) is usually faster. Substitution is also a good choice when you want to keep one variable's expression explicit, as in parametric or optimization problems.

## 6.4 The Elimination Method

Q: How does the elimination method (also called addition method) work?
A: Add or subtract suitable multiples of the two equations so that one variable cancels, leaving a single equation in one variable. Solve that, then back-substitute. Example: $3x + 2y = 11$ and $5x - 2y = 13$ — add: $8x = 24\Rightarrow x = 3$, then substitute: $3(3) + 2y = 11\Rightarrow y = 1$. Elimination is often the fastest approach when coefficients are easily made to cancel.

C: In the [elimination method], you multiply one or both equations by constants and add/subtract them to eliminate one variable, leaving a single equation in the other.

## 6.5 When to Multiply Before Eliminating

Q: What do you do if neither variable's coefficients match for elimination?
A: Multiply one or both equations by constants to make the coefficients of one variable equal in magnitude but opposite in sign. Example: $2x + 3y = 7$ and $3x + y = 5$. To eliminate $y$, multiply the second equation by $-3$: $-9x - 3y = -15$. Add to the first: $-7x = -8\Rightarrow x = 8/7$. Then back-substitute. Multiplying is the bridge between "can't cancel directly" and "can apply elimination."

## 6.6 Inconsistent Systems

Q: What happens algebraically when you try to solve an inconsistent system (parallel lines)?
A: You derive a contradiction like $0 = 5$. For example, $x + y = 2$ and $x + y = 5$: subtracting gives $0 = -3$, which is never true — so no $(x, y)$ satisfies both equations. Algebraically, the contradiction is the signal that the two lines cannot intersect. Geometrically, they are parallel with different intercepts.

## 6.7 Dependent Systems

Q: What happens algebraically when you try to solve a dependent system (coincident lines)?
A: You derive a tautology like $0 = 0$ after simplifying. For example, $2x + 4y = 6$ and $x + 2y = 3$: the first is exactly twice the second, so they describe the same line. Elimination reduces everything to $0 = 0$, which is always true but tells you nothing new. The solution is the whole line, expressed as a free parameter: $x = t, y = (3 - t)/2$ for any real $t$.

## 6.8 Three Variables

Q: How do you solve a system of three linear equations in three unknowns?
A: By systematically eliminating variables: use one equation to eliminate a variable from the other two, leaving a 2×2 system in the remaining variables. Solve that, then back-substitute into one of the original equations to find the eliminated variable. This is the "back-substitution" approach and is the algebraic version of Gaussian elimination, which generalizes to any number of variables.

C: The general strategy for a 3×3 linear system is to [eliminate one variable] to reduce to a 2×2 system, solve it, and then back-substitute.

## 6.9 Systems of Inequalities

Q: How does the solution of a system of linear inequalities look geometrically?
A: It is a region (sometimes called a "feasible region") bounded by the lines corresponding to the equalities. For example, $x + y\leq 4$ and $x\geq 0$ and $y\geq 0$ describes a triangular region in the first quadrant bounded by the axes and the line $x + y = 4$. The feasible region is the intersection of half-planes, one for each inequality, and may be bounded or unbounded depending on the constraints.

## 6.10 System by Elimination — P:/S:

P: Solve the system $\begin{cases}2x + 3y = 12 \\ 5x - 2y = 11\end{cases}$ using the elimination method.

S:
**IDENTIFY**: A 2×2 linear system. Use elimination to remove one variable, solve for the other, and back-substitute.

**PLAN**:
- Decide which variable to eliminate. Look at coefficients: $3y$ and $-2y$ — the LCM of $3$ and $2$ is $6$, so making $y$-coefficients $+6$ and $-6$ requires multiplying equation 1 by $2$ and equation 2 by $3$.
- Multiply and add the equations to eliminate $y$.
- Solve the resulting single-variable equation for $x$.
- Back-substitute into either original equation to find $y$.
- Verify in the other original equation.

**EXECUTE**:
1. Multiply equation 1 by $2$: $4x + 6y = 24$.
2. Multiply equation 2 by $3$: $15x - 6y = 33$.
3. Add: $(4x + 15x) + (6y - 6y) = 24 + 33\Rightarrow 19x = 57$.
4. Solve: $x = 57/19 = 3$.
5. Back-substitute into equation 1: $2(3) + 3y = 12\Rightarrow 6 + 3y = 12\Rightarrow 3y = 6\Rightarrow y = 2$.
6. Solution: $(x, y) = (3, 2)$.

**EVALUATE**:
- Check equation 1: $2(3) + 3(2) = 6 + 6 = 12$. ✓
- Check equation 2: $5(3) - 2(2) = 15 - 4 = 11$. ✓
- Both equations are satisfied, so $(3, 2)$ is the unique solution.
- Geometrically, the two lines intersect at exactly the point $(3, 2)$. This is the "one solution" case — the generic outcome for a 2×2 system whose two lines are neither parallel nor coincident.
- Alternative: substitution would also have worked. From equation 1, $y = (12 - 2x)/3$. Substituting into equation 2: $5x - 2(12 - 2x)/3 = 11\Rightarrow 15x - 2(12 - 2x) = 33\Rightarrow 15x - 24 + 4x = 33\Rightarrow 19x = 57\Rightarrow x = 3$. Same answer, but slightly more fraction handling.
- For this problem, elimination was faster because the coefficients were easy to manipulate. In general, if one equation is already "solved" for a variable, substitution is usually faster; if both are in general form, elimination is usually cleaner. Fluency in both methods lets you pick whichever suits the problem.
- This example also shows the importance of *verification* — plugging the solution back into both original equations catches arithmetic errors immediately. Never skip this step on an exam.
- For larger systems (3×3 or more), the same elimination strategy generalizes into Gaussian elimination, which is the foundation of linear algebra and numerical methods. Learning it well here will pay off dramatically when you meet matrices.
