+++
order = 10
tags = ["math", "algebra", "radical-equations", "complex-numbers", "imaginary-unit", "conjugate"]
+++

# Algebra — Radical Equations and Complex Numbers

## 10.1 Why we need complex numbers

Q: Why do complex numbers exist — what problem do they solve?
A: Within the real numbers, the equation $x^2 = -1$ has no solution, because any real number squared is non-negative. Yet many natural equations — especially quadratics with negative discriminants — demand a solution. Adjoining a new symbol $i$ satisfying $i^2 = -1$ repairs this defect: the Fundamental Theorem of Algebra then guarantees that every non-constant polynomial has a root. Complex numbers are not a trick but the natural completion of the real numbers under polynomial operations.

Q: Why does a quadratic with a negative discriminant have no real solutions?
A: The quadratic formula gives $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$, where $a$, $b$, $c$ are the coefficients of $ax^2 + bx + c = 0$. If the discriminant $D = b^2 - 4ac$ is negative, then $\sqrt{D}$ is not a real number, since no real number squared yields a negative value. So the two roots predicted by the formula cannot live in $\mathbb{R}$; they require a wider number system.

C: A real quadratic $ax^2+bx+c=0$ has no real roots exactly when its discriminant $b^2-4ac$ is [negative].

## 10.2 The imaginary unit $i$

C: The [imaginary unit] $i$ is defined as the number satisfying $i^2 = -1$.

Q: Why is $i$ called "imaginary" even though it is a legitimate number?
A: The name is a historical artifact from the 16th–17th centuries, when mathematicians using $i$ to solve cubics distrusted it because it had no geometric interpretation on the real line. Today $i$ is as legitimate as any real number — it simply lives in a two-dimensional number system (the complex plane) rather than on a line. The label "imaginary" persists by convention, not because $i$ is fictitious.

C: By definition of $i$, we have $\sqrt{-1} = [i]$.

## 10.3 Powers of $i$

Q: Why do the powers of $i$ cycle through only four values?
A: Since $i^2 = -1$, we get $i^3 = i^2 \cdot i = -i$ and $i^4 = (i^2)^2 = (-1)^2 = 1$. Once we reach $i^4 = 1$, multiplying by $i$ again restarts the sequence: $i^5 = i$, $i^6 = -1$, and so on. So the pattern repeats with period $4$.

C: The powers of $i$ cycle as $i^1 = i$, $i^2 = -1$, $i^3 = -i$, and $i^4 = [1]$.

C: To evaluate $i^n$ for a positive integer $n$, reduce $n$ modulo [4] and use the cycle $\{i, -1, -i, 1\}$.

Q: What is $i^{27}$?
A: Reduce the exponent modulo $4$: $27 = 4(6) + 3$, so $i^{27} = i^3 = -i$.

## 10.4 Standard form

C: A [complex number] written in standard form is $a + bi$, where $a$ and $b$ are real numbers and $i$ is the imaginary unit.

Q: Why insist on the standard form $a+bi$ for complex numbers?
A: Standard form makes complex numbers into an ordered pair of real numbers $(a,b)$, which (1) gives a unique representation for every complex number, (2) lets us add, subtract, and multiply by handling real and imaginary parts independently, and (3) matches the geometric picture of the complex plane with horizontal axis $a$ and vertical axis $b$.

C: A real number $a$ is the special case $a + [0]i$ of a complex number.

C: A pure [imaginary] number is a complex number of the form $0 + bi$ with $b \neq 0$.

## 10.5 Real and imaginary parts

C: For a complex number $z = a + bi$ with $a, b \in \mathbb{R}$, the real part is $\operatorname{Re}(z) = [a]$.

C: For a complex number $z = a + bi$ with $a, b \in \mathbb{R}$, the imaginary part is $\operatorname{Im}(z) = [b]$.

Q: Why is $\operatorname{Im}(a+bi) = b$ rather than $bi$?
A: By convention, the imaginary part is the real coefficient of $i$, not the imaginary term itself. This keeps both $\operatorname{Re}(z)$ and $\operatorname{Im}(z)$ as real numbers, which is essential because we want to treat $z \leftrightarrow (\operatorname{Re}(z), \operatorname{Im}(z))$ as an ordered pair of reals — the point representing $z$ in the complex plane.

