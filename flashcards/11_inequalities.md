+++
order = 11
tags = ["math", "algebra", "inequalities", "interval-notation", "absolute-value", "sign-chart"]
+++

# Algebra — Inequalities

## 11.1 What an inequality is; comparison with equations

Q: What is an inequality, and how does its solution set differ from that of an equation?
A: An inequality is a statement that one expression is less than, greater than, or possibly equal to another, using the symbols $<$, $\leq$, $>$, or $\geq$. Unlike an equation such as $2x+1=5$, whose solution is typically a finite set of isolated numbers ($x=2$), an inequality like $2x+1\leq 5$ has a solution set that is usually an interval or union of intervals on the real line (here $x\leq 2$). This is because inequalities describe regions of order rather than exact equality. Solving an inequality therefore means finding every real number that makes the statement true, not just a handful of roots.

C: The symbol $\leq$ means "[less than or equal to]", so $a\leq b$ is true when $a$ is either strictly smaller than $b$ or exactly equal to $b$.

Q: Why do inequalities usually have infinitely many solutions while equations typically have finitely many?
A: An equation imposes the exact condition that two expressions coincide, which on the real line generically forces a discrete set of points (e.g., the roots of a polynomial). An inequality instead asks which side of that boundary we lie on, so whenever a single point satisfies a strict inequality, nearby points do too by continuity. The solution set is therefore open or closed around those boundary points, producing intervals. Equations carve out points; inequalities carve out regions.

## 11.2 Interval notation: open, closed, half-open, infinite

Q: What is interval notation and why is it useful for writing solution sets of inequalities?
A: Interval notation is a compact way to describe a contiguous set of real numbers by listing only its endpoints together with symbols that indicate whether each endpoint is included. A square bracket $[\,$ or $\,]$ means the endpoint belongs to the set, while a parenthesis $($ or $)$ means it does not. It is useful because inequality solutions are almost always intervals or unions of intervals, so instead of writing "all $x$ with $-2\leq x < 5$" we can simply write $[-2,5)$. This notation also plugs cleanly into set operations like union and intersection.

C: The [closed interval] $[a,b]$ denotes all real $x$ with $a\leq x\leq b$; the square brackets indicate that both endpoints $a$ and $b$ are included.

C: The [open interval] $(a,b)$ denotes all real $x$ with $a < x < b$; parentheses indicate that neither endpoint is included.

C: The half-open interval $[a,b)$ contains $a$ but [excludes] $b$; it corresponds to $a\leq x < b$.

C: The infinite interval $[a,\infty)$ denotes all $x$ with $x\geq a$, and we always write $\infty$ with a [parenthesis] because infinity is not a real number and cannot be "included" as an endpoint.

## 11.3 Solving linear inequalities — parallel to equations

Q: Why can most steps used to solve linear equations be applied directly to linear inequalities?
A: Adding or subtracting the same quantity on both sides of an inequality shifts both sides by equal amounts on the number line, so their relative order is preserved. Multiplying or dividing both sides by the same positive number scales the line uniformly and also preserves order. These are exactly the elementary moves used to isolate $x$ in a linear equation, so the algebra of solving $3x+2\leq 11$ looks identical to solving $3x+2=11$ until the final step. The crucial exception, covered in 11.4, is multiplication or division by a negative number.

Q: Solve $3x+2\leq 11$ and express the answer in interval notation.
A: Subtract $2$ from both sides to get $3x\leq 9$; this preserves the inequality because we added the same number to both sides. Divide both sides by $3$, which is positive, so the direction of $\leq$ is unchanged, giving $x\leq 3$. The solution set is every real number at most $3$, which in interval notation is $(-\infty,3]$. The square bracket reflects that $x=3$ satisfies $\leq$.

## 11.4 The sign-flip rule — why multiplying/dividing by a negative reverses the inequality

Q: Why does multiplying both sides of an inequality by a negative number reverse the inequality?
A: Multiplying by a negative "flips" the number line — every positive becomes negative and vice versa, and the relative order of every pair is reversed. If $a < b$ then $a$ lies left of $b$ on the number line, but after multiplying by $-1$ the image of $a$ lies right of the image of $b$, so $-a > -b$. Concretely, $2<3$ but $-2>-3$. The rule applies only to multiplication or division by a negative; addition and subtraction shift both sides equally and preserve order.

C: When you multiply or divide both sides of an inequality by a negative number, you must [reverse] the direction of the inequality sign.

