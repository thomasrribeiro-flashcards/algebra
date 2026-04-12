+++
order = 13
tags = ["math", "algebra", "sequences", "series", "arithmetic", "geometric", "binomial-theorem"]
+++

# Algebra — Sequences and Series

## 13.1 What a sequence is

Q: Why is a sequence formally defined as a function whose domain is the natural numbers?
A: A sequence assigns to every positive integer $n$ a unique value $a_n$, which is exactly what a function does — it maps inputs to outputs. The domain is the natural numbers $\{1, 2, 3, \ldots\}$ (or sometimes $\{0, 1, 2, \ldots\}$) because sequences are ordered lists, and the natural numbers provide the ordering. This framing matters because it lets us apply all the tools of functions — limits, growth rates, graphs — to lists of numbers.

C: A [sequence] is a function whose domain is the [natural numbers]; its outputs $a_1, a_2, a_3, \ldots$ are called the [terms] of the sequence.

C: The [general term] or $n$th term of a sequence is denoted $a_n$, where $n$ is a [natural number] index.

## 13.2 Explicit vs recursive definitions

Q: What is the difference between an explicit and a recursive definition of a sequence, and when is each useful?
A: An explicit (closed-form) definition gives $a_n$ directly as a formula in $n$, so you can compute any term without computing earlier ones — e.g., $a_n = 2n+1$. A recursive definition specifies one or more starting terms plus a rule that builds each new term from previous ones — e.g., $a_1 = 3,\ a_n = a_{n-1}+2$. Explicit forms are better for jumping to a far-away term; recursive forms are better when the rule for generating terms is simpler than any closed form (e.g., Fibonacci).

C: An [explicit formula] for a sequence expresses $a_n$ directly in terms of [$n$].

C: A [recursive formula] defines $a_n$ in terms of one or more [previous terms], together with one or more [initial terms].

## 13.3 Arithmetic sequences

Q: Why is the defining feature of an arithmetic sequence a constant difference rather than a constant ratio?
A: An arithmetic sequence models quantities that grow by adding the same amount each step — like saving a fixed amount per month. The constant feature is the difference $a_{n+1} - a_n$, called the common difference $d$. Sequences with a constant ratio instead describe multiplicative growth and are called geometric, not arithmetic. Fixing the difference forces each new term to be the previous term plus $d$, which produces the uniform linear spacing characteristic of arithmetic sequences.

C: An [arithmetic sequence] is a sequence in which the difference between consecutive terms is constant; this constant is called the [common difference] $d$.

C: Recursively, an arithmetic sequence satisfies $a_n = [a_{n-1} + d]$, where $d$ is the common difference and $a_1$ is the first term.

## 13.4 $n$th term formula for arithmetic sequences

Q: Why does the $n$th term of an arithmetic sequence equal $a_1 + (n-1)d$ rather than $a_1 + nd$?
A: Starting at $a_1$, each step adds $d$. To reach $a_2$ requires 1 step, $a_3$ requires 2 steps, and $a_n$ requires $n-1$ steps — because you are already at $a_1$ before taking any steps. Adding $d$ a total of $n-1$ times gives $a_n = a_1 + (n-1)d$. Writing $a_1 + nd$ would double-count by adding one extra $d$, giving $a_{n+1}$ instead of $a_n$.

C: For an arithmetic sequence, the $n$th term is $a_n = [a_1 + (n-1)d]$, where $a_1$ is the first term and $d$ is the common difference.

P: Find the 20th term of the arithmetic sequence $3, 7, 11, 15, \ldots$
S:
**IDENTIFY:** Arithmetic sequence with $a_1 = 3$; find $a_{20}$.
**PLAN:** Compute $d = a_2 - a_1$, then apply $a_n = a_1 + (n-1)d$ with $n=20$.
**EXECUTE:** $d = 7 - 3 = 4$. Then $a_{20} = 3 + (20-1)(4) = 3 + 76 = 79$.
**EVALUATE:** Check $d$ is consistent: $11-7=4$, $15-11=4$. Check: $a_{20}$ is 19 steps of 4 past 3, i.e. $3+76=79$. Correct.