Q: When are two complex numbers $a+bi$ and $c+di$ equal?
A: Exactly when $a = c$ and $b = d$ — that is, when their real parts agree and their imaginary parts agree. A single complex equation in standard form is therefore equivalent to two real equations.

## 10.6 Addition and subtraction

Q: Why do we add complex numbers componentwise?
A: Treating $i$ as a symbol that commutes with real numbers, $(a+bi)+(c+di) = a + c + bi + di = (a+c) + (b+d)i$, where $a, b, c, d$ are real. The real parts combine and the imaginary parts combine, just as vector addition combines $x$-components and $y$-components independently.

C: Addition: $(a+bi) + (c+di) = [(a+c) + (b+d)i]$, where $a,b,c,d$ are real numbers.

C: Subtraction: $(a+bi) - (c+di) = [(a-c) + (b-d)i]$, where $a,b,c,d$ are real numbers.

Q: Compute $(3 + 5i) + (-4 + 2i)$.
A: Add real parts: $3 + (-4) = -1$. Add imaginary parts: $5 + 2 = 7$. Result: $-1 + 7i$.

## 10.7 Multiplication

Q: Why does FOIL plus $i^2 = -1$ suffice to multiply complex numbers?
A: A complex number $a+bi$ is a binomial in the symbol $i$, so FOIL applies: $(a+bi)(c+di) = ac + adi + bci + bd\,i^2$, where $a,b,c,d$ are real. The first three terms are ordinary polynomial algebra; the last uses the sole new rule $i^2 = -1$ to turn $bd\,i^2$ into $-bd$. Grouping real and imaginary parts gives the product in standard form.

C: Multiplication formula: $(a+bi)(c+di) = [(ac-bd) + (ad+bc)i]$, where $a,b,c,d$ are real numbers.

Q: Compute $(2 + 3i)(4 - i)$.
A: FOIL: $2 \cdot 4 + 2 \cdot (-i) + 3i \cdot 4 + 3i \cdot (-i) = 8 - 2i + 12i - 3i^2$. Substitute $i^2 = -1$: $-3i^2 = 3$. Combine: $(8+3) + (-2+12)i = 11 + 10i$.

## 10.8 Complex conjugate

C: The [complex conjugate] of $z = a+bi$ is $\bar{z} = a - bi$, obtained by negating the imaginary part.

Q: Why is the conjugate useful — what property does $z\bar{z}$ have?
A: For $z = a+bi$ with $a,b$ real, $z\bar{z} = (a+bi)(a-bi) = a^2 - (bi)^2 = a^2 - b^2 i^2 = a^2 + b^2$. The product of a complex number with its conjugate is always a non-negative real number. This is the key fact that lets us "clear" $i$ from denominators, in direct analogy to rationalizing a radical denominator using conjugates.

C: For any complex $z = a+bi$ with $a,b$ real, $z\bar{z} = [a^2 + b^2]$, which is always real and non-negative.

Q: What is the conjugate of $5 - 7i$?
A: $\overline{5 - 7i} = 5 + 7i$. The real part stays the same; the sign of the imaginary part flips.

## 10.9 Division

Q: Why do we multiply numerator and denominator by the conjugate when dividing complex numbers?
A: We want to write $\frac{a+bi}{c+di}$ in standard form $x+yi$ with $x, y$ real. Multiplying top and bottom by the conjugate $c - di$ produces a denominator of $c^2 + d^2$, which is a real number, and a numerator that is an ordinary complex product. This is exactly the same trick as rationalizing $\frac{1}{\sqrt{2}+1}$ by the conjugate $\sqrt{2} - 1$ — we clear the unwanted symbol from the denominator.

C: To divide complex numbers, multiply numerator and denominator by the [conjugate] of the denominator.

C: Division formula: $\dfrac{a+bi}{c+di} = \dfrac{(ac+bd) + (bc-ad)i}{[c^2 + d^2]}$, where $a,b,c,d$ are real and $c+di \neq 0$.

Q: Compute $\dfrac{3+2i}{1+i}$.
A: Multiply top and bottom by $\overline{1+i} = 1-i$: numerator $(3+2i)(1-i) = 3 - 3i + 2i - 2i^2 = 3 - i + 2 = 5 - i$; denominator $(1+i)(1-i) = 1 + 1 = 2$. Result: $\frac{5-i}{2} = \frac{5}{2} - \frac{1}{2}i$.

## 10.10 Modulus

