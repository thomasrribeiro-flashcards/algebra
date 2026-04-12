+++
order = 9
tags = ["math", "algebra", "rational-expressions", "rational-equations", "lcd", "extraneous-solutions"]
+++

# Algebra — Rational Expressions and Equations

## 9.1 What a rational expression is

Q: Why do we study rational expressions as a separate family of algebraic objects?
A: Rational expressions extend polynomial arithmetic to include division by variable quantities. While polynomials are closed under addition, subtraction, and multiplication, they are not closed under division — dividing two polynomials generally produces something that is not itself a polynomial. Rational expressions fill that gap, allowing us to model quantities like rates, proportions, and inverse relationships (e.g., $1/x$). They behave much like numerical fractions, but with the added subtlety that the denominator contains variables and can vanish for certain inputs.

C: A [rational expression] is a ratio $P/Q$ of two polynomials, where $P$ is the numerator and $Q$ is the denominator with $Q\neq 0$.

C: In the rational expression $\frac{x+1}{x^2-4}$, the numerator is $P=x+1$ and the [denominator] is $Q=x^2-4$.

Q: Is every polynomial also a rational expression?
A: Yes. Any polynomial $P$ can be written as $P/1$, which is a ratio of two polynomials whose denominator is the constant polynomial $1$. So polynomials form a subset of rational expressions, just as integers form a subset of rational numbers. The rational expressions that are not polynomials are the ones whose denominators contain at least one non-constant factor.

## 9.2 Domain — excluded values where denominator = 0

Q: Why must the denominator of a rational expression never be zero?
A: Because division by zero is undefined — there is no real number equal to $p/0$. For a rational expression to represent a number at every allowed input, we must exclude every value of the variable that makes the denominator zero. For $\frac{1}{x-3}$, we must exclude $x=3$; for $\frac{x}{x^2-4}$, we must exclude $x=\pm 2$. Finding these exclusions is the first step in analyzing any rational expression because they govern the expression's domain and flag potential extraneous solutions later.

C: The [domain] of a rational expression $P/Q$ is the set of all real numbers $x$ for which $Q(x)\neq 0$.

C: Values of $x$ that make the denominator zero are called [excluded values] (or restrictions) of the rational expression.

Q: How do you find the excluded values of $\frac{x+5}{x^2-x-6}$?
A: Set the denominator equal to zero and solve: $x^2-x-6=0$. Factor as $(x-3)(x+2)=0$, giving $x=3$ or $x=-2$. These are the excluded values, so the domain is all real numbers except $3$ and $-2$. Notice that you factor and solve the denominator before simplifying, because even factors that later cancel still produce excluded values in the original expression.

## 9.3 Simplifying rational expressions (factor + cancel common factors)

Q: Why does simplifying a rational expression require factoring first?
A: A rational expression is simplified by dividing the numerator and denominator by any common factor, just like reducing $\tfrac{6}{9}$ to $\tfrac{2}{3}$ by dividing by $3$. But factors are only visible after fully factoring both numerator and denominator — an unfactored polynomial hides its divisors. So the procedure is always: factor top and bottom completely, then divide out any factor that appears in both.

C: To simplify a rational expression, [factor] the numerator and denominator completely, then cancel any [common factor] that appears in both.

Q: Simplify $\frac{x^2-9}{x^2+5x+6}$ and state the restrictions.
A: Factor: $\frac{(x-3)(x+3)}{(x+2)(x+3)}$. The common factor $(x+3)$ cancels, leaving $\frac{x-3}{x+2}$. The restrictions come from the original denominator $(x+2)(x+3)=0$, giving $x\neq -2$ and $x\neq -3$. Both restrictions must be carried forward even though $(x+3)$ no longer appears — the simplified form is only equal to the original where the original was defined.

## 9.4 Why you cannot "cancel" across addition

Q: Why is it wrong to "cancel" the $x$ in $\frac{x+3}{x}$ to get $3$?
A: Cancellation is division, and division distributes over multiplication but not over addition. In $\frac{x+3}{x}$ the numerator is a sum, not a product, so $x$ is not a factor of the whole numerator — it is only a term. You can split the fraction as $\frac{x}{x}+\frac{3}{x}=1+\frac{3}{x}$, which is clearly not $3$. Cancellation is only legal when the cancelled quantity is a factor of the entire numerator and the entire denominator.

