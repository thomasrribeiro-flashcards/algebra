+++
order = 12
tags = ["math", "algebra", "exponential-functions", "logarithms", "natural-log", "compound-interest"]
+++

# Algebra — Exponential and Logarithmic Functions

## 12.1 The Exponential Function

Q: Before a formal definition, predict: what should an "exponential function" $f(x) = b^x$ do differently from a polynomial like $x^b$?
A: In an exponential function the variable $x$ sits in the exponent rather than the base, so each unit increase in $x$ multiplies the output by the fixed factor $b$. Polynomials grow or shrink by adding powers of $x$; exponentials grow or shrink by repeated multiplication. This makes exponentials increase (or decrease) far faster than any polynomial for large $x$.

C: An [exponential function] with base $b$ is a function of the form $f(x) = b^x$, where $b > 0$, $b\neq 1$, and $x$ is any real number.

C: In the exponential function $f(x) = b^x$, the constant [$b$] is called the base and the variable $x$ is the exponent.

Q: What distinguishes an exponential function from a power function?
A: In an exponential function $f(x) = b^x$ the variable is in the exponent and the base is a fixed positive constant. In a power function $f(x) = x^n$ the variable is in the base and the exponent is a fixed constant. They behave very differently: $2^x$ doubles with each unit increase in $x$, while $x^2$ grows quadratically.

## 12.2 Why the Base Restrictions

Q: Why is the base $b$ of an exponential function required to be positive?
A: The base must be positive because $b^x$ must be defined for every real $x$, including fractional exponents like $b^{1/2}$. If $b = -4$, then $b^{1/2}$ would be $\sqrt{-4}$, which is not a real number. More generally, negative bases give non-real outputs at infinitely many rational exponents, so $b^x$ fails to be a real-valued function on $\mathbb{R}$. Requiring $b > 0$ guarantees $b^x$ is defined and real for every real $x$.

Q: Why is $b = 1$ excluded from the definition of an exponential function?
A: Because $1^x = 1$ for every real $x$, so $f(x) = 1^x$ is just the constant function $f(x) = 1$. A constant function has no exponential growth or decay behavior, is not one-to-one, and fails every useful property we want exponentials to have. Excluding $b = 1$ leaves exactly the bases where $b^x$ is a genuinely non-constant function.

Q: Why is $b = 0$ excluded from the definition of an exponential function?
A: If $b = 0$, then $0^x = 0$ for $x > 0$ but $0^0$ is indeterminate and $0^x$ is undefined for $x < 0$ (since $0^{-1} = 1/0$). So $0^x$ is not a well-defined function on all of $\mathbb{R}$. The restriction $b > 0$ rules this out automatically.

## 12.3 Graph Shape — Growth and Decay

C: When the base satisfies $b > 1$, the graph of $f(x) = b^x$ shows exponential [growth]: it is increasing and rises steeply to the right.

C: When the base satisfies $0 < b < 1$, the graph of $f(x) = b^x$ shows exponential [decay]: it is decreasing and approaches zero to the right.

C: Every graph of $f(x) = b^x$ passes through the point $(0,\,[1])$, because $b^0 = 1$ for every allowed base $b$.

C: The graph of $f(x) = b^x$ has a horizontal [asymptote] at $y = 0$, which it approaches but never touches.

Q: For $b > 1$, on which side of the graph does $f(x) = b^x$ approach its horizontal asymptote $y = 0$?
A: As $x \to -\infty$, $b^x \to 0$ from above, so the graph hugs the $x$-axis on the left. On the right ($x \to +\infty$), the graph grows without bound. Decay bases ($0 < b < 1$) reverse this: the graph hugs $y = 0$ on the right and grows without bound on the left.

Q: Why does the graph of $f(x) = b^x$ never touch the $x$-axis?
A: Because $b^x > 0$ for every real $x$ whenever $b > 0$. Any positive number raised to any real power is strictly positive, so the output can get arbitrarily close to zero but can never equal zero. This is exactly why the range is $(0, \infty)$ and $y = 0$ is an asymptote rather than a value taken on.

## 12.4 The Number $e$

Q: Why does the number $e$ deserve a special name in mathematics?
A: The number $e \approx 2.71828$ is the unique base for which the exponential function $e^x$ has slope equal to its own value at every point — that is, $e^x$ is its own derivative. It also arises as the limit of $(1 + 1/n)^n$ as $n \to \infty$, which is exactly what continuous compounding produces. Because of these properties, $e$ makes exponential and logarithmic expressions in calculus dramatically simpler than any other base, which is why it is the "natural" choice.

C: The number $e$ is defined as the limit $e = \lim_{n\to\infty}\left(1 + \frac{1}{n}\right)^n \approx [2.71828]$.

