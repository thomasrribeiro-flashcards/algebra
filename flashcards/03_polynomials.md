+++
order = 3
tags = ["math", "algebra", "polynomials", "monomials", "degree", "multiplication", "identities"]
+++

# Algebra — Polynomials

## 3.1 What a Polynomial Is

C: A [polynomial] in one variable $x$ is an expression of the form $a_n x^n + a_{n-1}x^{n-1} + \cdots + a_1 x + a_0$, where the $a_i$ are real numbers and $n$ is a non-negative integer.

Q: Why are polynomials such a fundamental class of algebraic expressions?
A: Because they involve only the most basic operations — addition, subtraction, and multiplication of a variable by itself (via integer exponents) and by constants. They are closed under addition, subtraction, and multiplication, and they include every monomial, linear expression, and quadratic. Virtually all of elementary algebra, and much of calculus, revolves around polynomials or approximations by polynomials.

## 3.2 Monomials

C: A [monomial] is a polynomial with a single term: a product of a constant (called the coefficient) and a power of the variable, such as $3x^2$ or $-7x^5$.

Q: Why is it useful to think of a general polynomial as a sum of monomials?
A: Because each monomial is independent — its coefficient can be manipulated, added, or scaled without affecting the others. Viewing polynomials as sums of monomials lets you apply operations term-by-term (adding, subtracting, multiplying by constants), and it makes the concepts of "like terms" and "degree" easy to define. Every polynomial operation ultimately reduces to operations on its constituent monomials.

## 3.3 Degree of a Polynomial

C: The [degree] of a polynomial is the largest exponent of the variable that appears with a nonzero coefficient; for a constant polynomial $a_0\neq 0$, the degree is 0.

Q: Why is the degree of the zero polynomial left undefined (or sometimes defined as $-\infty$)?
A: Because the zero polynomial has no nonzero coefficients at all, so there is no "largest exponent with nonzero coefficient" to pick. Assigning degree $-\infty$ is a common convention that makes rules like $\deg(pq) = \deg p + \deg q$ hold in all cases (including when $p$ or $q$ is zero). Without this convention, such rules would have to be stated with exceptions.

Q: Why does the degree of a product of polynomials equal the sum of their degrees?
A: Because multiplying $a_n x^n$ by $b_m x^m$ gives $a_n b_m x^{n+m}$ — the leading term of the product has exponent $n + m$. No higher-degree term can arise from lower-degree terms on either side. So $\deg(pq) = \deg p + \deg q$, assuming neither polynomial is zero.

## 3.4 Names by Degree

Q: What are the common names for polynomials of small degree?
A: Degree 0: a (nonzero) constant. Degree 1: linear. Degree 2: quadratic. Degree 3: cubic. Degree 4: quartic. Degree 5: quintic. These names are worth memorizing because they appear throughout algebra and calculus. "Linear" and "quadratic" in particular recur constantly and are the most important two cases to understand in depth.

C: A polynomial of degree 1 is called [linear], degree 2 is [quadratic], and degree 3 is [cubic].

## 3.5 Like Terms

Q: What are "like terms" in a polynomial, and why can only like terms be combined by addition?
A: Like terms are monomials with the *same variable raised to the same power* — for example, $3x^2$ and $-5x^2$ are like terms but $3x^2$ and $4x$ are not. Only like terms can be combined by adding coefficients: $3x^2 + (-5x^2) = -2x^2$. Unlike terms cannot be simplified into a single monomial — they stay as separate terms in the sum.

## 3.6 Adding and Subtracting Polynomials

Q: How do you add two polynomials?
A: Group like terms together and add their coefficients. For example, $(3x^2 + 2x - 1) + (x^2 - 5x + 4) = (3 + 1)x^2 + (2 - 5)x + (-1 + 4) = 4x^2 - 3x + 3$. Constant terms combine with constant terms, $x$-terms with $x$-terms, and so on. Subtraction is the same, with the second polynomial's coefficients negated first.

## 3.7 Multiplying Polynomials

Q: How do you multiply two polynomials?
A: By distributing every term of the first over every term of the second, then combining like terms. For example, $(x + 2)(x + 3) = x\cdot x + x\cdot 3 + 2\cdot x + 2\cdot 3 = x^2 + 3x + 2x + 6 = x^2 + 5x + 6$. This "FOIL" pattern (First, Outer, Inner, Last) is a mnemonic for two-term-times-two-term multiplications but generalizes to any polynomial product: multiply every term by every term.

C: Multiplying two polynomials is done by [distributing] every term of the first over every term of the second and then combining like terms.

## 3.8 Special Product: Difference of Squares

C: The [difference of squares] identity is $(a + b)(a - b) = a^2 - b^2$.

