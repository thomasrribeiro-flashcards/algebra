+++
order = 5
tags = ["math", "algebra", "linear-equations", "inequalities", "lines", "slope"]
+++

# Algebra — Linear Equations and Inequalities

## 5.1 What a Linear Equation Is

C: A [linear equation] in one variable is an equation that can be written in the form $ax + b = 0$, where $a$ and $b$ are constants and $a\neq 0$.

Q: Why is the condition $a\neq 0$ part of the definition of a linear equation?
A: Because if $a = 0$, the equation collapses to $b = 0$, which is either always true (if $b = 0$) or never true (if $b\neq 0$) — a statement, not an equation to solve for $x$. The defining feature of a linear equation is that it has a unique solution $x = -b/a$, which requires $a\neq 0$. Without this condition, the equation would cease to be about $x$ at all.

## 5.2 Solving a Linear Equation

Q: What is the standard procedure for solving $ax + b = c$?
A: Isolate $x$ by reversing operations: subtract $b$, then divide by $a$, giving $x = (c - b)/a$. The "peel from the outside in" idea extends to more complex equations.

C: To solve $ax + b = c$, subtract $b$ from both sides and then divide by $a$, giving $x = [(c - b)/a]$.

## 5.3 Equations With the Variable on Both Sides

Q: How do you solve a linear equation that has the variable on both sides, like $3x + 7 = 5x - 1$?
A: Move all $x$-terms to one side and all constants to the other, then solve as usual. For example, $3x + 7 = 5x - 1\Rightarrow 7 + 1 = 5x - 3x\Rightarrow 8 = 2x\Rightarrow x = 4$. The key step is "collecting like terms" on each side of the equation — grouping the variable terms together and the constants together.

## 5.4 Equations with Fractions

Q: How do you handle a linear equation that contains fractions, like $(x/2) + (x/3) = 5$?
A: Multiply both sides by the least common denominator (LCD) to clear the fractions. Here, LCD = 6: $6\cdot(x/2) + 6\cdot(x/3) = 6\cdot 5\Rightarrow 3x + 2x = 30\Rightarrow 5x = 30\Rightarrow x = 6$. Clearing fractions at the beginning keeps the calculation manageable — working with fractions throughout is error-prone and slower.

## 5.5 Linear Inequalities

C: A [linear inequality] in one variable is an expression like $ax + b < c$ (or $\leq, >, \geq$), whose solution set is a range of values rather than a single point.

Q: Why does the inequality sign flip when you multiply or divide both sides by a negative number?
A: Because multiplying by a negative reverses the order of the real line: if $a < b$, then $-a > -b$ (think: $2 < 3$, but $-2 > -3$). This isn't a weird rule — it's a consequence of how negation acts on order. When you multiply both sides of an inequality by $-1$, the direction of "less than" becomes "greater than," and vice versa. Forgetting to flip the sign when dividing by a negative is one of the most common inequality mistakes.

C: When you multiply or divide both sides of an inequality by a [negative number], the inequality sign must flip direction.

## 5.6 Compound Inequalities

Q: What is a compound inequality, and how do you solve one like $-3 < 2x + 1 < 7$?
A: A compound inequality is two inequalities combined into one expression, describing a bounded range. Solve by applying the same operation to *all three parts* simultaneously: $-3 - 1 < 2x < 7 - 1\Rightarrow -4 < 2x < 6\Rightarrow -2 < x < 3$. The solution set is the interval $(-2, 3)$. The same approach works for any "$a < f(x) < b$"-style expression.

## 5.7 Absolute Value Inequalities

Q: How do you solve an absolute-value inequality like $|x - 2| < 5$?
A: Recognize that $|x - 2|$ is the distance from $x$ to $2$. The inequality says this distance is less than 5, so $x$ is within 5 units of 2: $-5 < x - 2 < 5$, i.e., $-3 < x < 7$. For $|x - 2| > 5$, the distance exceeds 5, so $x < -3$ or $x > 7$ (two unbounded pieces). The geometric "distance" interpretation from chapter 1 makes these inequalities natural rather than mysterious.

## 5.8 Lines in the Plane

C: A [line] in the coordinate plane is the graph of a linear equation in two variables, typically written in the form $y = mx + b$ (slope-intercept form) or $ax + by = c$ (standard form).