## 13.5 What a series is

Q: Why do we distinguish between a sequence and a series?
A: A sequence is a list of terms $a_1, a_2, a_3, \ldots$, while a series is the sum of those terms: $a_1 + a_2 + a_3 + \cdots$. The distinction matters because a sequence can have a simple pattern while its sum behaves very differently — for example, $a_n = 1/2^n$ is a shrinking sequence whose partial sums approach 1. Separating the list from its sum lets us ask different questions: what is the $n$th term? versus what is the total?

C: A [series] is the [sum] of the terms of a sequence; a [finite series] sums finitely many terms, and an [infinite series] sums infinitely many.

C: The $n$th [partial sum] $S_n$ of a series is the sum of its first [$n$] terms: $S_n = a_1 + a_2 + \cdots + a_n$.

## 13.6 Sum of a finite arithmetic series

Q: Why does the finite arithmetic series formula $S_n = \frac{n}{2}(a_1 + a_n)$ work?
A: Write $S_n = a_1 + a_2 + \cdots + a_n$ and also $S_n = a_n + a_{n-1} + \cdots + a_1$ (reversed). Add the two equations term by term: each paired sum equals $a_1 + a_n$ because in an arithmetic sequence, moving one step forward from the small end and one step backward from the large end preserves the total. There are $n$ such pairs, giving $2S_n = n(a_1 + a_n)$, so $S_n = \frac{n}{2}(a_1+a_n)$. Geometrically, this is the average of the first and last term times the count.

C: The sum of the first $n$ terms of an arithmetic series is $S_n = [\frac{n}{2}(a_1 + a_n)]$, where $a_1$ is the first term and $a_n$ is the $n$th term.

C: Substituting $a_n = a_1 + (n-1)d$ gives an equivalent form: $S_n = [\frac{n}{2}(2a_1 + (n-1)d)]$, useful when $a_n$ is not known directly.

## 13.7 Geometric sequences

Q: Why does a constant ratio produce exponential rather than linear behavior?
A: Each term of a geometric sequence is the previous term multiplied by $r$, so after $n-1$ multiplications, the first term has been scaled by $r^{n-1}$. Repeated multiplication is exponential growth (or decay if $|r|<1$), not linear, because the change at each step scales with the current value rather than being fixed. This is the same mechanism behind compound interest and population growth.

C: A [geometric sequence] is a sequence in which the ratio of consecutive terms is constant; this constant is called the [common ratio] $r$.

C: Recursively, a geometric sequence satisfies $a_n = [r \cdot a_{n-1}]$, where $r$ is the common ratio and $a_1$ is the first term.

## 13.8 $n$th term formula for geometric sequences

Q: Why is the $n$th term of a geometric sequence $a_1 r^{n-1}$ and not $a_1 r^n$?
A: Starting from $a_1$, each step multiplies by $r$. Reaching $a_2$ takes 1 multiplication, $a_3$ takes 2, and $a_n$ takes $n-1$ multiplications. So $a_n = a_1 \cdot r^{n-1}$. Using $r^n$ would apply one extra multiplication and give $a_{n+1}$ instead. The $n-1$ exponent mirrors the $(n-1)d$ in the arithmetic formula: both count steps taken after the starting term.

C: For a geometric sequence, $a_n = [a_1 r^{n-1}]$, where $a_1$ is the first term, $r$ is the common ratio, and $n$ is the term index.

P: Find the 8th term of the geometric sequence $5, 10, 20, 40, \ldots$
S:
**IDENTIFY:** Geometric sequence with $a_1 = 5$; find $a_8$.
**PLAN:** Determine $r = a_2/a_1$, then apply $a_n = a_1 r^{n-1}$ with $n=8$.
**EXECUTE:** $r = 10/5 = 2$. Then $a_8 = 5 \cdot 2^{8-1} = 5 \cdot 128 = 640$.
**EVALUATE:** Confirm ratio: $20/10 = 2$, $40/20 = 2$. Listing: $5, 10, 20, 40, 80, 160, 320, 640$. The 8th term is $640$. Correct.

