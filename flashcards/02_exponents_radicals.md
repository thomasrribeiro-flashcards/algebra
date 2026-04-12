+++
order = 2
tags = ["math", "algebra", "exponents", "radicals", "powers", "scientific-notation"]
+++

# Algebra — Exponents and Radicals

## 2.1 Integer Exponents

C: For a real number $a$ and a positive integer $n$, the expression $a^n$ means $a$ multiplied by itself $n$ times: $a^n = [a\cdot a\cdots a]$ ($n$ factors).

Q: Why define $a^0 = 1$ for $a\neq 0$?
A: Because the rule $a^m\cdot a^n = a^{m+n}$ should continue to hold when $n = 0$: $a^m\cdot a^0 = a^{m+0} = a^m$, which forces $a^0 = 1$. It is not an arbitrary convention but the *only* value that preserves the exponent-addition rule. $0^0$ is left undefined (or sometimes defined as 1 in combinatorial contexts) because no consistent value works for all rules.

Q: Why define $a^{-n} = 1/a^n$ for $a\neq 0$?
A: Because the same rule $a^m\cdot a^n = a^{m+n}$ requires $a^{-n}\cdot a^n = a^0 = 1$, which forces $a^{-n} = 1/a^n$. Again, this extension is dictated by consistency with the multiplicative rule, not chosen arbitrarily. Negative exponents are not a separate concept — they are forced by requiring the exponent rules to hold for all integers.

C: $a^{-n} = [1/a^n]$ for $a\neq 0$ — a definition dictated by the exponent-addition rule $a^m\cdot a^n = a^{m+n}$.

## 2.2 Rules for Exponents

Q: What are the five basic exponent rules for integer exponents?
A: (1) $a^m\cdot a^n = a^{m+n}$ (product rule). (2) $a^m/a^n = a^{m-n}$ (quotient rule, $a\neq 0$). (3) $(a^m)^n = a^{mn}$ (power rule). (4) $(ab)^n = a^n b^n$ (product-to-power rule). (5) $(a/b)^n = a^n/b^n$ (quotient-to-power rule, $b\neq 0$). Every algebraic manipulation involving powers ultimately relies on these five rules.

C: The exponent product rule is $a^m\cdot a^n = [a^{m+n}]$, and the power rule is $(a^m)^n = a^{mn}$.

## 2.3 Square Roots

C: The [principal square root] of a non-negative real number $a$ is the non-negative number $\sqrt{a}$ satisfying $(\sqrt{a})^2 = a$.

Q: Why is $\sqrt{a}$ defined to be non-negative when $a > 0$ has *two* square roots?
A: Because a function must produce exactly one output for each input, and the equation $x^2 = a$ has two solutions ($\pm\sqrt{a}$). To make $\sqrt{\cdot}$ a single-valued function, we conventionally pick the non-negative root. Both roots can be recovered by writing $\pm\sqrt{a}$ when needed. This convention is what makes $\sqrt{4} = 2$ rather than $\pm 2$.

Q: Why is $\sqrt{a^2} = |a|$ rather than $\sqrt{a^2} = a$?
A: Because the principal square root is non-negative by definition, so $\sqrt{a^2}$ must also be non-negative. If $a\geq 0$, then $|a| = a$; if $a < 0$, then $|a| = -a > 0$. Writing $\sqrt{a^2} = a$ would give a negative answer for negative $a$, contradicting the non-negativity of the principal root. This is a subtle but important point — forgetting the absolute value is a common source of sign errors.

C: For any real $a$, $\sqrt{a^2} = [|a|]$ — the absolute value, not $a$ itself, because the principal square root is always non-negative.

## 2.4 $n$-th Roots

C: The [$n$-th root] of a real number $a$, written $\sqrt[n]{a}$, is a number whose $n$-th power equals $a$; when $n$ is odd, it exists for every real $a$, when $n$ is even, it requires $a\geq 0$.

Q: Why does $\sqrt[n]{a}$ require $a\geq 0$ when $n$ is even but allow $a < 0$ when $n$ is odd?
A: Because an even power of a real number is always non-negative ($x^2, x^4,\dots\geq 0$), so no real $x$ satisfies $x^4 = -16$, for example. Odd powers, however, preserve sign: $(-2)^3 = -8$, so $\sqrt[3]{-8} = -2$ is a perfectly good real number. The existence of real $n$-th roots depends on the parity of $n$ — a distinction that vanishes when we later extend to complex numbers.

## 2.5 Rational Exponents

C: For $a > 0$ and $m, n$ integers with $n > 0$, the [rational exponent] is defined as $a^{m/n} = \sqrt[n]{a^m} = (\sqrt[n]{a})^m$.

Q: Why must rational exponents satisfy $a^{m/n} = \sqrt[n]{a^m}$?
A: Because the exponent rules force this definition: if we want $(a^{m/n})^n = a^m$, then $a^{m/n}$ must be an $n$-th root of $a^m$. So the fractional exponent is an encoding of "take an $n$-th root and raise to the $m$-th power," or equivalently in either order. This makes the exponent rules hold for all rational exponents, extending them smoothly beyond integers.