Q: How does $e$ arise from compound interest?
A: If you invest \$1 at 100% annual interest compounded $n$ times per year, your year-end balance is $(1 + 1/n)^n$. As $n \to \infty$ (compounding more and more frequently), this balance approaches $e \approx 2.71828$. So $e$ is literally the year-end value of one dollar at 100% continuously compounded interest, which is why $e$ appears whenever a quantity grows in proportion to its current size.

## 12.5 The Natural Exponential Function

C: The [natural exponential function] is $f(x) = e^x$, where $e \approx 2.71828$ is the natural base.

C: Because $e > 1$, the natural exponential $f(x) = e^x$ is an [increasing] function on all of $\mathbb{R}$.

Q: Why is $e^x$ called the "natural" exponential function if it behaves like any other $b^x$ with $b > 1$?
A: Qualitatively $e^x$ just grows like any exponential with base greater than 1, so its graph shape is not what makes it special. It is "natural" because $e$ is the unique base at which the growth rate of $b^x$ at every point equals the value of $b^x$ itself, making calculus with $e^x$ uniquely clean. Any other base introduces an extra constant factor ($\ln b$) into derivatives and integrals.

## 12.6 Exponentials Are One-to-One

Q: Why is $f(x) = b^x$ (with $b > 0$, $b \neq 1$) a one-to-one function?
A: Because it is strictly monotonic: for $b > 1$ it is strictly increasing, and for $0 < b < 1$ it is strictly decreasing. A strictly monotonic function never takes the same output value twice, so it passes the horizontal line test. Formally, $b^{x_1} = b^{x_2}$ forces $x_1 = x_2$, which is the definition of one-to-one.

Q: Why does being one-to-one matter for exponential functions?
A: A function has an inverse function if and only if it is one-to-one. Since $f(x) = b^x$ is one-to-one, it has an inverse — and that inverse is exactly the logarithm base $b$. Without one-to-oneness we could not speak of "the" logarithm as a function, because solving $b^y = x$ for $y$ could have multiple answers.

## 12.7 The Logarithm as Inverse of the Exponential

C: The [logarithm] base $b$ is defined by $\log_b x = y \iff b^y = x$, where $b > 0$, $b \neq 1$, and $x > 0$.

C: The logarithm $\log_b x$ answers the question: "To what [exponent] must $b$ be raised to produce $x$?"

Q: What does $\log_b x = y$ mean in plain words?
A: It means that $y$ is the exponent you put on $b$ to get $x$ — that is, $b^y = x$. So $\log_2 8 = 3$ because $2^3 = 8$, and $\log_{10} 1000 = 3$ because $10^3 = 1000$. The logarithm and the exponential are two ways of expressing the same relationship, just solved for different variables.

Q: What are $\log_b 1$ and $\log_b b$ for any valid base $b$, and why?
A: $\log_b 1 = 0$ because $b^0 = 1$ for every nonzero base. $\log_b b = 1$ because $b^1 = b$. These two identities follow directly from the definition $\log_b x = y \iff b^y = x$ and are useful sanity checks.

## 12.8 Domain and Range Swap

C: The exponential $f(x) = b^x$ has domain $[\mathbb{R}]$ and range $(0, \infty)$.

C: The logarithm $g(x) = \log_b x$ has domain $(0, \infty)$ and range $[\mathbb{R}]$.

Q: Why do the domains and ranges of $b^x$ and $\log_b x$ swap?
A: Because they are inverse functions, and inverse functions exchange inputs and outputs. Whatever values $b^x$ can take as outputs become the allowed inputs of $\log_b x$, and whatever values $b^x$ accepts as inputs become the outputs of $\log_b x$. Since $b^x$ takes all real inputs and outputs only positive reals, $\log_b x$ takes only positive inputs and outputs all reals.

Q: Why is $\log_b x$ undefined for $x \leq 0$?
A: Because $\log_b x = y$ requires $b^y = x$, and $b^y$ is always positive for any real $y$ when $b > 0$. There is no real exponent that makes $b^y$ equal zero or a negative number, so the equation has no solution and the logarithm is not defined. This is why the domain of every logarithm is strictly $(0, \infty)$.

## 12.9 Common and Natural Logarithms

C: The [common logarithm] is the logarithm base 10, written $\log x$ with the base suppressed: $\log x = \log_{10} x$.

C: The [natural logarithm] is the logarithm base $e$, written $\ln x$: $\ln x = \log_e x$.

Q: What does $\ln x = y$ mean?
A: It means $e^y = x$, i.e., $y$ is the exponent you put on $e$ to get $x$. So $\ln e = 1$, $\ln 1 = 0$, and $\ln e^k = k$ for every real $k$. The natural log is the inverse of the natural exponential $e^x$.