Q: Why does $(a + b)(a - b) = a^2 - b^2$ have no $ab$ cross term?
A: Expand the product: $(a + b)(a - b) = a\cdot a + a\cdot(-b) + b\cdot a + b\cdot(-b) = a^2 - ab + ab - b^2 = a^2 - b^2$. The two middle terms ($-ab$ and $+ab$) cancel exactly, leaving only the squared terms. This cancellation is why the identity is so clean and why "difference of squares" factors so beautifully.

## 3.9 Special Product: Perfect Square

C: The [perfect square] identities are $(a + b)^2 = a^2 + 2ab + b^2$ and $(a - b)^2 = a^2 - 2ab + b^2$.

Q: Why is $(a + b)^2 = a^2 + 2ab + b^2$ — why the $2ab$ term rather than just $ab$?
A: Because $(a + b)^2 = (a + b)(a + b) = a\cdot a + a\cdot b + b\cdot a + b\cdot b = a^2 + ab + ba + b^2 = a^2 + 2ab + b^2$. The cross term appears *twice* — once from multiplying the first $a$ by the second $b$, and once from multiplying the first $b$ by the second $a$. Forgetting this factor of 2 is one of the most common algebra mistakes.

## 3.10 Cubes

C: The [sum of cubes] factors as $a^3 + b^3 = (a + b)(a^2 - ab + b^2)$, and the [difference of cubes] as $a^3 - b^3 = (a - b)(a^2 + ab + b^2)$.

Q: Why does the difference-of-cubes factorization have an $+ab$ middle term while the sum-of-cubes has $-ab$?
A: Because expanding $(a - b)(a^2 + ab + b^2) = a^3 + a^2 b + ab^2 - a^2 b - ab^2 - b^3$ — the $a^2 b$ terms cancel, as do the $ab^2$ terms, leaving $a^3 - b^3$. Flipping the outer sign $(a + b)$ and the inner sign ($-ab$ to $+ab$) keeps the whole thing consistent. The precise signs are best remembered by noting that the outer factor and the middle term of the inner factor have *opposite* signs.

## 3.11 Polynomial Multiplication — P:/S:

P: Expand $(2x - 3)(x^2 + 4x - 1)$ fully and state the degree and leading coefficient of the result.

S:
**IDENTIFY**: A polynomial multiplication problem. Distribute each term of the first factor over every term of the second, then combine like terms.

**PLAN**:
- Distribute $2x$ over $(x^2 + 4x - 1)$.
- Distribute $-3$ over $(x^2 + 4x - 1)$.
- Sum the two results and combine like terms.
- Read off the degree (highest exponent) and leading coefficient.

**EXECUTE**:
1. $2x\cdot(x^2 + 4x - 1) = 2x^3 + 8x^2 - 2x$.
2. $-3\cdot(x^2 + 4x - 1) = -3x^2 - 12x + 3$.
3. Add: $(2x^3 + 8x^2 - 2x) + (-3x^2 - 12x + 3)$.
4. Combine like terms: $2x^3 + (8 - 3)x^2 + (-2 - 12)x + 3 = 2x^3 + 5x^2 - 14x + 3$.
5. Degree: 3 (the highest exponent). Leading coefficient: 2 (coefficient of $x^3$).

**EVALUATE**:
- Degree $= 3$: ✓ consistent with the rule $\deg(pq) = \deg p + \deg q$: the first factor is linear (degree 1), the second is quadratic (degree 2), and $1 + 2 = 3$. Leading coefficient $2 = 2\cdot 1$, consistent with "leading coefficient of product = product of leading coefficients."
- Sanity check with $x = 1$: $(2\cdot 1 - 3)(1^2 + 4\cdot 1 - 1) = (-1)(4) = -4$. Expanded: $2(1)^3 + 5(1)^2 - 14(1) + 3 = 2 + 5 - 14 + 3 = -4$. ✓
- The sign errors in step 4 are the most common pitfall when multiplying polynomials: a negative sign in the leading factor must be distributed carefully over every term of the second factor. If you see a wrong final sign, the usual culprit is a missed negative in the distribution step.
- The pattern generalizes: multiplying a degree-$m$ polynomial by a degree-$n$ polynomial gives a degree-$(m+n)$ polynomial with at most $m + n + 1$ terms (typically fewer after combining like terms). This bookkeeping helps you check the order of magnitude of a calculation before diving into the details.
- Multiplying polynomials is the bread-and-butter of algebra, appearing in factoring (reverse direction), solving equations by expansion, computing Taylor series, and multiplying matrices of polynomials. The three-step "distribute, sum, combine" procedure is the same in all cases.
