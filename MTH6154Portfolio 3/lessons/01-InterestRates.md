# 1. Interest rates

[Back to contents](../README.md)

## Summary

#### The Time value of money

Money has a different value depending on when we receive it.
For example, £1,000 invested today can be worth more than £1,000 received next year because we can put it in a bank and earn interest.
This means an investment made today can grow over time. 
However, inflation can also make the same £1,000 worth less in terms of what it can buy.

The starting amount we invest or borrow is called the **principal**,
$P$. 
The **nominal annual interest rate**,
$r$,
is the stated annual interest rate expressed as a decimal. 
For example, 5%, is written as $r$ = 0.05. 

If we borrow $P$ for one year, the interest charged is $r$$P$. The total amount we owe is therefore: 
              $P$ + $r$$P$ = $P(1+r)$
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

Here, T is the number of years. For semiannual compounding (n=2):

$P(T) = P\left(1+\frac{r}{2}\right)^2T$

More frequent compounding, generally increases the accumulated balance if $r$ >0. 

#### Effective Annual Interest Rate

The **effective annual rate** measures the actual yearly return, including compounding.

It is calculated as:

$r_{\mathrm{eff}}=\left(1+\frac{r}{n}\right)^n-1$
This allows rates with different compounding frequencies to be compared.

#### Continuous Compounding 
With **continuous compounding**, interest is added increasingly frequently. In notation: $\(n\to\infty\)$

$r_{\mathrm{eff}}=\left(1+\frac{r}{n}\right)^n-1$

This allows us to compare investments with different compounding frequencies to be compared fairly.







In your own words, the main ideas of the lesson. Short sentences are fine.

Maths is written between dollar signs. For example `$A = P(1+i)^n$` shows
as $A = P(1+i)^n$, and a displayed formula uses double dollars:

$$
\left(1+\frac{i^{(m)}}{m}\right)^m = 1+i
$$

## My example

A situation you made up (your own numbers, not the ones in the lecture
notes), worked step by step.

## Solved exercises

### Exercise 1.x (from Exercise Sheet 1)

Question, then your solution.

## Spreadsheet

[01-InterestRates.xlsx](../spreadsheets/01-InterestRates.xlsx): what it
does, which cells to change and what to look at.
