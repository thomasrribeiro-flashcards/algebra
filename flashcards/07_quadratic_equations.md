+++
order = 7
tags = ["math", "algebra", "quadratic-equations", "quadratic-formula", "completing-the-square", "discriminant"]
+++

# Algebra — Quadratic Equations

## 7.1 What a Quadratic Equation Is

C: A [quadratic equation] in one variable is an equation that can be written in the standard form $ax^2 + bx + c = 0$, where $a, b, c$ are real numbers and $a\neq 0$.

Q: Why is the condition $a\neq 0$ essential in the definition of a quadratic?
A: Because if $a = 0$, the $x^2$ term disappears and what remains, $bx + c = 0$, is linear, not quadratic. The defining feature of a quadratic equation is the presence of an $x^2$ term, which is what gives it up to two solutions and distinguishes its behavior from linear equations. Without $a\neq 0$, the equation would not belong to the quadratic category at all.

## 7.2 Solving by Factoring

Q: How do you solve a quadratic equation by factoring?
A: Rearrange the equation into standard form $ax^2 + bx + c = 0$, factor the left side as a product of linear factors, and apply the zero-product property: a product is zero iff at least one factor is zero. Example: $x^2 - 5x + 6 = 0\Rightarrow (x - 2)(x - 3) = 0\Rightarrow x = 2$ or $x = 3$. This is the quickest method when the quadratic factors cleanly over the rationals.

C: The [zero-product property] says that $AB = 0$ if and only if $A = 0$ or $B = 0$; this is what turns a factored quadratic into two linear equations.

## 7.3 Solving by Taking Square Roots

Q: How do you solve an equation of the form $(x - h)^2 = k$?
A: Take the square root of both sides, remembering the $\pm$: $x - h = \pm\sqrt{k}$, so $x = h\pm\sqrt{k}$. The $\pm$ captures both roots — forgetting it gives only half the solution. This method works for any equation that can be written with a single squared expression on one side.

Q: Why must you include $\pm$ when taking square roots in an equation but not when evaluating a root expression?
A: Because "the principal square root" ($\sqrt{k}$) is by definition non-negative — evaluating $\sqrt{4}$ gives only $2$. But solving an equation like $x^2 = 4$ asks for *all* $x$ satisfying it — both $2$ and $-2$ do. So when you take square roots as a step in solving, both signs must be included; when you merely evaluate a radical, only the principal root is intended.

## 7.4 Completing the Square

Q: What does "completing the square" mean, and why is it useful?
A: It means rewriting a quadratic $ax^2 + bx + c$ as $a(x - h)^2 + k$ for some $h, k$ — a form with the variable appearing inside a perfect square. This is useful because $(x - h)^2 = -k/a$ can then be solved by taking square roots, no factoring required. It's also the standard way to find the vertex of a parabola (chapter 8) and is the technique used to derive the quadratic formula.

## 7.5 Deriving the Quadratic Formula

Q: How is the quadratic formula derived by completing the square?
A: Start with $ax^2 + bx + c = 0$. Divide by $a$: $x^2 + (b/a)x + c/a = 0$. Move constant: $x^2 + (b/a)x = -c/a$. Complete the square by adding $(b/2a)^2$ to both sides: $(x + b/(2a))^2 = -c/a + b^2/(4a^2) = (b^2 - 4ac)/(4a^2)$. Take square root: $x + b/(2a) = \pm\sqrt{b^2 - 4ac}/(2a)$. Solve: $x = (-b\pm\sqrt{b^2 - 4ac})/(2a)$. Done.

## 7.6 The Quadratic Formula

C: The [quadratic formula] gives the solutions of $ax^2 + bx + c = 0$ as $x = (-b\pm\sqrt{b^2 - 4ac})/(2a)$.

Q: Why is the quadratic formula guaranteed to work when factoring fails?
A: Because it was derived by completing the square without any assumption about the roots being rational or the quadratic factoring nicely. Completing the square transforms any quadratic into a form that can be solved by taking square roots, giving explicit formulas for the roots in terms of the coefficients. Whenever $b^2 - 4ac\geq 0$, the formula produces real solutions; otherwise the solutions are complex.

## 7.7 The Discriminant

C: The [discriminant] of $ax^2 + bx + c = 0$ is $\Delta = b^2 - 4ac$; its sign determines the nature of the solutions.

