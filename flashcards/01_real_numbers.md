+++
order = 1
subject = "Math"
tags = ["math", "algebra", "real-numbers", "order", "absolute-value", "number-line"]
+++

# Algebra — Real Numbers and Arithmetic Foundations

## 1.1 Why Start With the Real Numbers

Q: Why does algebra begin with a careful look at the real number system?
A: Because every symbol, equation, and function you write in algebra ultimately represents or operates on real numbers. Before manipulating symbols, you need to know what kinds of numbers exist, how they are ordered, and which rules they obey. Rushing into equations without understanding the underlying number system leads to silent errors — for example, dividing by zero, taking square roots of negatives, or confusing "is less than" with "has smaller absolute value."

## 1.2 Natural Numbers

C: The [natural numbers] are $\mathbb{N} = \{1, 2, 3, \dots\}$ — the counting numbers used for positive whole quantities.

Q: Why are the natural numbers insufficient for algebra?
A: Because subtraction is not always possible within them: $3 - 5$ has no answer in $\mathbb{N}$. Algebra needs a number system closed under subtraction so that equations like $x + 5 = 3$ have solutions. Extending $\mathbb{N}$ to include $0$ and negative numbers gives the integers, which are closed under subtraction.

## 1.3 Integers

C: The [integers] are $\mathbb{Z} = \{\dots, -2, -1, 0, 1, 2, \dots\}$ — the naturals extended with zero and the negatives of the naturals.

Q: Why are the integers still insufficient for algebra?
A: Because division is not always possible within them: $3 \div 2$ has no answer in $\mathbb{Z}$. To solve equations like $2x = 3$, we need a number system closed under division (by nonzero elements). Extending $\mathbb{Z}$ to include ratios of integers gives the rational numbers.

## 1.4 Rational Numbers

C: The [rational numbers] are $\mathbb{Q} = \{p/q : p, q\in\mathbb{Z},\; q\neq 0\}$ — all ratios of integers with nonzero denominator.

Q: Why must the denominator $q$ be nonzero in a rational number?
A: Because division by zero is undefined: no real number $x$ satisfies $q\cdot x = p$ when $q = 0$ and $p\neq 0$, and every real $x$ satisfies it when $p = 0$. In neither case is the expression $p/0$ a single well-defined number. Excluding $q = 0$ from the definition of rationals is not a convention; it is a requirement for the resulting object to be a number at all.

Q: Why are the rationals still insufficient as a complete number system for algebra?
A: Because some equations with rational coefficients have no rational solutions: for example, $x^2 = 2$ is satisfied by no rational number (a theorem of Greek mathematics — $\sqrt{2}$ is irrational). To include solutions like $\sqrt{2}$, $\pi$, and $e$, we need the real numbers, which fill in the "gaps" left by the rationals.

## 1.5 Irrational Numbers

C: An [irrational number] is a real number that cannot be written as $p/q$ for integers $p, q$ with $q\neq 0$; examples include $\sqrt{2}$, $\pi$, and $e$.

Q: Why is $\sqrt{2}$ irrational?
A: Suppose $\sqrt{2} = p/q$ in lowest terms. Then $2q^2 = p^2$, so $p^2$ is even, hence $p$ is even, so $p = 2k$. Substituting gives $2q^2 = 4k^2$, so $q^2 = 2k^2$, which means $q$ is also even — contradicting the assumption that $p/q$ was in lowest terms. So no such $p, q$ exist. This is one of the earliest known proofs by contradiction in mathematics.

## 1.6 Real Numbers

C: The [real numbers] $\mathbb{R}$ are the union of the rationals and the irrationals, visualized as every point on an infinite number line with no gaps.

Q: Why is the real number line often described as "complete" while the rational line is not?
A: Because every non-empty set of reals that is bounded above has a least upper bound (supremum) in $\mathbb{R}$, but this fails for $\mathbb{Q}$: the set $\{x\in\mathbb{Q}: x^2 < 2\}$ is bounded above (by 2, for instance) but has no least upper bound within $\mathbb{Q}$ — its "natural" supremum $\sqrt{2}$ is not rational. The reals are constructed precisely to eliminate such gaps.

## 1.7 The Number Line

Q: What does it mean geometrically to represent real numbers on a number line?
A: Each real number corresponds to exactly one point on an infinite horizontal line, with 0 at the origin, positive numbers extending to the right, and negative numbers to the left. Distance between points corresponds to the absolute difference of their values, and order (left of / right of) corresponds to numerical order. The number line is a geometric tool for visualizing algebraic relationships.

C: On the number line, a number $a$ is less than $b$ if and only if $a$ lies [to the left of] $b$.

## 1.8 Ordering of the Reals

C: For any two real numbers $a$ and $b$, exactly one of $a < b$, $a = b$, or $a > b$ holds — a property called [trichotomy].

Q: What does it mean for $<$ to be transitive, and why does that matter algebraically?
A: Transitivity means: if $a < b$ and $b < c$, then $a < c$. It lets you chain inequalities, so you can conclude $a < c$ without directly comparing $a$ to $c$. Transitivity is the property that makes ordering "work" as an intuitive notion of "smaller than" — without it, sorting and comparing numbers would break down.

