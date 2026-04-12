+++
order = 8
tags = ["math", "algebra", "functions", "domain", "range", "graphs", "transformations"]
+++

# Algebra — Functions and Their Graphs

## 8.1 What a Function Is

C: A [function] from a set $X$ to a set $Y$ is a rule that assigns to each element of $X$ exactly one element of $Y$.

Q: Why must a function assign *exactly one* output to each input?
A: Because this is what distinguishes functions from more general relations. "$y^2 = x$" is a relation but not a function, because for $x = 4$ both $y = 2$ and $y = -2$ satisfy it — a single input gives multiple outputs. Restricting to exactly-one-output per input makes functions predictable and composable, and is why calculus, differential equations, and virtually all of modern analysis are built on functions.

## 8.2 Function Notation

Q: What does $f(x)$ mean, and why use this notation?
A: $f(x)$ is read "$f$ of $x$" or "$f$ evaluated at $x$" — it denotes the output of the function $f$ when the input is $x$. This notation separates the *name* of the function ($f$) from the *input* ($x$) and makes it easy to talk about the function as an object ("the function $f$") and to plug in specific values ("$f(3) = 7$"). It scales cleanly to multiple functions: $g(x), h(x)$, etc.

## 8.3 Domain and Range

C: The [domain] of a function is the set of all inputs for which the function is defined; the [range] is the set of all values the function actually outputs.

Q: Why does the domain of $f(x) = 1/x$ exclude $x = 0$?
A: Because dividing by zero is undefined — there is no real number equal to $1/0$. For $f(x) = 1/x$ to have an output at every allowed input, we must remove $x = 0$ from the domain. The rest of the real line, $(-\infty, 0)\cup(0, \infty)$, is the natural domain. Domain restrictions arise from any operation that is undefined for some inputs: division by zero, even roots of negatives, logs of non-positive numbers, etc.

Q: What is the natural domain of $f(x) = \sqrt{x - 4}$?
A: $x\geq 4$, because the radicand must be non-negative for a real square root to exist. The natural domain consists of all inputs for which the formula produces a real number; it is $[4, \infty)$. The range, correspondingly, is $[0, \infty)$ — every non-negative real output is achieved. Determining the natural domain is a routine first step when analyzing any new function.

## 8.4 The Vertical Line Test

Q: What is the vertical line test, and why does it work?
A: A curve in the plane is the graph of a function (of $x$) if and only if no vertical line crosses it more than once. The reason: a vertical line at $x = a$ crosses the graph at the points $(a, y)$ where $y = f(a)$ — and a function must have exactly one $y$ for each $a$, so exactly one crossing per vertical line. Two crossings would mean two outputs for the same input, violating the function definition.

C: A curve in the plane is the graph of a function of $x$ if and only if every [vertical line] crosses it at most once.

## 8.5 Graphing Basic Functions

Q: What are the graphs of the most basic functions you should recognize instantly?
A: (1) Constant function $f(x) = c$ — a horizontal line at height $c$. (2) Linear $f(x) = mx + b$ — a straight line with slope $m$ and intercept $b$. (3) Quadratic $f(x) = x^2$ — a parabola opening upward with vertex at origin. (4) Absolute value $f(x) = |x|$ — a V shape with corner at origin. (5) Reciprocal $f(x) = 1/x$ — a hyperbola with asymptotes on both axes. (6) Square root $f(x) = \sqrt{x}$ — a half-parabola on its side starting at origin. (7) Cube root $f(x) = \sqrt[3]{x}$ — an S-shape through the origin.

## 8.6 Vertical and Horizontal Shifts

Q: How does the graph of $f(x) + c$ differ from the graph of $f(x)$?
A: Adding a constant $c$ to the function shifts the graph *vertically* by $c$ units — upward if $c > 0$, downward if $c < 0$. Every point $(x, y)$ on the original graph becomes $(x, y + c)$ on the new graph. For example, $y = x^2 + 3$ is the standard parabola shifted up 3 units.

Q: How does the graph of $f(x - h)$ differ from the graph of $f(x)$?
A: Subtracting $h$ from $x$ inside the function shifts the graph *horizontally* by $h$ units — to the right if $h > 0$, to the left if $h < 0$. The direction is "backwards" from what people expect: you'd think $f(x - 5)$ moves left, but it moves right. The reason: to get the same output, you need $x - 5$ to equal the original input, so the new $x$ must be 5 larger. Every point $(x, y)$ becomes $(x + h, y)$.

C: The graph of $f(x - h) + k$ is the graph of $f(x)$ shifted [$h$ units right and $k$ units up], with negative $h$ meaning left and negative $k$ meaning down.

## 8.7 Reflections and Stretches

Q: How do you recognize a vertical stretch, compression, or reflection from the formula?
A: Multiplying the function by a constant $a$ gives $af(x)$: (1) If $|a| > 1$, the graph is stretched vertically by factor $|a|$. (2) If $0 < |a| < 1$, it is compressed vertically by factor $|a|$. (3) If $a < 0$, it is also reflected across the $x$-axis. For example, $y = -2x^2$ is the standard parabola stretched by 2 and flipped upside down.

Q: How does $f(-x)$ differ from $f(x)$ graphically?
A: $f(-x)$ reflects the graph across the $y$-axis — every point $(x, y)$ goes to $(-x, y)$. For example, if $f(x) = \sqrt{x}$, then $f(-x) = \sqrt{-x}$ is defined for $x\leq 0$ and is the mirror image of the original through the vertical axis. Together with the vertical reflection $-f(x)$, these two reflections let you construct the rotated and mirrored variants of any basic function.