C: You may only cancel a [common factor] — a quantity multiplied by the rest of the numerator and the rest of the denominator — never a term inside a sum.

Q: Spot the error: "$\frac{x^2+4}{x^2}=\frac{4}{1}=4$."
A: The numerator $x^2+4$ is a sum, not a product, so $x^2$ is a term and not a factor. You cannot cancel it against the $x^2$ in the denominator. The correct simplification is $\frac{x^2+4}{x^2}=1+\frac{4}{x^2}$, which depends on $x$ and is certainly not the constant $4$. The general rule: if the numerator or denominator contains a $+$ or $-$ at the top level, factor first to expose genuine factors before cancelling anything.

## 9.5 Multiplying rational expressions

Q: Why is multiplying rational expressions so much easier than adding them?
A: Multiplication distributes naturally over the fraction bar: $\frac{A}{B}\cdot\frac{C}{D}=\frac{AC}{BD}$. No common denominator is needed because we are combining two ratios into one ratio of products. This is the same rule as multiplying numerical fractions. Addition, by contrast, requires a common denominator because $\frac{A}{B}+\frac{C}{D}$ has no single ratio form until both pieces share the same "unit."

C: To multiply rational expressions, use $\frac{A}{B}\cdot\frac{C}{D}=[\frac{AC}{BD}]$, then factor and cancel common factors.

Q: Compute $\frac{x^2-1}{x+2}\cdot\frac{x^2+4x+4}{x-1}$.
A: Factor each piece: $\frac{(x-1)(x+1)}{x+2}\cdot\frac{(x+2)^2}{x-1}$. Multiply straight across: $\frac{(x-1)(x+1)(x+2)^2}{(x+2)(x-1)}$. Cancel the common factors $(x-1)$ and one $(x+2)$: $(x+1)(x+2)$. Restrictions from the originals: $x\neq -2$ and $x\neq 1$. Always factor before multiplying — it avoids expanding huge products that you will just have to factor again to cancel.

## 9.6 Dividing rational expressions (multiply by reciprocal)

Q: Why does dividing by a rational expression become multiplication by its reciprocal?
A: Division is defined as multiplication by the multiplicative inverse: $a\div b = a\cdot b^{-1}$ whenever $b\neq 0$. The multiplicative inverse of the ratio $C/D$ is $D/C$, because $\frac{C}{D}\cdot\frac{D}{C}=1$. So $\frac{A}{B}\div\frac{C}{D}=\frac{A}{B}\cdot\frac{D}{C}$. This is the same "invert and multiply" rule from elementary fractions, justified by the definition of division.

C: To divide rational expressions, use $\frac{A}{B}\div\frac{C}{D}=\frac{A}{B}\cdot[\frac{D}{C}]$, provided $B,C,D$ are nonzero.

Q: When dividing, where do the new excluded values come from?
A: Two places. First, every denominator in the original problem contributes exclusions: $B\neq 0$ and $D\neq 0$. Second, the expression we are dividing by must itself be nonzero, otherwise division is undefined; this forces $C\neq 0$ as well, even though $C$ started in a numerator. Missing this extra restriction is a common source of bugs — always check all four polynomials $A, B, C, D$ when determining the domain.

## 9.7 Adding/subtracting with common denominators

Q: Why do you add the numerators and keep the denominator when denominators already match?
A: The denominator names the "unit" of the fraction — it tells you what size piece you are counting. If two fractions use the same unit, adding them just counts total pieces, so the numerators add and the unit is unchanged. Symbolically, $\frac{A}{D}+\frac{B}{D}=\frac{A+B}{D}$, which follows from the distributive property: $\frac{1}{D}(A)+\frac{1}{D}(B)=\frac{1}{D}(A+B)$.

C: With a common denominator, $\frac{A}{D}\pm\frac{B}{D}=[\frac{A\pm B}{D}]$.

Q: Compute $\frac{2x+1}{x-3}-\frac{x-4}{x-3}$.
A: Same denominator $x-3$, so subtract numerators: $\frac{(2x+1)-(x-4)}{x-3}$. Distribute the minus: $\frac{2x+1-x+4}{x-3}=\frac{x+5}{x-3}$. The most common mistake is forgetting to distribute the subtraction across every term of the second numerator, which here would give a wrong $+(-4)$ instead of $-(-4)=+4$. Restriction: $x\neq 3$.