Q: Solve $-2x+1 > 7$ and explain which step requires the sign-flip rule.
A: Subtract $1$ from both sides, giving $-2x>6$; this step uses only addition/subtraction so the inequality direction is preserved. Now divide both sides by $-2$; because $-2$ is negative, the direction must reverse from $>$ to $<$, yielding $x<-3$. The solution set is $(-\infty,-3)$. The parenthesis reflects that the inequality is strict.

## 11.5 Compound inequalities — "and" vs "or" (intersection vs union)

Q: What is the difference between an "and" compound inequality and an "or" compound inequality?
A: An "and" compound inequality requires both conditions to hold simultaneously, so its solution set is the intersection of the two individual solution sets. An "or" compound inequality requires at least one of the conditions to hold, so its solution set is the union of the two. Intersection typically produces a single interval (or the empty set), while union often produces a disjoint pair of intervals. The word "and" corresponds to $\cap$ and "or" corresponds to $\cup$.

C: The solution set of an "and" compound inequality is the [intersection] of the individual solution sets, because both conditions must hold at once.

C: The solution set of an "or" compound inequality is the [union] of the individual solution sets, because only one condition needs to hold.

Q: Solve the compound inequality $-1 < 2x+3 \leq 7$.
A: This is shorthand for "$-1<2x+3$ AND $2x+3\leq 7$", so we solve both simultaneously by operating on all three parts. Subtract $3$ from each part: $-4<2x\leq 4$. Divide each part by $2$ (positive, so no flip): $-2<x\leq 2$. The solution is the interval $(-2,2]$, open at $-2$ because the left inequality is strict and closed at $2$ because the right is non-strict.

## 11.6 Absolute value inequalities: $|x| < a$ means $-a < x < a$

Q: Why is $|x|<a$ (for $a>0$) equivalent to the compound inequality $-a<x<a$?
A: The absolute value $|x|$ measures the distance from $x$ to $0$ on the number line. Saying $|x|<a$ therefore says "$x$ is within distance $a$ of zero", which geometrically is the open interval centered at $0$ with radius $a$. That interval is exactly the set of real numbers strictly greater than $-a$ and strictly less than $a$, i.e., $-a<x<a$. If $a\leq 0$ the inequality $|x|<a$ has no solutions, since absolute value is never negative.

C: For $a>0$, the inequality $|x|\leq a$ is equivalent to the compound inequality $[-a\leq x\leq a]$, because $|x|$ measures distance from $0$.

Q: Solve $|2x-1|<5$.
A: Rewrite the absolute value inequality as the compound inequality $-5<2x-1<5$, since $|E|<5$ means $E$ lies within distance $5$ of $0$. Add $1$ to all three parts: $-4<2x<6$. Divide by $2$ (positive): $-2<x<3$. The solution is the open interval $(-2,3)$.

## 11.7 Absolute value inequalities: $|x| > a$ means $x < -a$ or $x > a$

Q: Why is $|x|>a$ (for $a\geq 0$) equivalent to "$x<-a$ or $x>a$"?
A: $|x|>a$ says the distance from $x$ to $0$ is greater than $a$, i.e., $x$ lies outside the interval $[-a,a]$. The complement of that interval on the real line is the union $(-\infty,-a)\cup(a,\infty)$, which corresponds to "$x<-a$ OR $x>a$". Because the solution is the exterior of an interval it naturally splits into two disjoint pieces, which is why the "or" form is required rather than a single compound interval. If $a<0$, every real $x$ satisfies $|x|>a$ trivially.

Q: Solve $|3x+2|\geq 4$ and explain why the solution splits into two pieces.
A: Rewrite as the "or" statement $3x+2\leq -4$ or $3x+2\geq 4$, since $|E|\geq 4$ means $E$ is at distance at least $4$ from $0$, forcing it above $4$ or below $-4$. From $3x+2\leq -4$ we get $3x\leq -6$, so $x\leq -2$. From $3x+2\geq 4$ we get $3x\geq 2$, so $x\geq 2/3$. The solution is the union $(-\infty,-2]\cup[2/3,\infty)$; it splits because the set "far from a point" is the complement of an interval, which is disconnected.

## 11.8 Quadratic inequalities — why you can't just "move to one side and take a root"

Q: Why can't a quadratic inequality like $x^2-x-6\geq 0$ be solved by just taking a square root the way one solves $x^2=9$?
A: Taking a square root undoes squaring only when the expression is known to equal a specific value, but an inequality describes a region, not a single value, and $x^2-x-6$ is not a pure square. Moreover, squaring is not a monotonic operation on all of $\mathbb R$: it decreases on $(-\infty,0)$ and increases on $(0,\infty)$, so "undoing" it does not preserve inequality directions globally. The correct approach is to factor the quadratic (using the tools from chapter on factoring) and analyze the sign of each factor separately. This sign analysis, introduced next, replaces naive root-taking.