Q: Why is care needed with $a^{m/n}$ when $a < 0$?
A: Because $\sqrt[n]{a}$ may not exist for even $n$ when $a < 0$, and even when it does, $a^{m/n}$ may give inconsistent values if $m/n$ can be written in multiple reduced forms. For instance, $(-8)^{2/6}$ is not straightforwardly computable: $(-8)^{1/6}$ is not a real number, but $(-8)^{1/3} = -2$ gives $((-8)^{1/3})^2 = 4$. These ambiguities are why rational exponents are usually restricted to $a > 0$ in algebra.

## 2.6 Simplifying Radical Expressions

Q: Why is $\sqrt{ab} = \sqrt{a}\sqrt{b}$ for $a, b\geq 0$, and why does this fail for negative values?
A: For non-negative $a, b$, both sides are non-negative, and squaring either gives $ab$ — so they are equal by the uniqueness of the principal square root. For negative values, the identity fails: e.g., $\sqrt{(-1)(-1)} = \sqrt{1} = 1$, but $\sqrt{-1}\cdot\sqrt{-1} = i\cdot i = -1$. Keeping to non-negative arguments is essential when working with real radicals.

C: For $a, b\geq 0$, $\sqrt{ab} = [\sqrt{a}\sqrt{b}]$; this identity fails if either $a$ or $b$ is negative because the real square root is undefined there.

## 2.7 Rationalizing Denominators

Q: Why is it standard practice to "rationalize the denominator" of expressions like $1/\sqrt{2}$?
A: Historically, it made manual numerical computations easier: dividing by an irrational was cumbersome, so people multiplied top and bottom by $\sqrt{2}$ to write $1/\sqrt{2} = \sqrt{2}/2$ — a form that could be evaluated by dividing a known decimal by 2. In modern algebra, rationalizing serves more as a canonical-form convention: it makes expressions easier to compare, and it reveals cancellations that would be hidden in a raw radical denominator.

## 2.8 Scientific Notation

C: [Scientific notation] writes a real number as $a\times 10^n$, where $1\leq|a| < 10$ and $n$ is an integer, giving a compact representation for very large or very small magnitudes.

Q: Why is scientific notation preferred for numbers like $299792458$ or $0.000000001$?
A: Because it separates the magnitude (the power of 10) from the significant digits (the mantissa $a$), making the scale obvious at a glance and minimizing the number of zeros you have to count. $299792458 = 2.99792458\times 10^8$ clearly shows the magnitude as "hundreds of millions," while writing out every digit does not. In physics, engineering, and science generally, it is the standard way to write any number whose magnitude is far from 1.

## 2.9 Rational Exponent Calculation — P:/S:

P: Simplify $\dfrac{(x^3 y^{-2})^2 \cdot (x^{-1} y^3)}{x^2 y^{-1}}$, expressing the answer with positive exponents only. Assume $x, y > 0$.

S:
**IDENTIFY**: An exponent-simplification problem. Use the product, quotient, and power rules to combine and reduce.

**PLAN**:
- Expand $(x^3 y^{-2})^2$ using the power rule: each inner exponent multiplies by 2.
- Multiply the numerator factors using the product rule: add exponents of like bases.
- Divide by the denominator using the quotient rule: subtract exponents of like bases.
- Convert any negative exponents to positive by moving bases across the fraction bar.

**EXECUTE**:
1. $(x^3 y^{-2})^2 = x^{3\cdot 2} y^{-2\cdot 2} = x^6 y^{-4}$.
2. Numerator: $x^6 y^{-4}\cdot x^{-1} y^3 = x^{6 + (-1)} y^{-4 + 3} = x^5 y^{-1}$.
3. Full fraction: $\dfrac{x^5 y^{-1}}{x^2 y^{-1}} = x^{5 - 2}\,y^{-1 - (-1)} = x^3 y^0 = x^3$.
4. The $y$ exponent is zero, so the $y$ drops out entirely.
5. Final answer: $x^3$.

**EVALUATE**:
- Start-to-finish, an unruly-looking expression reduced to just $x^3$. The $y$ terms cancelled exactly, which is the payoff for keeping careful track of exponents: the simplification is guaranteed by the rules, not by guessing.
- Sanity check with a numerical example: let $x = 2, y = 5$. Numerator: $(2^3\cdot 5^{-2})^2\cdot 2^{-1}\cdot 5^3 = (8/25)^2\cdot(1/2)\cdot 125 = (64/625)\cdot(125/2) = 64\cdot 125/(625\cdot 2) = 8000/1250 = 6.4$. Denominator: $2^2\cdot 5^{-1} = 4/5 = 0.8$. Quotient: $6.4/0.8 = 8 = 2^3 = x^3$. ✓
- The pattern of "expand powers → combine like bases → cancel" is the universal strategy for any expression involving only powers and products/quotients. More complicated expressions (with sums, radicals, etc.) may require additional steps, but the exponent bookkeeping is always the same.
- Negative exponents are notationally convenient in intermediate steps — they let you treat division as multiplication with a negative exponent, avoiding constant re-arrangement of fractions. Converting to positive exponents is a final cleanup step, not something you do every line.
- As expressions grow more complex in later chapters (polynomials, rational functions, radicals mixed with exponents), the ability to handle exponent arithmetic without error is the bottleneck. Practicing it on worked examples like this one is time well spent.