Q: What is the slope of a line, and how do you compute it from two points?
A: The slope $m$ is the ratio of vertical change to horizontal change — "rise over run" — as you move along the line: $m = (y_2 - y_1)/(x_2 - x_1)$ for any two distinct points $(x_1, y_1)$ and $(x_2, y_2)$. It measures how steeply the line rises or falls and is a single constant for any given line. Slopes are positive for lines going up-right, negative for down-right, zero for horizontal, and undefined for vertical lines.

C: The [slope] of a line through two points $(x_1, y_1)$ and $(x_2, y_2)$ is $m = (y_2 - y_1)/(x_2 - x_1)$, provided $x_1\neq x_2$.

## 5.9 Slope-Intercept Form

C: The [slope-intercept form] of a line is $y = mx + b$, where $m$ is the slope and $b$ is the $y$-intercept (the $y$-value where the line crosses the $y$-axis).

Q: Why is $y = mx + b$ called "slope-intercept form"?
A: Because the two defining parameters — the slope $m$ and the $y$-intercept $b$ — appear directly as coefficients in the equation. You can read them off immediately: $y = 3x - 7$ has slope $3$ and $y$-intercept $-7$. This form is the most useful for graphing (start at $(0, b)$, move with slope $m$) and for comparing lines (parallel lines have the same $m$).

## 5.10 Point-Slope Form

C: The [point-slope form] of a line is $y - y_1 = m(x - x_1)$, where $(x_1, y_1)$ is any point on the line and $m$ is the slope.

Q: When is point-slope form the most convenient way to write a line's equation?
A: When you are given a point and a slope, or two points (from which you can compute a slope). For example, "line through $(2, 5)$ with slope $3$" becomes $y - 5 = 3(x - 2)$ directly, without any algebra. Point-slope form is the natural "input format" for problems that specify a line geometrically; converting to slope-intercept form is often a second step.

## 5.11 Parallel and Perpendicular Lines

Q: How can you tell whether two lines are parallel or perpendicular from their slopes?
A: Two lines are *parallel* iff they have the same slope ($m_1 = m_2$) and are distinct (different $y$-intercepts). They are *perpendicular* iff their slopes multiply to $-1$ ($m_1 m_2 = -1$), equivalently $m_2 = -1/m_1$. Horizontal and vertical lines are a special case: horizontal has slope 0, vertical has undefined slope, and they are perpendicular to each other even though the $m_1 m_2 = -1$ rule doesn't directly apply.

C: Two non-vertical lines are [perpendicular] if and only if their slopes satisfy $m_1 m_2 = -1$.

## 5.12 Finding a Line Through Two Points — P:/S:

P: Find the equation of the line passing through the points $(1, 4)$ and $(3, 10)$. Express the answer in slope-intercept form $y = mx + b$.

S:
**IDENTIFY**: A line-finding problem given two points. Use the slope formula first, then the point-slope form (or plug into slope-intercept form).

**PLAN**:
- Compute the slope $m$ using $m = (y_2 - y_1)/(x_2 - x_1)$.
- Use point-slope form with one of the given points to write $y - y_1 = m(x - x_1)$.
- Rearrange to $y = mx + b$.
- Verify by plugging the other point into the result.

**EXECUTE**:
1. Slope: $m = (10 - 4)/(3 - 1) = 6/2 = 3$.
2. Point-slope form using $(1, 4)$: $y - 4 = 3(x - 1)$.
3. Expand: $y - 4 = 3x - 3$.
4. Add 4 to both sides: $y = 3x + 1$.
5. $y$-intercept is $b = 1$.

**EVALUATE**:
- Check $(1, 4)$: $y = 3(1) + 1 = 4$ ✓; check $(3, 10)$: $y = 3(3) + 1 = 10$ ✓.
- Either given point works in point-slope form; the result is the same.
- Vertical lines ($x_1 = x_2$) are the only edge case: slope is undefined, write $x = x_1$.

Q: You're given two points and asked for a line equation. What's the procedure?
A: Slope $m = \Delta y / \Delta x$, then point-slope $y - y_1 = m(x - x_1)$, then rearrange.
