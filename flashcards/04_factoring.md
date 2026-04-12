+++
order = 4
tags = ["math", "algebra", "factoring", "polynomials", "gcf", "grouping", "quadratic-factoring"]
+++

# Algebra — Factoring Polynomials

## 4.1 Why Factor

Q: What does it mean to "factor" a polynomial, and why is factoring useful?
A: Factoring means rewriting a polynomial as a product of simpler polynomials (its factors), ideally so that each factor cannot be broken down further (over the reals or rationals). Factoring is useful because it turns many problems into trivial ones: finding the zeros of $(x - 2)(x - 3)$ is obvious, but finding the zeros of $x^2 - 5x + 6$ is less so until you factor it. Factoring is the reverse of the multiplication you learned in chapter 3 — and it is much harder.

## 4.2 Greatest Common Factor

Q: What is the greatest common factor (GCF) of a polynomial's terms, and why is it always the first factoring step to try?
A: The GCF is the largest monomial (including constants) that divides every term of the polynomial. For example, in $6x^3 - 9x^2 + 12x$, the GCF is $3x$, and factoring gives $3x(2x^2 - 3x + 4)$. Extracting the GCF is always the first step because it simplifies what remains — often making subsequent factoring techniques applicable that weren't before.

C: The first step in factoring any polynomial is extracting the [greatest common factor] of its terms.

## 4.3 Factoring by Grouping

Q: When can you factor a polynomial by grouping?
A: When the polynomial has four or more terms that can be split into groups, each sharing a common factor, and the grouped factors combine into a further common factor. For example, $x^3 + 2x^2 + 3x + 6 = x^2(x + 2) + 3(x + 2) = (x^2 + 3)(x + 2)$. Grouping succeeds when the "paired" common factor (here, $(x + 2)$) appears in both groups; if not, rearranging the terms or a different grouping may work.

## 4.4 Recognizing Difference of Squares

Q: How do you recognize and factor a difference of squares?
A: Look for $a^2 - b^2$ — two terms, one positive and one negative, both perfect squares. Factor as $(a + b)(a - b)$. For example, $x^2 - 9 = (x + 3)(x - 3)$, $4y^2 - 25 = (2y + 5)(2y - 5)$, and $x^4 - 16 = (x^2 + 4)(x^2 - 4) = (x^2 + 4)(x + 2)(x - 2)$. The pattern extends recursively — after one application, the result itself may be factorable.

C: The [difference of squares] $a^2 - b^2$ factors as $(a + b)(a - b)$; this is often the first factoring recipe to check after extracting the GCF.

Q: Why can a sum of squares $a^2 + b^2$ not be factored over the real numbers?
A: Because any factorization $(a + b)(\dots)$ would require the second factor to produce $+b^2$ from the $b$ term, which forces a minus sign somewhere that cancels to zero in the cross terms — incompatible with having the $a^2$ and $b^2$ both positive. Over the complex numbers, $a^2 + b^2 = (a + bi)(a - bi)$, but over the reals, $a^2 + b^2$ is irreducible (for real $a, b$ with $b\neq 0$).

## 4.5 Recognizing Perfect Square Trinomials

Q: How do you recognize a perfect square trinomial?
A: A trinomial $ax^2 + bx + c$ is a perfect square if $a$ and $c$ are positive perfect squares, and the middle coefficient satisfies $b = \pm 2\sqrt{a}\sqrt{c}$. In that case, it factors as $(\sqrt{a}x + \sqrt{c})^2$ (plus sign) or $(\sqrt{a}x - \sqrt{c})^2$ (minus sign). Example: $x^2 + 6x + 9 = (x + 3)^2$, because $9 = 3^2$ and $6 = 2\cdot 3$.

C: A [perfect square trinomial] has the form $a^2\pm 2ab + b^2 = (a\pm b)^2$, recognizable when the first and last terms are squares and the middle term is twice their product (with appropriate sign).

## 4.6 Factoring Quadratics $x^2 + bx + c$

Q: How do you factor a monic quadratic $x^2 + bx + c$ (leading coefficient 1)?
A: Find two numbers $p$ and $q$ such that $p + q = b$ and $pq = c$. Then $x^2 + bx + c = (x + p)(x + q)$. For example, $x^2 + 5x + 6$: find two numbers summing to 5 and multiplying to 6 → $p = 2, q = 3$ → $(x + 2)(x + 3)$. This is the most common factoring pattern in beginning algebra and should become reflexive with practice.

Q: Why does the sum-and-product method work for factoring $x^2 + bx + c$?
A: Because expanding $(x + p)(x + q) = x^2 + (p + q)x + pq$, which matches $x^2 + bx + c$ if and only if $p + q = b$ and $pq = c$. So factoring reduces to solving a system of two equations in two unknowns. For monic quadratics with integer coefficients, $p$ and $q$ are often easy to find by inspection; for harder cases, the quadratic formula (chapter 6) always works.