Q: Why are $\log$ (base 10) and $\ln$ (base $e$) singled out with their own notation?
A: Base 10 is natural for human calculation because our number system is decimal, so $\log_{10}$ directly reads off orders of magnitude (e.g., $\log 1000 = 3$). Base $e$ is natural for calculus and for anything growing in proportion to its current size, since $e^x$ is its own derivative. These two bases are so dominant in practice that they get dedicated shorthand.

## 12.10 Product Rule

C: Logarithm product rule: $\log_b(xy) = [\log_b x + \log_b y]$, for $x, y > 0$.

Q: State the product rule for logarithms in words.
A: The log of a product is the sum of the logs of the factors: $\log_b(xy) = \log_b x + \log_b y$, provided $x$ and $y$ are positive and $b$ is a valid base. This converts multiplication of positive numbers into addition of their logarithms.

## 12.11 Quotient Rule

C: Logarithm quotient rule: $\log_b\!\left(\dfrac{x}{y}\right) = [\log_b x - \log_b y]$, for $x, y > 0$.

Q: State the quotient rule for logarithms in words.
A: The log of a quotient is the log of the numerator minus the log of the denominator: $\log_b(x/y) = \log_b x - \log_b y$. This converts division of positive numbers into subtraction of their logarithms.

## 12.12 Power Rule

C: Logarithm power rule: $\log_b(x^r) = [r\log_b x]$, for $x > 0$ and any real $r$.

Q: State the power rule for logarithms in words.
A: The log of a number raised to a power equals the power times the log of the number: $\log_b(x^r) = r\log_b x$. This is the rule that lets you "bring an exponent down in front," which is the single most important move for solving exponential equations.

## 12.13 Why These Rules Hold

Q: Why does $\log_b(xy) = \log_b x + \log_b y$?
A: It is just the exponent rule $b^m \cdot b^n = b^{m+n}$ read backward through the logarithm. Write $x = b^m$ and $y = b^n$, so $m = \log_b x$ and $n = \log_b y$. Then $xy = b^m \cdot b^n = b^{m+n}$, which by definition of the logarithm means $\log_b(xy) = m + n = \log_b x + \log_b y$.

Q: Why does $\log_b(x^r) = r\log_b x$?
A: It comes from the exponent rule $(b^m)^r = b^{mr}$. Write $x = b^m$, so $m = \log_b x$. Then $x^r = (b^m)^r = b^{mr}$, which by the definition of the logarithm means $\log_b(x^r) = mr = r\log_b x$. Every log property is an exponent property in disguise, turned inside out by the inverse relationship.

## 12.14 Change of Base

C: Change-of-base formula: $\log_b x = \dfrac{[\ln x]}{\ln b}$, valid for $x > 0$ and any valid base $b$.

Q: Why is the change-of-base formula useful?
A: Most calculators only compute $\ln$ and $\log_{10}$ directly, so to evaluate something like $\log_7 50$ numerically you rewrite it as $\ln 50 / \ln 7$. The formula also lets you convert between any two bases when simplifying algebraic expressions, because the choice of auxiliary base in the numerator and denominator cancels out.

Q: Derive the change-of-base formula $\log_b x = \dfrac{\ln x}{\ln b}$.
A: Let $y = \log_b x$, which by definition means $b^y = x$. Take $\ln$ of both sides: $\ln(b^y) = \ln x$. By the power rule, $y \ln b = \ln x$, so $y = \ln x / \ln b$. Substituting back gives $\log_b x = \ln x / \ln b$. The same derivation works with any base in place of $\ln$, giving the general form $\log_b x = \log_a x / \log_a b$.

## 12.15 Solving Exponential Equations

Q: What is the general strategy for solving an exponential equation where the variable is in the exponent?
A: Take the logarithm (usually $\ln$) of both sides and apply the power rule $\ln(a^b) = b\ln a$ to bring the exponent down as a coefficient. This converts the exponential equation into a linear (or polynomial) equation in the variable, which can then be solved with ordinary algebra. Any valid base works, but $\ln$ is standard because calculators compute it directly.

C: To solve an equation of the form $b^{f(x)} = c$ with $c > 0$, take $\ln$ of both sides to get $f(x)\ln b = [\ln c]$, then solve for $x$.

## 12.16 Solving Logarithmic Equations

Q: What is the general strategy for solving a logarithmic equation?
A: Combine all logs on one side into a single log using the product, quotient, and power rules, then exponentiate both sides with base $b$ to cancel $\log_b$. This converts $\log_b(\text{expression}) = k$ into $\text{expression} = b^k$, a polynomial or rational equation. After solving, you must check every candidate in the original equation because the domain of $\log_b$ is only $(0, \infty)$.