C: A quadratic inequality like $ax^2+bx+c>0$ is solved by first factoring it, then analyzing the [sign] of each factor on the intervals between the roots.

## 11.9 Sign analysis / sign chart method

Q: What is a sign chart, and why does it correctly solve polynomial and rational inequalities?
A: A sign chart is a diagram of the real number line on which we mark every point where a factor of the expression is zero or undefined; these are the only points where the expression can change sign. Between consecutive marked points each factor has constant sign (by continuity and the intermediate value theorem applied to each factor), so the product or quotient also has constant sign on each open interval. We then pick a convenient test value from each interval to determine that sign. The solution of the inequality is the union of intervals whose sign matches the desired direction, together with boundary points where appropriate.

C: On a sign chart, the sign of a product or quotient can change only at points where a factor equals [zero] or is undefined; between such points the sign is constant.

Q: Why do we only need one test value per interval on a sign chart?
A: Each factor of a factored polynomial or rational expression is continuous and nonzero on an open interval between consecutive critical points, so it cannot change sign there without passing through zero — which would create another critical point, contradicting the choice of interval. Hence the sign of each factor, and therefore of their product or quotient, is constant on that interval. One test value is enough to determine that constant sign for the whole interval.

## 11.10 Solving quadratic inequalities using sign charts

Q: Describe the sign-chart method for solving a quadratic inequality $ax^2+bx+c\,\square\,0$, where $\square$ is one of $<,\leq,>,\geq$.
A: First move everything to one side so the inequality reads "expression $\square$ 0", then factor the quadratic as $a(x-r_1)(x-r_2)$ where $r_1\leq r_2$ are the real roots. Mark $r_1$ and $r_2$ on a number line, creating the three intervals $(-\infty,r_1)$, $(r_1,r_2)$, $(r_2,\infty)$. Pick a test value in each interval and record the sign of the factored expression there. Finally, select the intervals whose sign matches the desired direction, including $r_1$ and $r_2$ themselves if the inequality is non-strict ($\leq$ or $\geq$).

Q: Solve $x^2+2x-3<0$ using a sign chart.
A: Factor: $x^2+2x-3=(x+3)(x-1)$, so the critical points are $x=-3$ and $x=1$, dividing the line into $(-\infty,-3)$, $(-3,1)$, and $(1,\infty)$. Test $x=-4$: $(-)(-)=+$; test $x=0$: $(+)(-)=-$; test $x=2$: $(+)(+)=+$. We want the expression strictly negative, which happens only on $(-3,1)$. The solution is $(-3,1)$, with parentheses because the inequality is strict.

## 11.11 Rational inequalities — sign-change points from numerator AND denominator zeros

Q: In a rational inequality, why must the sign chart include zeros of both the numerator and the denominator?
A: A rational expression $N(x)/D(x)$ can change sign only where $N(x)=0$ (the expression itself is zero) or where $D(x)=0$ (the expression is undefined, and crossing such a point flips the sign of the denominator). Numerator zeros may or may not be included in the solution set depending on whether the inequality is strict, but denominator zeros are never included because the expression is not defined there. Omitting denominator zeros from the chart would miss genuine sign changes and give an incorrect solution.

C: On a sign chart for a rational inequality, zeros of the denominator must always be marked but [excluded] from the solution set, because the expression is undefined there.

## 11.12 Why you cannot clear denominators by multiplying in a rational inequality

Q: Why is it generally wrong to "clear the denominator" in a rational inequality by multiplying both sides by the denominator, as one would in an equation?
A: Multiplying both sides of an inequality by a quantity preserves the inequality only if that quantity has a known, fixed sign — positive keeps the direction, negative reverses it (11.4). In a rational inequality like $\tfrac{x-1}{x+2}\geq 0$, the denominator $x+2$ changes sign depending on $x$, so multiplying by it would require splitting into cases and would likely flip the inequality on some of those cases. The safer, systematic method is to move everything to one side, combine into a single fraction, and apply the sign-chart method treating numerator and denominator zeros as critical points.

## 11.13 Polynomial inequalities — generalize the sign chart

Q: How does the sign-chart method extend from quadratics to general polynomial inequalities?
A: Given $P(x)\,\square\,0$ with $P$ a polynomial, factor $P$ completely over the reals as a product of linear and irreducible quadratic factors; the real roots of $P$ are exactly the critical points. Mark all real roots on the number line, partitioning it into finitely many open intervals, and determine the sign of $P$ on each using one test value. Irreducible quadratic factors have constant sign (always positive or always negative depending on leading coefficient) and do not contribute critical points. Finally pick the intervals matching the desired sign, including roots themselves iff the inequality is non-strict.