## 9.8 Least common denominator (LCD) for unlike denominators

Q: Why do we need a least common denominator before adding unlike fractions?
A: Addition requires a shared unit, and the denominator defines that unit. If denominators differ, we first rewrite each fraction with a common denominator — every original denominator must divide it evenly, so multiplying top and bottom by the missing factor doesn't change the value. The least such denominator keeps the numbers small, matching the LCM of the denominators in the numerical case.

C: The [least common denominator (LCD)] of several rational expressions is the product of each distinct factor of any denominator raised to the highest power in which it appears.

Q: Find the LCD of $\frac{1}{x^2-x}$ and $\frac{1}{x^2-1}$.
A: Factor each denominator: $x^2-x=x(x-1)$ and $x^2-1=(x-1)(x+1)$. Collect each distinct factor at its highest power: $x$, $(x-1)$, and $(x+1)$, each appearing to power $1$. The LCD is $x(x-1)(x+1)$. Any larger common denominator would work but would introduce unnecessary factors; this is the smallest that contains both original denominators.

Q: Compute $\frac{1}{x}+\frac{1}{x+2}$.
A: Denominators $x$ and $x+2$ share no factors, so $\text{LCD}=x(x+2)$. Rewrite each: $\frac{1}{x}=\frac{x+2}{x(x+2)}$ and $\frac{1}{x+2}=\frac{x}{x(x+2)}$. Add: $\frac{(x+2)+x}{x(x+2)}=\frac{2x+2}{x(x+2)}=\frac{2(x+1)}{x(x+2)}$. Restrictions: $x\neq 0$ and $x\neq -2$. Always factor the final numerator to check whether further cancellation is possible.

## 9.9 Complex fractions (fractions within fractions)

Q: What is a complex fraction, and why is the LCD-multiplication method usually cleanest?
A: A complex fraction is a rational expression whose numerator, denominator, or both contain fractions themselves, like $\frac{1+\frac{1}{x}}{1-\frac{1}{x}}$. The cleanest technique is to find the LCD of all the "little" fractions and multiply the big numerator and big denominator by that LCD. This clears every inner fraction in one step, converting the complex fraction to a simple ratio of polynomials. The alternative — combining top and bottom separately, then dividing — works but requires more steps.

C: To simplify a complex fraction, multiply its numerator and denominator by the [LCD] of all inner fractions to clear them simultaneously.

Q: Simplify $\dfrac{1+\tfrac{1}{x}}{1-\tfrac{1}{x}}$.
A: The inner LCD is $x$. Multiply top and bottom by $x$: $\frac{x(1+1/x)}{x(1-1/x)}=\frac{x+1}{x-1}$. Restrictions: $x\neq 0$ (from the inner fractions) and $x\neq 1$ (from the resulting denominator). Multiplying top and bottom by the same nonzero quantity does not change the value of the overall fraction, which is why the technique is legal.

## 9.10 Solving rational equations — multiply through by LCD

Q: Why do we multiply a rational equation through by the LCD when solving?
A: Multiplying both sides of an equation by the same nonzero quantity preserves its solution set, and multiplying by the LCD clears every denominator in one step, converting a rational equation into a polynomial equation — which we already know how to solve. The key condition is "nonzero": if the LCD equals zero at some candidate solution, we have multiplied by zero there, which is not a legal step, and that candidate must be rejected at the end.

C: To solve a rational equation, multiply both sides by the [LCD] of all denominators, solve the resulting polynomial equation, then check against the excluded values.

Q: What is the difference between simplifying a rational expression and solving a rational equation?
A: In simplification there is no equals sign, so we cannot multiply by the LCD — we must preserve the expression's value and therefore work within the fraction, keeping a denominator at every step. In an equation, the equals sign lets us multiply both sides by the LCD to clear denominators entirely, because the equation remains true under any nonzero multiplication. Mixing these two workflows is a frequent source of errors.

## 9.11 Extraneous solutions — why checking matters

Q: Why can multiplying by the LCD introduce extraneous solutions?
A: The LCD itself contains the variable, so at excluded values it equals zero. Multiplying both sides by an expression that can be zero is not always reversible: the new polynomial equation may have roots at those excluded values, but the original rational equation is undefined there. Such roots satisfy the cleared equation but not the original one, so they must be discarded. This is why checking every candidate solution against the original denominators is mandatory.