## 4.7 Factoring Quadratics $ax^2 + bx + c$

Q: How do you factor a non-monic quadratic $ax^2 + bx + c$ where $a\neq 1$?
A: One method is the "$ac$-method": compute $a\cdot c$ and find two numbers $p$ and $q$ with $p + q = b$ and $pq = ac$. Then rewrite $bx = px + qx$ and factor by grouping: $ax^2 + px + qx + c$. For example, $2x^2 + 7x + 3$: $ac = 6$, numbers summing to 7 and multiplying to 6 are 6 and 1 → $2x^2 + 6x + x + 3 = 2x(x + 3) + (x + 3) = (2x + 1)(x + 3)$. If no such $p, q$ exist, the quadratic does not factor over the rationals.

## 4.8 Factoring Higher-Degree Polynomials

Q: What strategies help factor polynomials of degree 3 or higher?
A: (1) Extract the GCF first. (2) Look for special forms: sum or difference of cubes, recursive differences of squares, etc. (3) Try factoring by grouping for 4+ terms. (4) Use the rational root theorem (chapter 6) to find one root $r$, then divide by $(x - r)$ to reduce the degree by 1, and repeat. (5) Substitute $u = x^k$ to reduce higher-degree polynomials to lower-degree ones when they are "disguised" (e.g., $x^4 - 5x^2 + 4$ is a quadratic in $u = x^2$).

## 4.9 When a Polynomial Is Irreducible

Q: What does it mean for a polynomial to be "irreducible over the rationals" or "irreducible over the reals"?
A: Irreducible over $\mathbb{Q}$ means it cannot be written as a product of two non-constant polynomials with rational coefficients — for example, $x^2 - 2$ is irreducible over $\mathbb{Q}$ (no rational factorization) but reducible over $\mathbb{R}$ as $(x - \sqrt{2})(x + \sqrt{2})$. Irreducible over $\mathbb{R}$ means it cannot be factored into real polynomials of smaller degree; for example, $x^2 + 1$ is irreducible over $\mathbb{R}$ but factors over $\mathbb{C}$ as $(x - i)(x + i)$. The "ground field" matters — it determines what counts as a valid factor.

C: A polynomial is [irreducible] over a field if it cannot be written as a product of two non-constant polynomials with coefficients in that field.

## 4.10 Multi-Step Factoring — P:/S:

P: Factor the polynomial $3x^3 - 27x$ completely over the reals.

S:
**IDENTIFY**: A multi-step factoring problem. Extract the GCF first, then look for a special form in what remains.

**PLAN**:
- Inspect the expression for a common factor in every term.
- Extract the GCF and see what remains inside the parentheses.
- Check the remaining factor for a recognizable pattern: difference of squares, perfect square, etc.
- Apply the pattern and simplify to completion. Verify by expanding.

**EXECUTE**:
1. GCF of $3x^3$ and $-27x$: the constants share a factor of 3, and both terms have at least one $x$. GCF = $3x$.
2. Factor out $3x$: $3x^3 - 27x = 3x(x^2 - 9)$.
3. The remaining factor $x^2 - 9$ is a difference of squares: $x^2 - 3^2 = (x + 3)(x - 3)$.
4. Combine: $3x^3 - 27x = 3x(x + 3)(x - 3)$.
5. Verify by expanding: $3x(x + 3)(x - 3) = 3x(x^2 - 9) = 3x^3 - 27x$. ✓

**EVALUATE**:
- Three factors: $3x$, $(x + 3)$, $(x - 3)$. Each is linear in $x$ (or a constant-times-$x$), and together they multiply to a cubic — consistent with the expected degree.
- Real roots: $x = 0, x = -3, x = 3$. These are exactly the zeros of the cubic, which you can verify by plugging each into $3x^3 - 27x$: $0, -27(-3) + 27(-3) = \dots = 0$, and so on. The three distinct roots match the degree, as expected for a polynomial with three real roots.
- This problem illustrates why the GCF must be extracted *first*: without pulling out $3x$, you'd be trying to factor the full cubic $3x^3 - 27x$ directly, which is harder and obscures the underlying quadratic structure. Always GCF first, then patterns.
- A common mistake is to stop after $3x(x^2 - 9)$, forgetting that $x^2 - 9$ itself factors further. "Complete factorization" means continuing until every factor is either a GCF-type monomial, a linear binomial, or (over the reals) an irreducible quadratic.
- The full factorization $3x(x + 3)(x - 3)$ exposes the three zeros immediately and would let you solve $3x^3 - 27x = 0$ in one glance. This is the payoff: factoring turns polynomial equations into trivial ones by reducing them to "one factor must be zero."