Q: What do the three cases of the discriminant tell you about the roots?
A: (1) $\Delta > 0$: two distinct real roots — the formula produces two different values. (2) $\Delta = 0$: one repeated real root (a double root) — the $\pm$ gives the same answer twice. (3) $\Delta < 0$: no real roots; the solutions are complex conjugates (we'll treat complex numbers in a later deck). The discriminant lets you describe the solutions without actually computing them — useful when you only need the *type* of solutions, not their values.

## 7.8 Vieta's Formulas

Q: If $x_1$ and $x_2$ are the roots of $ax^2 + bx + c = 0$, what do their sum and product equal in terms of the coefficients?
A: By Vieta's formulas, $x_1 + x_2 = -b/a$ and $x_1 x_2 = c/a$. These follow from expanding $a(x - x_1)(x - x_2) = ax^2 - a(x_1 + x_2)x + ax_1 x_2$ and comparing to $ax^2 + bx + c$. Vieta's formulas are useful for checking solutions and for constructing quadratics with specified roots.

C: For a quadratic $ax^2 + bx + c = 0$ with roots $x_1, x_2$: $x_1 + x_2 = [-b/a]$ and $x_1 x_2 = c/a$.

## 7.9 Word Problems and Quadratics

Q: Why do so many word problems reduce to quadratic equations?
A: Because many natural relationships — area as length times width, projectile height as initial height plus initial velocity times time minus $(1/2)gt^2$, compound interest over multiple periods — involve products of two related quantities or squared quantities. Once translated into algebra, these produce equations of degree 2. Recognizing the quadratic structure early lets you jump straight to the quadratic formula or factoring.

## 7.10 Quadratic Equation — P:/S:

P: Solve $2x^2 - 7x + 3 = 0$ using the quadratic formula, and verify the sum and product of the roots using Vieta's formulas.

S:
**IDENTIFY**: A quadratic equation in standard form with $a = 2, b = -7, c = 3$. Use the quadratic formula to find the roots, then check via Vieta's formulas.

**PLAN**:
- Identify $a, b, c$ from the standard form.
- Compute the discriminant $\Delta = b^2 - 4ac$.
- Plug into the formula $x = (-b\pm\sqrt{\Delta})/(2a)$.
- Verify: $x_1 + x_2$ should equal $-b/a$, and $x_1 x_2$ should equal $c/a$.

**EXECUTE**:
1. $a = 2, b = -7, c = 3$.
2. Discriminant: $\Delta = (-7)^2 - 4(2)(3) = 49 - 24 = 25$.
3. $\sqrt{\Delta} = 5$.
4. $x = (-(-7)\pm 5)/(2\cdot 2) = (7\pm 5)/4$.
5. $x_1 = (7 + 5)/4 = 12/4 = 3$.
6. $x_2 = (7 - 5)/4 = 2/4 = 1/2$.
7. Solutions: $x\in\{3, 1/2\}$.

**EVALUATE**:
- Check $x_1 = 3$: $2(3)^2 - 7(3) + 3 = 18 - 21 + 3 = 0$. ✓
- Check $x_2 = 1/2$: $2(1/2)^2 - 7(1/2) + 3 = 1/2 - 7/2 + 3 = (1 - 7)/2 + 3 = -3 + 3 = 0$. ✓
- Vieta's formulas: sum $= x_1 + x_2 = 3 + 1/2 = 7/2$. Expected: $-b/a = 7/2$. ✓
- Product $= x_1 x_2 = 3\cdot(1/2) = 3/2$. Expected: $c/a = 3/2$. ✓
- Both Vieta checks match, giving independent confirmation that the roots are correct. This is a good practice for exam problems: after applying the quadratic formula, verify with Vieta's formulas in a few seconds.
- Discriminant $\Delta = 25 > 0$: ✓ consistent with two distinct real roots. Had $\Delta$ come out to 0, the formula would have given a single repeated root; had it been negative, the solutions would have been complex.
- This quadratic could also have been factored: $2x^2 - 7x + 3 = (2x - 1)(x - 3) = 0$, giving $x = 1/2$ or $x = 3$ directly. For "nice" rational-root quadratics, factoring is faster; for anything with irrational or complex roots, the quadratic formula is the reliable general method.
- The quadratic formula should become a reflex — memorized, checked, and applied without hesitation. Along with factoring and completing the square, it is the complete toolkit for solving degree-2 equations and is the foundation for understanding parabolas, conic sections, and the quadratic approximation of arbitrary functions.