## 1.9 Absolute Value

C: The [absolute value] of a real number $a$ is $|a| = a$ if $a\geq 0$ and $|a| = -a$ if $a < 0$; it represents the distance of $a$ from $0$ on the number line.

Q: Why does the definition of absolute value have two cases?
A: Because distance is always non-negative, but real numbers can be negative. For $a\geq 0$, the distance from $0$ is just $a$. For $a < 0$, the distance is the positive version $-a$ (e.g., the distance from $-3$ to $0$ is $3$, which equals $-(-3)$). The two-case definition ensures $|a|\geq 0$ for every $a$, regardless of sign.

Q: What is the geometric meaning of $|a - b|$?
A: It is the distance between the points $a$ and $b$ on the number line, regardless of which one is larger. So $|5 - 2| = 3$ and $|2 - 5| = 3$ both give the correct distance. Writing distances as absolute values is a basic pattern that will appear throughout algebra, geometry, and calculus.

C: The distance between two real numbers $a$ and $b$ is [$|a - b|$], always non-negative and independent of order.

## 1.10 Basic Properties of Absolute Value

Q: Why does $|ab| = |a|\cdot|b|$ hold for all real $a$ and $b$?
A: Because the sign of a product is determined by the signs of the factors, but the magnitude is unaffected by signs. Whether $a$ and $b$ are positive or negative, $|ab|$ ignores the sign of the product and returns the magnitude, which is always the product of magnitudes. This multiplicative property makes absolute value play well with multiplication but not (directly) with addition.

Q: Why is $|a + b|\leq |a| + |b|$ (the triangle inequality), with equality only when $a$ and $b$ have the same sign?
A: Because if $a$ and $b$ agree in sign, they reinforce and $|a + b| = |a| + |b|$. If they disagree in sign, they partially cancel and $|a + b| < |a| + |b|$. Geometrically, going from $0$ to $a + b$ directly is never longer than going from $0$ to $a$ and then adding $|b|$ — the "triangle inequality" in its one-dimensional form. This inequality generalizes to vectors in higher dimensions.

C: The [triangle inequality] states $|a + b|\leq |a| + |b|$, with equality if and only if $a$ and $b$ have the same sign.

## 1.11 Order of Operations

Q: Why is an agreed order of operations necessary when evaluating arithmetic expressions?
A: Because different orderings give different answers: $2 + 3\times 4 = 14$ if you multiply first, or $20$ if you add first. Without a fixed convention, the same expression would be ambiguous. The standard order — parentheses, exponents, multiplication/division (left to right), addition/subtraction (left to right) — is a universally adopted convention, commonly memorized as PEMDAS or BODMAS.

C: The standard order of operations is [parentheses, exponents, multiplication/division, addition/subtraction], evaluated left-to-right within each precedence level.

## 1.12 Solving a Distance Equation — P:/S:

P: Find all real numbers $x$ such that $|x - 3| = 5$. Describe the geometric meaning on the number line.

S:
**IDENTIFY**: An absolute-value equation. Use the definition: $|a| = c$ (for $c > 0$) means $a = c$ or $a = -c$.

**PLAN**:
- Apply the definition to $|x - 3| = 5$: either $x - 3 = 5$ or $x - 3 = -5$.
- Solve each linear equation for $x$.
- Check both candidates by substituting back.
- Interpret geometrically: $|x - 3|$ is the distance between $x$ and $3$.

**EXECUTE**:
1. Case 1: $x - 3 = 5\Rightarrow x = 8$.
2. Case 2: $x - 3 = -5\Rightarrow x = -2$.
3. Check $x = 8$: $|8 - 3| = |5| = 5$. ✓
4. Check $x = -2$: $|-2 - 3| = |-5| = 5$. ✓
5. Solution set: $x\in\{-2, 8\}$.

**EVALUATE**:
- Geometrically, the equation $|x - 3| = 5$ asks: which points on the number line are exactly 5 units away from $3$? There are two such points: one 5 units to the right of 3 (that's 8) and one 5 units to the left of 3 (that's $-2$). ✓
- If the equation had been $|x - 3| = 0$, there would be exactly one solution ($x = 3$, zero distance from $3$). If the right side had been negative, say $|x - 3| = -5$, there would be no solution, because absolute value is never negative. These three cases (two solutions, one solution, no solution) exhaust all possibilities for $|x - a| = c$.
- The same pattern generalizes to absolute-value *inequalities*: $|x - 3| < 5$ describes the open interval $(-2, 8)$, and $|x - 3| > 5$ describes the two unbounded intervals $(-\infty, -2)\cup(8, \infty)$. Both use the same "distance from 3" interpretation but translate into a range rather than two points.
- Recognizing $|x - a|$ as "distance from $a$" is a pattern you will apply repeatedly: in solving inequalities, in describing open/closed intervals, in defining limits in calculus, and in writing metric spaces in analysis.