## 13.9 Sum of a finite geometric series

Q: Why does the finite geometric series formula $S_n = a_1 \frac{1-r^n}{1-r}$ hold?
A: Write $S_n = a_1 + a_1 r + a_1 r^2 + \cdots + a_1 r^{n-1}$. Multiply both sides by $r$: $rS_n = a_1 r + a_1 r^2 + \cdots + a_1 r^n$. Subtract: $S_n - rS_n = a_1 - a_1 r^n$, because all intermediate terms cancel. Factoring gives $(1-r)S_n = a_1(1 - r^n)$, so $S_n = a_1 \frac{1-r^n}{1-r}$, valid whenever $r \neq 1$.

C: The sum of the first $n$ terms of a geometric series is $S_n = [a_1 \frac{1-r^n}{1-r}]$, valid for $r \neq 1$, where $a_1$ is the first term and $r$ is the common ratio.

C: When $r = 1$, every term equals $a_1$, so the sum is simply $S_n = [n \cdot a_1]$; the general formula fails because the denominator $1-r$ would be zero.

## 13.10 Infinite geometric series and convergence

Q: Why does an infinite geometric series converge only when $|r| < 1$?
A: Each term is $a_1 r^{n-1}$. For the running sum to approach a finite limit, the terms must shrink to zero, which happens only when $|r| < 1$. If $|r| \geq 1$, the terms don't shrink — they stay the same size or grow — and the partial sums grow without bound (or oscillate without settling). The derivation: $S_n = a_1\frac{1-r^n}{1-r}$; as $n\to\infty$, $r^n\to 0$ exactly when $|r|<1$, giving the limit $S = \frac{a_1}{1-r}$.

C: An infinite geometric series converges if and only if its common ratio satisfies [$|r| < 1$]; otherwise it diverges.

## 13.11 Sum of an infinite geometric series

Q: Why does the infinite geometric sum formula drop the $r^n$ term from the finite version?
A: Starting from $S_n = a_1 \frac{1-r^n}{1-r}$, we take the limit as $n\to\infty$. When $|r| < 1$, $r^n \to 0$, so the numerator $1 - r^n \to 1$. The entire expression approaches $\frac{a_1}{1-r}$. The $r^n$ term disappears because, geometrically, what remains to be summed after $n$ terms shrinks to nothing as $n$ grows.

C: For $|r| < 1$, the sum of an infinite geometric series is $S = [\frac{a_1}{1-r}]$, where $a_1$ is the first term and $r$ is the common ratio.

P: Determine whether the infinite geometric series $8 + 6 + 4.5 + 3.375 + \cdots$ converges, and if so find its sum.
S:
**IDENTIFY:** Infinite geometric series with $a_1 = 8$; need to test convergence and, if convergent, compute $S$.
**PLAN:** Find $r = a_2/a_1$; check whether $|r| < 1$; if yes, apply $S = \frac{a_1}{1-r}$.
**EXECUTE:** $r = 6/8 = 0.75$. Since $|0.75| < 1$, the series converges. Sum: $S = \frac{8}{1 - 0.75} = \frac{8}{0.25} = 32$.
**EVALUATE:** Verify ratio: $4.5/6 = 0.75$, $3.375/4.5 = 0.75$. Partial sums $8, 14, 18.5, 21.875, \ldots$ are increasing toward 32, consistent with the limit.

## 13.12 Sigma notation

Q: Why is sigma notation preferred over writing a series out with $+ \cdots +$?
A: Sigma notation is unambiguous: $\sum_{k=1}^{n} a_k$ states exactly the index variable ($k$), the lower bound ($1$), the upper bound ($n$), and the formula for each term ($a_k$). Writing $a_1 + a_2 + \cdots + a_n$ relies on the reader to guess the pattern from the ellipsis, which fails when the pattern is complex. Sigma notation also composes cleanly: you can manipulate bounds, split sums, and factor constants using algebraic rules.