Q: Why must you check for extraneous solutions when solving logarithmic equations?
A: Because $\log_b x$ is only defined for $x > 0$, any candidate solution that makes the argument of any logarithm in the original equation zero or negative is invalid, even if it satisfies the algebraic equation obtained after exponentiating. Exponentiating enlarges the solution set, so checking in the original equation is the only way to detect these extraneous roots and discard them.

C: Extraneous solutions can appear when solving logarithmic equations because the domain of $\log_b$ is only the [positive] reals, so any candidate that makes a log argument non-positive must be rejected.

## 12.17 Compound Interest

C: For interest compounded $n$ times per year, the balance after $t$ years is $A = P\left(1 + \dfrac{r}{n}\right)^{[nt]}$, where $P$ is the principal, $r$ is the annual interest rate (as a decimal), and $t$ is time in years.

C: For continuously compounded interest, the balance after $t$ years is $A = [Pe^{rt}]$, where $P$ is the principal, $r$ is the annual rate (as a decimal), and $t$ is time in years.

Q: Why does the continuous-compounding formula use $e^{rt}$?
A: As you compound more frequently, $(1 + r/n)^{nt}$ approaches $e^{rt}$ in the limit $n \to \infty$. This is a direct consequence of the definition $e = \lim_{n\to\infty}(1 + 1/n)^n$, rescaled by $r$ and $t$. So $Pe^{rt}$ is exactly what you get by compounding infinitely often — the "perfect" limit of more and more frequent compounding.

Q: How do you solve for the time $t$ required for a continuously compounded investment to reach a target amount $A$?
A: Start from $A = Pe^{rt}$, divide both sides by $P$ to get $A/P = e^{rt}$, then take $\ln$ of both sides: $\ln(A/P) = rt$. Dividing by $r$ gives $t = \ln(A/P)/r$. This is a typical use of logs: the variable lives in the exponent, so $\ln$ is the tool that frees it.

## 12.18 Worked Example — Exponential Equation

P: Solve $3^{2x+1} = 17$ for $x$, expressing the answer in terms of $\ln$.

S:
**IDENTIFY**: Exponential equation with the unknown $x$ in the exponent. Method: take $\ln$ of both sides, use the power rule $\ln(a^b) = b\ln a$ to pull the exponent down, then solve the resulting linear equation.

**PLAN**:
- Take $\ln$ of both sides of $3^{2x+1} = 17$.
- Apply the power rule to move $2x+1$ to the front.
- Solve the resulting linear equation for $x$.

**EXECUTE**:
1. $\ln\!\left(3^{2x+1}\right) = \ln 17$.
2. Power rule: $(2x+1)\ln 3 = \ln 17$.
3. Divide by $\ln 3$: $2x + 1 = \dfrac{\ln 17}{\ln 3}$.
4. Subtract 1: $2x = \dfrac{\ln 17}{\ln 3} - 1$.
5. Divide by 2: $x = \dfrac{1}{2}\!\left(\dfrac{\ln 17}{\ln 3} - 1\right)$.

**EVALUATE**:
- Numerically, $\ln 17 / \ln 3 \approx 2.579$, so $x \approx (2.579 - 1)/2 \approx 0.790$.
- Check: $2x + 1 \approx 2.579$, and $3^{2.579} \approx 17$. ✓
- The answer exists for every positive right-hand side, as expected since the range of $3^{2x+1}$ is $(0,\infty)$.

## 12.19 Worked Example — Logarithmic Equation with Extraneous Check

P: Solve $\log_2(x) + \log_2(x-2) = 3$ for $x$, and check for extraneous solutions.

S:
**IDENTIFY**: Logarithmic equation with two log terms on the same side. Method: combine the logs using the product rule, exponentiate to eliminate the log, solve the resulting polynomial, then test each candidate against the domain of the original logs.

**PLAN**:
- Combine $\log_2 x + \log_2(x-2)$ into a single log using the product rule.
- Exponentiate both sides with base 2 to remove the logarithm.
- Solve the resulting quadratic equation.
- Check each candidate in the original equation: both $x$ and $x-2$ must be positive.

**EXECUTE**:
1. Product rule: $\log_2\!\big(x(x-2)\big) = 3$.
2. Exponentiate: $x(x-2) = 2^3 = 8$.
3. Expand: $x^2 - 2x - 8 = 0$.
4. Factor: $(x-4)(x+2) = 0$, giving candidates $x = 4$ and $x = -2$.
5. Check $x = 4$: $\log_2 4 + \log_2 2 = 2 + 1 = 3$. ✓
6. Check $x = -2$: $\log_2(-2)$ is undefined because $-2 \leq 0$. Reject.

**EVALUATE**:
- Only $x = 4$ is a valid solution; $x = -2$ is extraneous.
- The extraneous root appeared because exponentiating the equation enlarged the solution set to include values outside the domain of the original logarithms.
- This is exactly why every logarithmic equation demands a domain check at the end.
