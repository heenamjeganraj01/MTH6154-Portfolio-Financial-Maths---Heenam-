# 1. Interest rates

[Back to contents](../README.md)

## Summary

#### The Time value of money

Money has a different value depending on when we receive it.
For example, £5,000 invested today can be worth more than £15,000 received next year because we can put it in a bank and earn interest.
This means an investment made today can grow over time. 
However, inflation can also make the same £1,000 worth less in terms of what it can buy.

The starting amount we invest or borrow is called the **principal**,
$P$. 

#### Nominal Annual Interest Rate

The **nominal annual interest rate**,
$r$,
is the stated annual interest rate expressed as a decimal. 
For example, 5%, is written as $r$ = 0.05. 

If we borrow $P$ for one year, the interest charged is $rP$. The total amount we owe is therefore: 
$P$ + $rP$ = $P(1+r)$. 
The same applies to a savings situation.

#### Compound Interest

Compound interest means earning interest on both your original money and previously earned interest. This means the balance can grow faster over time.

When interest is added once a year, called **annual compounding**, the amount after $T$ years is:
$P(T)$ = $P(1+r)^T$

For example when T=1: 

$P(1) = P(1+r)$

However, banks may add interest more frequently. If interest is compounded $n$ times per year for $T$ years, where each period uses the rate $r/n$: 

$P(T) = P\left(1+\frac{r}{n}\right)^{nT}$

where: 
- $P$ = initial principal
- $P(T)$ = accumulated balance
- $r$ = nominal annual interest rate
- $n$ = compounding periods per year
- $T$ = investment duration in years

Examples of compounding frequencies: 

- Annually: $n=1$
- Semiannually: $n=2$
- Quarterly: $n=4$
- Monthly: $n=12$
- Daily: $n=365$

Here, T is the number of years. 

For semiannual compounding (n=2):
$P(T) = P\left(1+\frac{r}{2}\right)^{2T}$

More frequent compounding, generally increases the accumulated balance if $r$ >0. 

#### Effective Annual Interest Rate

The **effective annual rate **$r_{\mathrm{eff}}$** measures the actual yearly return, after accounting for how often interest is added:

$r_{\mathrm{eff}}=\left(1+\frac{r}{n}\right)^n-1$

This allows rates with different compounding frequencies to be compared.

#### Continuous Compounding 
With **continuous compounding**, interest is added increasingly frequently. In notation: $\n\to\infty\$: 

$\lim_{n\to\infty}P\left(1+\frac rn\right)^{nT}
=Pe^{rT}$

Therefore: 

$P(T)=Pe^{rT},\qquad r_{\mathrm{eff}}=e^r-1$
Using the **effective annual rate**, we can also write $\(P(T)=P(1+r_{\mathrm{eff}})^T\)$. These formulas also apply to loans when no repayments are made. 

#### Doubling Time

**Doubling Time** tells us how long money takes to double under **continuous compounding**:

Let $T$ represent the amount of years it takes an amount $P$ to double, we have 

$\[2P=Pe^{rT}\quad\Rightarrow\quad\boxed{T=\frac{\ln2}{r}\approx\frac{0.693}{r}}\]$, by rearranging to solve $T$.

The **Rule of 72** is a quick estimate: 
$\[T\approx\frac{72}{R}\]$,
where $R$ is the interest rate written as a percentage.

### Variable Interest Rates
#### Instantaneous Interest Rate
Interest rates can change over time. The **instantaneous interest rate $r(t)$** tells us the rate at a particular moment. 

Let **$r(t)$** be the interest rate at time **$t$**, **$P(t)$** the balance at that time, and **$P(0)$** the starting balance at **time zero**. 

Over a very short time interval $h$, the interest rate is approximately constant. Using $\(e^{r(t)h}\approx1+r(t)h\)$ we can calculate the amount of interest that occurs between time $t$ and $t+h$: 

$\[P(t+h)\approx P(t)e^{r(t)h}\approx P(t)(1+r(t)h)\]£
This means that the balance is approximately the current balance plus the interest earned. As $h$ approaches zero:

$\[\{P'(t)=P(t)r(t)}\]$






So the balance changes approximately by: 
$\[P(t+h)\approx P(t)(1+hr(t))\]$
as 









## My example

A situation you made up (your own numbers, not the ones in the lecture
notes), worked step by step.

## Solved exercises

### Exercise 1.x (from Exercise Sheet 1)

Question, then your solution.

## Spreadsheet

[01-InterestRates.xlsx](../spreadsheets/01-InterestRates.xlsx): what it
does, which cells to change and what to look at.