C: An irreducible quadratic factor like $x^2+1$ contributes no critical points to a sign chart, because it is never [zero] on the real line and so has constant sign everywhere.

Q: Why does a repeated root of even multiplicity not cause a sign change on a polynomial sign chart?
A: Near a root $r$ of multiplicity $k$, the polynomial behaves like $c(x-r)^k$ times a factor that is nonzero and of constant sign nearby. If $k$ is even, $(x-r)^k\geq 0$ on both sides of $r$, so the polynomial does not change sign as $x$ crosses $r$; if $k$ is odd, $(x-r)^k$ changes sign at $r$, so the polynomial does too. This refinement is important when drawing the sign chart, because it tells you whether to flip the sign at a given critical point or not.

## 11.14 P:/S: Solve a quadratic inequality with sign chart

P: Solve $x^2-x-6\geq 0$ and express the answer in interval notation.

S: **IDENTIFY**: We have a quadratic inequality in the standard form "polynomial $\geq 0$", with expression $x^2-x-6$. The unknown is the real variable $x$; we want every real value making the expression non-negative.

**PLAN**: Factor the quadratic to find its real roots, which become the critical points of the sign chart. Partition the number line by these roots, test the sign of the factored expression on each subinterval, and select the intervals where the expression is $\geq 0$. Because the inequality is non-strict, include the roots themselves.

**EXECUTE**: Factor: $x^2-x-6=(x-3)(x+2)$, giving roots $x=-2$ and $x=3$. Mark these, producing intervals $(-\infty,-2)$, $(-2,3)$, and $(3,\infty)$. Test $x=-3$: $(-3-3)(-3+2)=(-)(-)=+$. Test $x=0$: $(0-3)(0+2)=(-)(+)=-$. Test $x=4$: $(4-3)(4+2)=(+)(+)=+$. The expression is $\geq 0$ on $(-\infty,-2)$ and $(3,\infty)$, plus the endpoints $-2$ and $3$ where it equals zero. Solution: $(-\infty,-2]\cup[3,\infty)$.

**EVALUATE**: Check a boundary: at $x=-2$, $(-2)^2-(-2)-6=4+2-6=0\geq 0$, so $-2$ correctly belongs. Check an interior point of the solution: $x=5$ gives $25-5-6=14\geq 0$. Check a point we excluded: $x=0$ gives $-6<0$, correctly outside. The square brackets reflect the non-strict $\geq$.

## 11.15 P:/S: Solve a rational inequality

P: Solve $\dfrac{x-1}{x+2}\geq 0$ and express the answer in interval notation.

S: **IDENTIFY**: We have a rational inequality of the form $N(x)/D(x)\geq 0$, with numerator $N(x)=x-1$ and denominator $D(x)=x+2$. The unknown is the real variable $x$, excluding any value that makes the denominator zero.

**PLAN**: Find the zeros of the numerator (candidates for inclusion) and the denominator (always excluded) to mark all sign-change points. Do not multiply through by $x+2$, since its sign depends on $x$ (11.12). Build a sign chart using both critical points, test each subinterval, and select the intervals where the quotient is $\geq 0$.

**EXECUTE**: Numerator zero: $x=1$. Denominator zero: $x=-2$ (excluded from the domain). Critical points divide the line into $(-\infty,-2)$, $(-2,1)$, and $(1,\infty)$. Test $x=-3$: $(-3-1)/(-3+2)=(-4)/(-1)=+$. Test $x=0$: $(0-1)/(0+2)=(-1)/2=-$. Test $x=2$: $(2-1)/(2+2)=1/4=+$. The quotient is $\geq 0$ on $(-\infty,-2)$ and $(1,\infty)$. We include $x=1$ (numerator zero makes the quotient exactly $0$, which satisfies $\geq$), but exclude $x=-2$ (undefined). Solution: $(-\infty,-2)\cup[1,\infty)$.

**EVALUATE**: At $x=1$: $0/3=0\geq 0$, correctly included. At $x=-2$: undefined, correctly excluded with a parenthesis. Spot-check $x=-10$: $(-11)/(-8)=11/8>0$, in the solution. Spot-check $x=0$: $-1/2<0$, correctly outside. The asymmetric brackets — parenthesis at $-2$, bracket at $1$ — reflect the distinction between denominator and numerator zeros.