C: The [modulus] of a complex number $z = a+bi$ is $|z| = \sqrt{a^2 + b^2}$, where $a = \operatorname{Re}(z)$ and $b = \operatorname{Im}(z)$.

Q: Why is the modulus defined as $\sqrt{a^2+b^2}$?
A: Identifying $z = a+bi$ with the point $(a,b)$ in the complex plane, $|z|$ is the Euclidean distance from $z$ to the origin. By the Pythagorean theorem applied to the right triangle with legs $a$ and $b$, that distance is $\sqrt{a^2+b^2}$. So the modulus is the natural generalization of absolute value: for real $z = a + 0i$, $|z| = \sqrt{a^2} = |a|$.

C: The modulus relates to the conjugate via $|z|^2 = [z\bar{z}]$, which is how we recover real magnitude from complex multiplication.

Q: What is $|3 - 4i|$?
A: $|3-4i| = \sqrt{3^2 + (-4)^2} = \sqrt{9 + 16} = \sqrt{25} = 5$.

## 10.11 Solving radical equations

C: A [radical equation] is an equation in which the unknown appears under a radical sign, such as $\sqrt{x+1} = 3$.

Q: What is the standard strategy for solving a radical equation?
A: (1) Isolate one radical on one side of the equation. (2) Raise both sides to the power equal to the index of the radical (square both sides for a square root) to eliminate it. (3) Solve the resulting polynomial equation. (4) Check every candidate in the original equation, because squaring can introduce extraneous solutions.

C: To eliminate a square root $\sqrt{f(x)}$, isolate it on one side and [square] both sides of the equation.

Q: Solve $\sqrt{x+1} = 3$.
A: Square both sides: $x+1 = 9$, so $x = 8$. Check: $\sqrt{8+1} = \sqrt{9} = 3$. Valid.

## 10.12 Extraneous solutions

Q: Why can squaring both sides of an equation introduce extraneous solutions?
A: Squaring is not a reversible operation: different numbers can share a square. Concretely, $a = b$ implies $a^2 = b^2$, but $a^2 = b^2$ only implies $a = \pm b$. So squaring $\sqrt{f(x)} = g(x)$ produces the combined equation $f(x) = g(x)^2$, which also contains the solutions of $\sqrt{f(x)} = -g(x)$. Roots introduced by that second equation do not satisfy the original and must be rejected.

C: A solution that appears after squaring but fails the original equation is called an [extraneous] solution.

C: Because $\sqrt{\ }$ always returns a non-negative value, any candidate making the isolated radical side [negative] must be rejected.

Q: Show that $\sqrt{x} = -2$ has no solution and explain why squaring suggests one.
A: $\sqrt{x}$ is non-negative for all real $x \geq 0$, so it can never equal $-2$. Squaring gives $x = 4$, which is a solution of $\sqrt{x} = 2$, not of $\sqrt{x} = -2$. Checking $x = 4$ in the original equation gives $\sqrt{4} = 2 \neq -2$, so $x = 4$ is extraneous.

## 10.13 Equations with two radicals

Q: How do you solve an equation with two square roots, such as $\sqrt{x+5} - \sqrt{x} = 1$?
A: Isolate one radical, square both sides, then isolate the remaining radical and square again. Squaring once will usually leave a single radical in a simpler equation; the second squaring eliminates it. After reaching a polynomial, solve it and check every candidate in the original equation, because each squaring step can introduce extraneous solutions.

C: For an equation with two radicals, you must isolate and square [twice] (or as many times as there are radicals).

Q: Solve $\sqrt{x+5} - \sqrt{x} = 1$.
A: Rewrite as $\sqrt{x+5} = 1 + \sqrt{x}$ and square: $x+5 = 1 + 2\sqrt{x} + x$, giving $4 = 2\sqrt{x}$, so $\sqrt{x} = 2$. Square again: $x = 4$. Check: $\sqrt{9} - \sqrt{4} = 3 - 2 = 1$. Valid.

## 10.14 Solving $x^2 = -k$ over $\mathbb{C}$

Q: How do you solve $x^2 = -k$ for $k > 0$ using complex numbers?
A: Write $-k = k \cdot (-1)$, so $x^2 = -k$ becomes $x^2 = -1 \cdot k$. Taking square roots, $x = \pm\sqrt{-1}\cdot\sqrt{k} = \pm i\sqrt{k}$. The equation always has exactly two complex solutions — a conjugate pair $\pm i\sqrt{k}$ — because squaring either one yields $i^2 k = -k$.