## 8.8 Even and Odd Functions

C: A function is [even] if $f(-x) = f(x)$ for every $x$ in its domain, and [odd] if $f(-x) = -f(x)$ for every $x$.

Q: What do the graphs of even and odd functions look like geometrically?
A: Even functions are symmetric about the $y$-axis — the left and right halves are mirror images. Odd functions are symmetric about the origin — rotating the graph 180° leaves it unchanged. Examples: $f(x) = x^2$ is even ($(-x)^2 = x^2$), $f(x) = x^3$ is odd, $f(x) = x^2 + x$ is neither. Recognizing symmetry can simplify integration, summation, and other calculations later.

## 8.9 Composition of Functions

C: The [composition] of two functions $f$ and $g$, written $(f\circ g)(x)$, is defined by $(f\circ g)(x) = f(g(x))$: apply $g$ first, then $f$ to the result.

Q: Is $f\circ g$ always the same as $g\circ f$?
A: No — function composition is generally not commutative. Example: $f(x) = x^2$ and $g(x) = x + 1$. Then $(f\circ g)(x) = (x + 1)^2$ but $(g\circ f)(x) = x^2 + 1$. These are different functions. The order matters because the "inner" function's output becomes the "outer" function's input, and squaring after adding one is not the same as adding one after squaring.

## 8.10 Inverse Functions

Q: What is the inverse of a function, and what condition must the original function satisfy for an inverse to exist?
A: The inverse $f^{-1}$ "undoes" $f$: $f^{-1}(f(x)) = x$ and $f(f^{-1}(y)) = y$. For an inverse to exist, $f$ must be *one-to-one* (injective): each output corresponds to exactly one input. A function that assigns the same output to two different inputs cannot be inverted, because $f^{-1}$ would have to return two different values for the same input — violating the function definition.

C: A function has an [inverse] if and only if it is one-to-one; graphically, this is captured by the [horizontal line test].

Q: How do you find $f^{-1}$ algebraically, given a formula for $f(x)$?
A: Replace $f(x)$ with $y$: $y = f(x)$. Solve for $x$ in terms of $y$: $x = g(y)$. Swap the roles: $f^{-1}(y) = g(y)$ (or rename the variable back to $x$). Example: $f(x) = 3x + 1$. Set $y = 3x + 1$, solve: $x = (y - 1)/3$. So $f^{-1}(x) = (x - 1)/3$. Verify: $f(f^{-1}(x)) = 3\cdot((x - 1)/3) + 1 = x - 1 + 1 = x$. ✓

## 8.11 Finding an Inverse — P:/S:

P: Given the function $f(x) = 2x - 5$, find its inverse $f^{-1}(x)$, verify the inverse property, and state the domain and range of both $f$ and $f^{-1}$.

S:
**IDENTIFY**: An inverse-function problem. Use the algebraic algorithm: swap $x$ and $y$, solve for the new $y$. Verify using $f\circ f^{-1} = \text{identity}$.

**PLAN**:
- Write $y = 2x - 5$.
- Solve for $x$: move the $-5$, then divide by 2.
- Rename variables to express $f^{-1}$ as a function of $x$.
- Verify $f(f^{-1}(x)) = x$ and $f^{-1}(f(x)) = x$.
- Determine the domain and range of both functions.

**EXECUTE**:
1. $y = 2x - 5$.
2. Add 5 to both sides: $y + 5 = 2x$.
3. Divide by 2: $x = (y + 5)/2$.
4. Rename: $f^{-1}(x) = (x + 5)/2$.
5. Verify $f(f^{-1}(x))$: $f((x + 5)/2) = 2\cdot(x + 5)/2 - 5 = x + 5 - 5 = x$. ✓
6. Verify $f^{-1}(f(x))$: $f^{-1}(2x - 5) = ((2x - 5) + 5)/2 = 2x/2 = x$. ✓
7. Domain of $f$: all real numbers, $(-\infty, \infty)$. Range of $f$: all real numbers. $f^{-1}$: same.

**EVALUATE**:
- Both composition checks give the identity, confirming $f^{-1}(x) = (x + 5)/2$ is correct.
- Slopes: $f$ has slope 2, $f^{-1}$ has slope $1/2$. Note the product: $2\cdot(1/2) = 1$, not $-1$. This is because $f$ and $f^{-1}$ are *not* perpendicular — they are *reflections of each other across the line $y = x$*. The slopes of a function and its inverse are reciprocals (not negative reciprocals).
- Graphically, the graph of $f^{-1}$ is the mirror image of the graph of $f$ across the line $y = x$. Every point $(a, b)$ on $y = f(x)$ corresponds to $(b, a)$ on $y = f^{-1}(x)$. You can use this to sketch $f^{-1}$ once you have $f$, without any algebra.
- The domain of $f^{-1}$ is the *range* of $f$, and vice versa. For linear functions with nonzero slope, both domain and range are all of $\mathbb{R}$, so this reversal is trivial. For more restricted functions like $f(x) = \sqrt{x}$ (domain $[0, \infty)$, range $[0, \infty)$), the symmetry is subtler: $f^{-1}(x) = x^2$, but restricted to $x\geq 0$ (not all real $x$, because $f^{-1}$'s domain must equal $f$'s range).
- This problem also highlights that inverses are a purely local concept for each function: every nontrivial function has its own rule, and computing $f^{-1}$ is a mechanical but careful procedure. Practice with linear, power, exponential, and logarithmic functions until it becomes routine — it will be needed constantly in later chapters.