C: A solution to the cleared polynomial equation that makes an original denominator zero is called an [extraneous solution] and must be rejected.

Q: In general, how do you check for extraneous solutions?
A: Identify the excluded values up front by setting each original denominator equal to zero. After solving the cleared polynomial equation, compare every candidate root against that list of excluded values. Any candidate that appears on the list is extraneous and discarded; the rest are genuine solutions. A quick sanity-substitution into the original equation is also useful to catch arithmetic errors during clearing.

## 9.12 P:/S: Solve a rational equation with LCD, catching extraneous solution

P: Solve $\dfrac{x}{x-2}+\dfrac{2}{x-2}=\dfrac{x^2}{x-2}$ for $x$.

S:
**IDENTIFY**: Rational equation with a single common denominator $x-2$. Clear the denominator by multiplying through by the LCD, solve the resulting polynomial equation, then check each candidate against the excluded value $x=2$.

**PLAN**:
- Determine excluded values: $x-2=0\Rightarrow x=2$, so $x\neq 2$.
- LCD $=x-2$. Multiply both sides by $x-2$.
- The result is a quadratic equation; solve by moving everything to one side and factoring.
- Discard any candidate equal to an excluded value.

**EXECUTE**:
1. Exclusions: $x\neq 2$.
2. Multiply both sides by $x-2$: $x + 2 = x^2$.
3. Rearrange: $x^2 - x - 2 = 0$.
4. Factor: $(x-2)(x+1)=0$, giving candidates $x=2$ and $x=-1$.
5. Check: $x=2$ is excluded (makes the denominator zero), so it is extraneous and rejected. $x=-1$ is not excluded.
6. Verify $x=-1$ in the original: $\frac{-1}{-3}+\frac{2}{-3}=\frac{1}{-3}=-\tfrac{1}{3}$ on the left; $\frac{(-1)^2}{-3}=-\tfrac{1}{3}$ on the right. Match.

**EVALUATE**:
- Only $x=-1$ is a valid solution; $x=2$ is extraneous.
- The extraneous root appeared exactly because the LCD $x-2$ is zero there, so the LCD-multiplication step is invalid at $x=2$.
- Both candidate roots and excluded values should always be written down explicitly to avoid missing this kind of rejection.

## 9.13 P:/S: Work/rate word problem (e.g., two workers together)

P: Alice can paint a room alone in $3$ hours, and Bob can paint the same room alone in $6$ hours. How long does it take them to paint the room working together at their individual rates?

S:
**IDENTIFY**: Work-rate problem. The key modeling idea is that "rate" means fraction of job per unit time; rates add when workers work simultaneously, producing a rational equation for the combined time.

**PLAN**:
- Let $t$ be the time in hours for Alice and Bob together.
- Alice's rate is $\tfrac{1}{3}$ room per hour; Bob's rate is $\tfrac{1}{6}$ room per hour.
- Their combined rate is $\tfrac{1}{t}$ room per hour.
- Set up the equation $\tfrac{1}{3}+\tfrac{1}{6}=\tfrac{1}{t}$.
- Solve by multiplying through by the LCD and check the result is positive and consistent.

**EXECUTE**:
1. Define: $t=$ combined time in hours, with $t>0$.
2. Rates: Alice $=1/3$, Bob $=1/6$, together $=1/t$.
3. Equation: $\dfrac{1}{3}+\dfrac{1}{6}=\dfrac{1}{t}$.
4. LCD of $3,6,t$ is $6t$. Multiply through: $2t+t=6$, i.e., $3t=6$.
5. Solve: $t=2$ hours.
6. Check against exclusions: $t=0$ was the only excluded value; $t=2$ is valid.

**EVALUATE**:
- Combined time $t=2$ hours is less than either individual time ($3$ h and $6$ h), as required when two workers help — the combined rate must exceed each individual rate.
- Unit check: $\tfrac{1}{3}+\tfrac{1}{6}=\tfrac{2}{6}+\tfrac{1}{6}=\tfrac{3}{6}=\tfrac{1}{2}$ rooms per hour, and $1/t=1/2$ gives $t=2$ h, consistent.
- The same template (rates add, set equal to $1/t$) handles pipes filling a tank, data transfer, and any other "simultaneous effort" problem.