C: For $k > 0$, the equation $x^2 = -k$ has complex solutions $x = [\pm i\sqrt{k}]$.

Q: Solve $x^2 + 9 = 0$.
A: Rearrange to $x^2 = -9$. Then $x = \pm i\sqrt{9} = \pm 3i$. Check: $(3i)^2 + 9 = 9i^2 + 9 = -9 + 9 = 0$.

Q: Solve $x^2 - 2x + 5 = 0$ using the quadratic formula.
A: With $a=1$, $b=-2$, $c=5$, the discriminant is $b^2 - 4ac = 4 - 20 = -16$. So $x = \frac{2 \pm \sqrt{-16}}{2} = \frac{2 \pm 4i}{2} = 1 \pm 2i$. The two complex roots form a conjugate pair, as expected for a real quadratic with negative discriminant.

## 10.15 P:/S: Radical equation with extraneous-solution check

P: Solve $\sqrt{2x + 7} = x + 2$ for $x$, checking all candidate solutions.

S:
**IDENTIFY**: Radical equation with one square root on the left and a linear expression on the right. We must square to eliminate the radical and then check for extraneous solutions because the right-hand side can be negative.

**PLAN**:
- Confirm the radical is already isolated.
- Square both sides to obtain a quadratic in $x$.
- Solve the quadratic.
- Substitute each candidate back into the original equation to verify.

**EXECUTE**:
1. The radical is isolated: $\sqrt{2x+7} = x+2$.
2. Square both sides: $2x + 7 = (x+2)^2 = x^2 + 4x + 4$.
3. Rearrange: $0 = x^2 + 4x + 4 - 2x - 7 = x^2 + 2x - 3$.
4. Factor: $x^2 + 2x - 3 = (x+3)(x-1) = 0$, giving candidates $x = -3$ and $x = 1$.
5. Check $x = 1$: LHS $= \sqrt{2(1)+7} = \sqrt{9} = 3$; RHS $= 1 + 2 = 3$. Valid.
6. Check $x = -3$: LHS $= \sqrt{2(-3)+7} = \sqrt{1} = 1$; RHS $= -3 + 2 = -1$. Since $1 \neq -1$, $x = -3$ is extraneous.

**EVALUATE**: Only $x = 1$ is a solution. The extraneous root $x = -3$ appeared because squaring also solves $\sqrt{2x+7} = -(x+2)$, and $x = -3$ satisfies that sign-flipped equation. Always checking in the original equation catches this.

## 10.16 P:/S: Complex arithmetic — multiply and divide

P: Let $z_1 = 2 + 3i$ and $z_2 = 1 - 2i$. Compute $z_1 z_2$ and $\dfrac{z_1}{z_2}$, giving both results in standard form $a + bi$.

S:
**IDENTIFY**: Complex multiplication (FOIL plus $i^2 = -1$) and complex division (multiply by the conjugate of the denominator).

**PLAN**:
- For the product, expand $(2+3i)(1-2i)$ using FOIL and simplify $i^2 = -1$.
- For the quotient, multiply numerator and denominator by $\overline{z_2} = 1 + 2i$, then divide by the resulting real denominator $|z_2|^2 = 1^2 + 2^2 = 5$.

**EXECUTE**:
1. Product: $(2+3i)(1-2i) = 2 - 4i + 3i - 6i^2 = 2 - i - 6(-1) = 2 - i + 6 = 8 - i$.
2. Quotient, multiply by conjugate: $\dfrac{2+3i}{1-2i} \cdot \dfrac{1+2i}{1+2i} = \dfrac{(2+3i)(1+2i)}{(1-2i)(1+2i)}$.
3. Numerator: $(2+3i)(1+2i) = 2 + 4i + 3i + 6i^2 = 2 + 7i - 6 = -4 + 7i$.
4. Denominator: $(1-2i)(1+2i) = 1^2 + 2^2 = 5$.
5. Quotient: $\dfrac{-4 + 7i}{5} = -\dfrac{4}{5} + \dfrac{7}{5}i$.

**EVALUATE**: Both results are in standard form $a+bi$ with real $a$ and $b$, as required. Sanity check: $|z_1 z_2| = |z_1||z_2| = \sqrt{13}\cdot\sqrt{5} = \sqrt{65}$, and $|8-i| = \sqrt{64+1} = \sqrt{65}$. Consistent, so the product is correct.