C: In sigma notation, $\sum_{k=1}^{n} a_k$ means the sum of $a_k$ as $k$ runs from [$1$] to [$n$]; the variable $k$ is the [index of summation].

C: Two useful rules: $\sum_{k=1}^{n}(c \cdot a_k) = [c \sum_{k=1}^{n} a_k]$ (factor constants out) and $\sum_{k=1}^{n}(a_k + b_k) = [\sum a_k + \sum b_k]$ (sums split across addition).

## 13.13 The binomial theorem and Pascal's triangle

Q: Why do the coefficients in the expansion of $(a+b)^n$ form Pascal's triangle?
A: Expanding $(a+b)^n$ means choosing, from each of $n$ factors, either $a$ or $b$. The coefficient of $a^{n-k} b^k$ counts how many ways to pick $b$ from $k$ of the $n$ factors, which is $\binom{n}{k}$. Pascal's triangle is built by the identity $\binom{n}{k} = \binom{n-1}{k-1} + \binom{n-1}{k}$: each entry is the sum of the two above it, because selecting $k$ items from $n$ either includes the last item (leaving $k-1$ from $n-1$) or excludes it (leaving $k$ from $n-1$). This combinatorial structure is the reason the triangle and the expansion coincide.

C: The [binomial theorem] states $(a+b)^n = \sum_{k=0}^{n} \binom{n}{k} a^{n-k} b^k$, where $\binom{n}{k} = [\frac{n!}{k!(n-k)!}]$ is the binomial coefficient.

C: Pascal's triangle has [1]s on the edges, and each interior entry is the [sum of the two entries directly above it]; row $n$ gives the coefficients of $(a+b)^n$.

C: In the expansion of $(a+b)^n$, the exponent of $a$ [decreases] from $n$ to $0$ while the exponent of $b$ [increases] from $0$ to $n$, and the two exponents in each term always sum to [$n$].

## 13.14 P:/S: Sum a specific finite arithmetic series

P: Find the sum of the first 30 terms of the arithmetic series $4 + 9 + 14 + 19 + \cdots$
S:
**IDENTIFY:** Arithmetic series with $a_1 = 4$; need $S_{30}$.
**PLAN:** Find $d$, compute $a_{30}$ using $a_n = a_1 + (n-1)d$, then apply $S_n = \frac{n}{2}(a_1 + a_n)$.
**EXECUTE:** $d = 9 - 4 = 5$. $a_{30} = 4 + (30-1)(5) = 4 + 145 = 149$. $S_{30} = \frac{30}{2}(4 + 149) = 15 \cdot 153 = 2295$.
**EVALUATE:** Cross-check with the alternate form: $S_{30} = \frac{30}{2}(2(4) + 29(5)) = 15(8 + 145) = 15 \cdot 153 = 2295$. Both forms agree.

## 13.15 P:/S: Determine convergence of an infinite geometric series and find its sum

P: Does the infinite geometric series $\sum_{k=1}^{\infty} 12 \left(-\frac{2}{3}\right)^{k-1}$ converge? If so, find its sum.
S:
**IDENTIFY:** Infinite geometric series in sigma form with $a_1 = 12$ (value at $k=1$) and $r = -\tfrac{2}{3}$.
**PLAN:** Check the convergence condition $|r| < 1$; if satisfied, apply $S = \frac{a_1}{1-r}$.
**EXECUTE:** $|{-2/3}| = 2/3 < 1$, so the series converges. $S = \frac{12}{1 - (-2/3)} = \frac{12}{1 + 2/3} = \frac{12}{5/3} = 12 \cdot \frac{3}{5} = \frac{36}{5} = 7.2$.
**EVALUATE:** Since $r$ is negative, partial sums should oscillate around the limit: $S_1 = 12$, $S_2 = 12 - 8 = 4$, $S_3 = 4 + 16/3 \approx 9.33$, $S_4 \approx 9.33 - 32/9 \approx 5.78$, alternating tightening around $7.2$. Consistent with convergence to $36/5$.
